# RED ROOM — Le Serveur Maudit
## Bible de production (v1.0)

> Document de référence pour l'équipe qui monte le jeu.
> **Script complet** : `story-pipeline/draft.md` (dialogues, scènes, interventions de combat).
> **Fiches personnages** : `story-pipeline/characters.md` · **Intrigue** : `story-pipeline/plot.md` · **Brief et règles** : `story-pipeline/input.md`.
> Les références de scène (ex. **1-6**, **F-4**) renvoient aux scènes du script.
> Toutes les valeurs chiffrées (PV, dégâts, prix, niveaux) sont **indicatives, à équilibrer** en playtest.

---

## 0. Sommaire

1. Le projet en une page
2. Moteur et conventions techniques
3. Structure du jeu et durée
4. Personnages jouables
5. Compagnons, guides et personnages clés
6. Compétences
7. États (statuts)
8. Objets
9. Équipements
10. Ennemis communs
11. Boss
12. Cartes
13. PNJ
14. Énigmes
15. Événements communs (mécaniques récurrentes)
16. Switches et variables (flags)
17. Cinématiques et scènes scriptées
18. Audio
19. Liste des assets graphiques
20. Placeholders à compléter
21. Mon avis, risques et recommandations
22. Plan de travail et quand me solliciter

---

## 1. Le projet en une page

| | |
|---|---|
| **Titre** | Red Room — Le Serveur Maudit |
| **Genre** | RPG classique au tour par tour, comédie fantastique loufoque |
| **Public** | Privé : la Red Room et ses proches. Pas de diffusion publique. |
| **Durée cible** | 3 à 4 heures |
| **Pitch** | Une nuit, Jordan clique sur un lien « free RP 100% legit » posté sur le Discord de la Red Room. Le serveur est corrompu et il est aspiré dedans. Chaque salon est devenu un royaume tenu par le **Modérateur Fou**. Il doit retrouver ses sept amis un par un, réunir les sept fragments du Premier Message de la Red Room et monter dans la Tour des Modérateurs. Tout le monde accuse Camil. Le vrai cerveau, c'est **Ceyn**. |
| **Ton** | Léger, absurde, affectueux. On rit **avec** les potes, pas contre eux. |
| **Règles de design** | Combats 100 % standards (attaque, compétences, objets, fuite). Le loufoque est dans l'habillage. Boss avec phases et **interventions scriptées** (un personnage arrive, parle, donne un objet, affaiblit ou renforce le boss). Énigmes variées et simples. Pas de mécanique de réflexe. |

**Les huit héros** : Jordan (protagoniste), José, Kevin, Bidou, Robin, Florian, Yanis, Alex.
**Compagnons** : Snow (le chat de Jordan), Clyde (vieux bot guide).
**Antagonistes** : le Modérateur Fou (bot), Camil (faux cerveau, vrai méchant), Ceyn (vrai cerveau, révélé au final).

---

## 2. Moteur et conventions techniques

### Recommandation : RPG Maker MZ
- Combat au tour par tour natif, base de données (acteurs, classes, compétences, états, objets, ennemis, troupes) prête à l'emploi.
- Les **interventions de boss** se font avec les **événements de troupe** (conditions « Tour X » ou « PV de l'ennemi ≤ X % »), sans code.
- Les **mécaniques récurrentes** (gag « Ceyn. », pet de Snow, drague de José) sont des **événements communs**.
- Énigmes de glace, blocs à pousser, interrupteurs, dalles : réalisables en événements standard (nombreux tutoriels).
- Plugins utiles (gratuits, à choisir par l'équipe) : messages avec visages et noms, système d'équipe et réserve, affichage de texte en jeu (bulles).

### Alternative : Godot 4
- Plus de liberté visuelle, mais tout le système de combat et d'inventaire est à coder.
- Si Godot est choisi : reprendre les tableaux de ce document comme fichiers de données (JSON ou ressources `.tres`), et implémenter les flags comme un dictionnaire global (`GameState.flags`, `GameState.vars`).

### Conventions de nommage
| Type | Préfixe | Exemple |
|---|---|---|
| Carte | `M` + numéro | `M11` Stade Orbital |
| PNJ | `N` + numéro | `N015` Abeille Marchande |
| Objet | `I` + numéro | `I001` Chips |
| Équipement | `E` + numéro | `E010` Médiator de Bard |
| Objet clé | `K` + numéro | `K001` Fragment 1/7 |
| Compétence | `SK` + numéro | `SK020` Riff Saturé |
| État | `ST` + numéro | `ST03` Muet |
| Ennemi | `EN` + numéro | `EN010` Spam-bot |
| Boss | `B` + numéro | `B02` Reine de la Ruche |
| Switch | `S` + numéro | `S001` snow_a_clique |
| Variable | `V` + numéro | `V001` rateaux_jose |
| Événement commun | `CE` + numéro | `CE01` Gag « Ceyn. » |
| Musique | `BGM_` | `BGM_Generalia` |
| Son | `SE_` | `SE_Prrrt` |

### Format du script (`draft.md`)
`[DÉCOR]` décor · `[MUSIQUE]` / `[SFX]` son · `[ÉVÉNEMENT]` action scriptée · `[CHOIX]` choix · `[COMBAT]` combat · `[DISCORD]` faux message affiché (boîte de dialogue ou texte dans le ciel) · `[FLAG]` switch ou variable · `NOM :` réplique · *(didascalie)*.

---

## 3. Structure du jeu et durée

| # | Chapitre | Salon / zone | Recrue | Énigme principale | Boss | Niveau équipe conseillé | Durée |
|---|---|---|---|---|---|---|---|
| P | Prologue | QG de Jordan | — | — | — | 1 | 5 min |
| 1 | Généralia | #général | José, Snow, Clyde | Cloches (objets) + mot de passe | Gardien des Épinglés | 5 | 25 min |
| 2 | Le Stade Orbital | #rocket-league | Kevin | Quête du Kop Rouge (objets) | Reine de la Ruche | 8 | 25 min |
| 3 | Les Cimes Sans Air | #vocal-1 | Bidou | Lac gelé (glace) + quiz | Grand Mute | 11 | 20 min |
| 4 | La Base d'Annonces | #annonces | Robin | Interrupteurs + slogans | Adjudant @everyone | 14 | 25 min |
| 5 | Les Enfers du Classé | #classé | Florian | Blocs à pousser | Juge du Matchmaking | 17 | 20 min |
| 6 | Le Marais d'AFK | #afk | Yanis | Labyrinthe (miettes) | Sablier d'Inactivité | 20 | 20 min |
| 7 | Les Terres Lointaines | hors serveur (Toulouse) | Alex | Dalles du combo (Q Q W R) | Démon du Lag | 23 | 25 min |
| I | Le Barbecue | Jardin de Camil (hub) | — | PowerPoint (dialogue) | — | 23 | 15 min |
| F | La Tour des Modérateurs | Tour | — | Miroirs | Golem de Vaisselle, Camil, Ceyn | 26 à 28 | 35 min |
| | | | | | | **Total** | **≈ 3 h 30** |

### Progression de l'équipe
| Après | Membres disponibles | En combat |
|---|---|---|
| Ch. 1 | Jordan, José | 2 |
| Ch. 2 | + Kevin | 3 |
| Ch. 3 | + Bidou | 4 |
| Ch. 4 | + Robin | 4 (+1 réserve, **système de réserve activé**) |
| Ch. 5 | + Florian | 4 (+2) |
| Ch. 6 | + Yanis | 4 (+3) |
| Ch. 7 | + Alex | 4 (+4) |

### Combats à équipe imposée
| Combat | Contrainte |
|---|---|
| B02 Reine de la Ruche | Jordan, José, Kevin (seuls disponibles) |
| B03 Grand Mute | Jordan, José, Kevin, Bidou |
| B05 Juge du Matchmaking | Florian obligatoire |
| B06 Sablier d'Inactivité | Yanis obligatoire |
| B07 Démon du Lag | Alex obligatoire |
| B09 Camil | **Kevin interdit** (il passe en réserve automatiquement, règle d'écriture : aucune interaction Kevin / Camil) |
| B10 Ceyn | Libre |

### Carte du monde
Un écran de sélection façon **liste de salons Discord** (colonne de gauche) remplace la carte classique. Les salons se débloquent au fil de l'histoire :
- après le ch. 1 : `#rocket-league`, `#vocal-1` ;
- après le ch. 3 : `#annonces` ;
- après le ch. 4 : `#classé` ;
- après le ch. 5 : `#afk` ;
- après le ch. 6 : la route vers les **Terres Lointaines** (hors liste, un lien « ping 400 » en bas) ;
- après le ch. 7 : `Jardin de Camil` puis `Tour des Modérateurs`.

`#général` (Généralia) reste accessible comme ville-hub (boutique, auberge).

---

## 4. Personnages jouables

### Profils de stats (★ = relatif, 1 à 5)
| Héros | Rôle | PV | Magie | Atk | Déf | Mag | Vit | Particularité |
|---|---|---|---|---|---|---|---|---|
| **Jordan** | Tireur / soigneur (Senna) | ★★★ | ★★★★ | ★★★ | ★★ | ★★★★ | ★★★ | Protagoniste, toujours dans l'équipe |
| **José** | Combattant rapide (Neon) | ★★★ | ★★ | ★★★★ | ★★★ | ★ | ★★★★★ | Agit souvent en premier |
| **Kevin** | Gros dégâts (Rocket League) | ★★★ | ★★★ | ★★★★★ | ★★ | ★★★ | ★★★ | Fort contre les volants |
| **Bidou** | Support (Bard) | ★★ | ★★ (Souffle) | ★★★ | ★★★ | ★★★★ | ★★★ | Magie renommée **Souffle**, petite réserve, bonne régénération |
| **Robin** | Tank (Garen) | ★★★★★ | ★★ | ★★★★ | ★★★★★ | ★ | ★★ | Encaisse et protège |
| **Florian** | ADC (Zeri) | ★★★ | ★★ | ★★★★★ | ★★ | ★★ | ★★★★ | Dégâts constants |
| **Yanis** | Contrôle (Lilia) | ★★★★ | ★★★ | ★★★★ | ★★★ | ★★★★ | ★ | **Vitesse la plus basse du jeu**, gros coup retardé |
| **Alex** | Bruiser (Lee Sin) | ★★★★ | ★★★ | ★★★★ | ★★★ | ★★ | ★★★★ | Polyvalent |

### Fiches express (pour les dialogues et les animations)
| Héros | Look | Running gags | Phrase culte |
|---|---|---|---|
| **Jordan** | Le plus vieux (29 ans), tenue adulte « propre » | Il a connu les dinosaures ; son dos craque ; il est le « riche » (voiture, appart) : les marchands lui font payer +30 % ; il n'a jamais désinvité José | « J'ai jamais désinvité personne ! » |
| **José** | Explorateur stylé : chapeau, foulard, pinceau ; pantalon qui tombe pile sur les baskets | Archéologue ; « mec cool » ; drague et se prend un râteau à chaque chapitre (façon Pierre dans Pokémon) ; « Tu m'as désinvité » (Portugal) | « Je suis un mec cool. » |
| **Kevin** | Casque de cosmonaute, maillot | Génie de l'espace et cerveau brainrot ; ne veut pas jouer à LoL (sans le détester) ; trauma Düsseldorf 2023 | « Skibidi pour de vrai. » |
| **Bidou** | Métalleux : cheveux longs, veste en cuir, guitare électrique | Manque toujours d'air (pauses pour respirer) ; rageux et très susceptible | « C'est bon, j'ai compris. Je boude. » |
| **Robin** | Combinaison d'aviateur, galons | Aviateur à contrecœur, fait sa thèse sur l'IA ; « Vive la lutte » ; sa copine Emma | « Zingis. » |
| **Florian** | Campagnard : pantacourt, chemise à carreaux, casquette de tracteur | Ascenseur en classé ; rageux en jeu mais un amour ; « c'est pas ma faute » ; son tracteur | « C'était le jungler. » |
| **Yanis** | Sweat confortable, AirPods, sourire éclatant | Lent dans **ses gestes** (pas dans sa parole) ; toujours en retard ; rituel des AirPods ; sandwich interminable | « Salut les mecs ! » |
| **Alex** | Beau gosse parfait… en jogging et pantoufles chez lui | Trop beau et gêné qu'on le dise ; habite Toulouse et « ne veut pas nous voir » ; gros geek de Lee Sin ; sa copine Vaiana, gendarme | « Arrêtez, c'est gênant. » |

---

## 5. Compagnons, guides et personnages clés

| Personnage | Rôle de jeu | Notes |
|---|---|---|
| **Snow** | Compagnon non combattant (suit Jordan sur la carte) | Gros chat blanc. **Pète** (nuage vert, « Ah, ça pue »). Intervient dans certains combats scriptés. Refuse parfois d'avancer. Légende locale du ch. 1 : « la Bête Blanche ». |
| **Clyde** | Guide non combattant (ch. 1 → fin) | Petit robot bleu rond, ancien bot officiel de Discord à la retraite. Explique le monde, sert d'interprète au ch. 4, bannit Camil au final. |
| **Le Modérateur Fou** | Antagoniste (voix des annonces) | Bot tyran. Ses annonces s'affichent dans le ciel en fin de chapitre, signées « Approuvé par Camil (1,62 m) ». |
| **Camil** | Antagoniste (hologrammes, boss B09) | Ego démesuré, **très petit** (1,62 m) : statues minuscules sur socles immenses, monte sur une caisse « NE PAS ENLEVER ». Banni et condamné à la vaisselle éternelle. **Aucune réconciliation.** |
| **Ceyn** | Antagoniste caché (boss final B10) | Ancien fondateur. Coupe mulet, maillot Karmine Corp, pantalon sans rapport avec des chaînes, appareil photo. N'apparaît **que comme un nom écrit** jusqu'au final. |
| **Emma** | Caméo (ch. 4 radio, interlude) | Copine de Robin depuis très longtemps. Bienveillante (« T'as mangé ? »). |
| **Vaiana** | Caméo (ch. 7 boss, interlude) | Copine d'Alex, gendarme, calme, carnet d'amendes. |

---

## 6. Compétences

> Coûts en points de Magie (Souffle pour Bidou). Puissance : **faible / moyenne / forte / très forte**. Niveau = niveau d'apprentissage.
> Chaque héros a aussi **Attaque** et **Défense** standards.

### Jordan (classe *L'Ancien*)
| ID | Nom | Type | Cible | Coût | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK001 | Tir de l'Ancien | Dégâts | 1 ennemi | 4 | Moyenne | 1 |
| SK002 | Brume Ancestrale | Soin | Équipe | 10 | Soin moyen | 1 |
| SK003 | Souvenirs du Crétacé | Debuff | 1 ennemi | 6 | Défense −25 % (3 tours). Réplique : « J'ai déjà vu ça en 1998. » | 3 |
| SK004 | Tournée Générale | Buff | Équipe | 12 | Attaque +25 % (3 tours) | 10 |

### José (*L'Archéologue Stylé*)
| ID | Nom | Type | Cible | Coût | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK010 | Coup de Pinceau | Dégâts | 1 ennemi | 3 | Moyenne | 1 |
| SK011 | Sprint Néon | Dégâts | 1 ennemi | 5 | Moyenne, **priorité** (agit en premier) | 1 |
| SK012 | Tombé de Pantalon Parfait | Buff | Soi | 4 | Défense +50 % (3 tours). « Je suis un mec cool. » | 4 |
| SK013 | Éboulement de Fouilles | Dégâts | Tous les ennemis | 10 | Moyenne | 9 |

### Kevin (*L'Ingénieur Orbital*)
| ID | Nom | Type | Cible | Coût | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK020 | Aerial | Dégâts | 1 ennemi | 6 | Forte, ×1,5 contre les ennemis volants | 8 |
| SK021 | Démolition | Dégâts | Tous les ennemis | 12 | Moyenne | 8 |
| SK022 | Calcul de Trajectoire | Buff | 1 allié | 6 | Précision et taux critique +50 % (2 tours) | 8 |
| SK023 | Boost | Buff | Équipe | 10 | Vitesse +30 % (3 tours) | 12 |

### Bidou (*Le Métalleux Cosmique*, joue Bard)
| ID | Nom | Type | Cible | Coût (Souffle) | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK030 | Riff Saturé | Dégâts | 1 ennemi | 4 | Moyenne | 11 |
| SK031 | Headbang | Dégâts | Tous les ennemis | 8 | Moyenne | 11 |
| SK032 | Carillons | Soin | Équipe | 8 | Soin moyen (clin d'œil aux carillons de Bard) | 11 |
| SK033 | Destin Figé | Statut | Tous les ennemis | 14 | *Étourdi* 1 tour (60 %) (la ult de Bard) | 13 |
> Animation : quand le Souffle est vide, Bidou est plié en deux, mains sur les genoux.

### Robin (*L'Aviateur Malgré Lui*, main Garen)
| ID | Nom | Type | Cible | Coût | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK040 | JUSTICE DÉMACIENNE | Dégâts | 1 ennemi | 10 | Très forte | 14 |
| SK041 | Frappe Aérienne | Dégâts | Tous les ennemis | 10 | Moyenne | 14 |
| SK042 | Grève Générale | Statut | Tous les ennemis | 12 | *Étourdi* 1 tour (40 %, 80 % contre les « sbires ») | 14 |
| SK043 | Plan de Vol | Buff | Équipe | 8 | Défense +30 % (3 tours) | 16 |

### Florian (*Le Tireur Campagnard*, Zeri)
| ID | Nom | Type | Cible | Coût | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK050 | Rafale Électrique | Dégâts | 1 ennemi | 5 | Forte | 17 |
| SK051 | Tir de Tracteur | Dégâts | Tous les ennemis | 10 | Moyenne | 17 |
| SK052 | Rage de Tilt | Buff | Soi | 4 | Attaque +50 %, Défense −20 % (3 tours). « ET TOI LE ZED… » | 17 |
| SK053 | Câlin | Soin | 1 allié | 6 | Soin fort (c'est un amour) | 18 |

### Yanis (*Le Faon Lent*, Lilia)
| ID | Nom | Type | Cible | Coût | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK060 | Coup de Fleur | Dégâts | 1 ennemi | 4 | Moyenne | 20 |
| SK061 | Sieste de Lilia | Statut | Tous les ennemis | 12 | *Sommeil* (50 %) | 20 |
| SK062 | Sourire Éclatant | Soin + statut | Équipe + 1 ennemi | 12 | Soin moyen de l'équipe, *Aveugle* sur 1 ennemi | 20 |
| SK063 | J'arrive… | Dégâts | 1 ennemi | 14 | Très forte (compense sa lenteur) | 21 |

### Alex (*Le Moine Trop Beau*, Lee Sin)
| ID | Nom | Type | Cible | Coût | Effet | Niv. |
|---|---|---|---|---|---|---|
| SK070 | Coup Résonnant | Dégâts | 1 ennemi | 4 | Moyenne | 23 |
| SK071 | Insec | Dégâts + debuff | 1 ennemi | 10 | Forte, Défense −25 % (3 tours) | 23 |
| SK072 | Beauté Aveuglante | Statut | Tous les ennemis | 10 | *Aveugle* (60 %) | 23 |
| SK073 | Rempart | Buff | 1 allié | 6 | Défense +50 % (3 tours) | 23 |

> **Niveaux de recrutement** : chaque recrue rejoint au niveau de l'équipe ; ses compétences de base sont déjà apprises.

---

## 7. États (statuts)

| ID | Nom | Effet | Durée | Soigné par |
|---|---|---|---|---|
| ST01 | Poison | Perd 5 % PV max par tour | 5 tours / fin de combat | Bain de Bouche, Carillons |
| ST02 | Sommeil | Ne peut pas agir ; réveillé par un coup | 1 à 3 tours | Café Serré, coup reçu |
| ST03 | Muet | Ne peut pas utiliser de compétences | 2 à 3 tours | Pastille pour la Gorge, Bonbonne d'Air |
| ST04 | Paralysie | Ne peut pas agir | 1 tour | Fin du tour |
| ST05 | Aveugle | Précision −50 % | 3 tours | Collyre |
| ST06 | Confusion | Attaque une cible au hasard | 2 tours | Coup reçu (25 %) |
| ST07 | Étourdi | Perd son prochain tour | 1 tour | Fin du tour |
| ST08 | Brûlure | Perd 3 % PV par tour, Attaque −10 % | 3 tours | Bain de Bouche |
| ST09 | Banni | Ne peut pas agir, sprite grisé (« VOUS N'ÊTES PLUS INVITÉ ») | 2 tours | Fin du statut uniquement |
| ST10 | Vexé (positif) | Attaque +30 % | Fin du combat | — (Bidou, scripté) |
| ST11 | Tilt (mixte) | Attaque +40 %, Défense −30 % | Scripté | Scripté (ch. 5) |
| ST12 | Gueule de bois | Vitesse −20 % | 2 tours | Café Serré |

---

## 8. Objets

### Consommables
| ID | Nom | Effet | Prix | Où |
|---|---|---|---|---|
| I001 | Chips | Soin 50 PV | 10 | Toutes les boutiques |
| I002 | Canette | Rend 15 Magie/Souffle | 20 | Toutes les boutiques |
| I003 | Hot-dog en Apesanteur | Soin 150 PV | 30 | Stade Orbital (buvette) |
| I004 | Pastille pour la Gorge | Soigne *Muet* | 25 | Cimes (Guide), Base |
| I005 | Bain de Bouche | Soigne *Poison* et *Brûlure* | 25 | Toutes |
| I006 | Collyre | Soigne *Aveugle* | 25 | Toutes |
| I007 | Café Serré | Soigne *Sommeil* et *Gueule de bois*, Vitesse +20 % (3 tours) | 40 | Marais, Toulouse |
| I008 | Bière Tiède de la Campagne | Soin 300 PV, 20 % de chance de *Confusion* | 35 | Enfers (après Florian) |
| I009 | Miel de la Ruche | Soin 500 PV | 80 | Stade (après le boss), Barbecue |
| I010 | Bonbonne d'Air | Soigne *Muet* de l'équipe, Souffle de Bidou au max | 60 | Cimes (après le boss) |
| I011 | Sandwich de Yanis (entamé) | Soin complet d'un allié | Non vendu (3 dans le jeu) | Coffres du Marais |
| I012 | Croquettes Spatiales | Objet de quête pour Snow (ne fait rien en combat) | 15 | Stade, Cimes |

> **Prix « Jordan »** : la plupart des marchands affichent les prix +30 % (« Vous avez une voiture »). Dans RPG Maker, utiliser un multiplicateur de prix global (plugin) ou des listes de prix gonflées. Exception : l'Abeille Marchande au Barbecue (« prix normal, cette fois »).

### Objets clés
| ID | Nom | Obtenu | Utilisé |
|---|---|---|---|
| K001 à K007 | Fragment du Premier Message (1/7 à 7/7) | Fin de chaque chapitre (le 7ᵉ donné par Alex) | Fusionnent en K008 |
| K008 | Premier Message de la Red Room | Fin du ch. 7 | Ouvre la Tour (F-1) |
| K010 | Cloche Barrée ×3 | Crypte (2 coffres, 1 sbire) | Socles de la Crypte (1-5-b) |
| K020 | Poster KC ×5 | Stade | Supporters mutés (2-3) |
| K021 | Écharpe de Kevin | Vestiaire | Chef du Kop (2-6) |
| K022 | Photo de Düsseldorf | Vestiaire | Montrée à Kevin (2-7) |
| K023 | Miel Royal | Ruche des Gradins | Échangé contre K024 |
| K024 | Billet Düsseldorf 2023 | Abeille Marchande | Chef du Kop (2-6) |
| K040 | Uniformes ×4 | Laverie de la Base | Passer la barrière (4-2) |
| K080 | Plaque à Frites Vide | Barbecue | Aucune (souvenir) |

### Objets de combat scriptés (donnés par les interventions, non achetables)
| Nom | Combat | Effet |
|---|---|---|
| Bonbonne d'Air Dorée | B03 Grand Mute | Retire *Muet* à l'équipe, Souffle de Bidou au max |
| Panier Repas d'Emma | B04 Adjudant | Soin complet de l'équipe, Robin Attaque/Défense +30 % |
| Café Serré d'Alex | B06 Sablier | Retire *Sommeil*, Vitesse +20 % pour l'équipe |

---

## 9. Équipements

> Chaque héros a 4 emplacements : Arme, Armure, Couvre-chef, Accessoire. Les équipements de récompense de chapitre sont uniques.

| ID | Nom | Type | Héros | Bonus | Obtenu |
|---|---|---|---|---|---|
| E001 | Canon-Relique Rouillé | Arme | Jordan | Atk +5, Mag +5 | Départ |
| E002 | Pinceau d'Archéologue | Arme | José | Atk +6 | Départ (ch. 1) |
| E003 | Chapeau d'Explorateur | Couvre-chef | José | Déf +3, Vit +2 | Départ (ch. 1) |
| E004 | Clé à Molette Orbitale | Arme | Kevin | Atk +12 | Ch. 2 |
| E005 | Maillot de la Demi-Finale | Armure | Kevin | Déf +15. « Encore un peu humide de larmes. » | Fin du ch. 2 |
| E010 | Médiator de Bard | Arme | Bidou | Mag +15. Fait « meep » | Fin du ch. 3 |
| E011 | Veste en Cuir Cloutée | Armure | Bidou | Déf +12 | Ch. 3 (coffre) |
| E020 | Épée Démacienne Trop Grande | Arme | Robin | Atk +18 | Ch. 4 |
| E021 | Galons de Sergent | Accessoire | Robin | Déf +10. « Envie d'être là −50 » | Fin du ch. 4 |
| E030 | Lance-Éclairs de Campagne | Arme | Florian | Atk +20 | Ch. 5 |
| E031 | Pantacourt Légendaire | Armure | Florian | Déf +18, résistance *Brûlure* | Fin du ch. 5 |
| E040 | Bâton Fleuri | Arme | Yanis | Atk +18, Mag +10 | Ch. 6 |
| E041 | AirPods de Yanis | Accessoire | Yanis | Immunité *Sommeil* | Fin du ch. 6 |
| E050 | Bandeau du Moine | Couvre-chef | Alex | Atk +8, Vit +5 | Ch. 7 |
| E051 | Pantoufles de Gamer | Accessoire | Alex | Vit +10 | Fin du ch. 7 |
| E060 | Tablier de Barbecue | Armure | Jordan | Déf +20 | Barbecue |
| E061 | Écharpe KC | Accessoire | Tous | Résistance *Muet* | Boutique de Généralia (après ch. 2) |

> Compléter avec des équipements génériques par palier (Armure de Mod niv. 1/2/3, etc.) dans les boutiques de Généralia et de Toulouse.

---

## 10. Ennemis communs

| ID | Nom | Zone | Niv. | Attaques | Note |
|---|---|---|---|---|---|
| EN001 | Spam-bot | Généralia, Crypte | 2 | Mono faible ×2 | « CLIQUEZ ICI POUR GAGNER » |
| EN002 | Notification Fantôme | Crypte | 3 | « 99+ mentions » : *Confusion* | |
| EN003 | Réaction Abandonnée 👍 | Crypte | 2 | Mono faible | Fuit souvent |
| EN004 | Sbire du Modérateur 🔨 | Partout | 3 à 15 | « Avertissement » : *Muet* | Faible à Grève Générale |
| EN010 | Abeille Ouvrière | Ruche | 7 | Mono faible | Volante |
| EN011 | Frelon Ultra | Ruche | 8 | Mono + *Poison* | Volant |
| EN012 | Chambreur Jaune | Ruche, Stade | 8 | Debuff attaque (« T'as perdu en 2023 ! ») | |
| EN013 | Abeille Videur | Vestiaire | 9 | Mono forte | Combat obligatoire |
| EN020 | Micro Coupé | Cimes | 10 | *Muet* | |
| EN021 | Larsen Sauvage | Cimes | 10 | Zone faible | |
| EN022 | Bouchon d'Oreille | Cimes | 11 | Debuff attaque | |
| EN030 | Avion de Papier | Base | 13 | Mono, rapide | Volant |
| EN031 | Haut-Parleur | Base | 13 | Zone + *Confusion* (« ANNONCE IMPORTANTE ! ») | |
| EN040 | Âme Toxique | Enfers | 16 | Debuff attaque (« t'es nul ») | |
| EN041 | Inter | Enfers | 16 | Mono forte, défense très faible | |
| EN042 | AFK Errant | Enfers | 16 | Ne fait rien 2 tours, puis frappe fort | |
| EN043 | Flamme du Chat | Enfers | 17 | Zone + *Brûlure* | |
| EN050 | Moustique Insomniaque | Marais | 19 | Mono, rapide | Volant |
| EN051 | Dormeur Somnambule | Marais | 19 | Zone + *Sommeil* | |
| EN052 | Notif « Êtes-vous toujours là ? » | Marais | 20 | Debuff vitesse | |
| EN060 | Ward de Contrôle | Toulouse | 22 | Debuff précision | Apparaît si erreur au combo |
| EN061 | Paquet Perdu | Route, Toulouse | 22 | Mono, rate souvent | |
| EN070 | Reflet Vaniteux | Tour | 25 | Mono + buff défense sur lui | Apparaît si erreur aux miroirs |
| EN071 | Statue Minuscule | Tour (invoquée par Camil) | 26 | Aucune attaque, buff défense à Camil | Add du boss |

---

## 11. Boss

> Valeurs indicatives (échelle RPG Maker MZ). Les **interventions** sont des événements de troupe : condition, puis messages, puis effets (ajouter/retirer un état, soin, dégâts).

### B01 — Gardien des Épinglés (ch. 1, scène 1-6)
| | |
|---|---|
| PV | 600 |
| Phases | P1 (100 à 60 %) · P2 (60 à 25 %) · P3 (< 25 %) |
| P1 | Coup d'Épingle (mono), Épinglage (*Paralysie*), Rappel à l'ordre (*Muet*) |
| P2 | + Retrait d'Invitation : *Banni* sur **José** (2 tours) |
| P3 | + Suppression (zone forte) |
| Interventions | **PV ≤ 60 %** : message « VOUS N'ÊTES PLUS INVITÉ », José banni ; à la fin de l'état, José gagne Attaque +30 % (réplique « Personne. Ne. Me. Désinvite. ») · **PV ≤ 25 %** : CE02 (pet de Snow), boss Défense −30 % jusqu'à la fin |
| Récompense | K001, 150 XP, 100 pièces |

### B02 — Reine de la Ruche (ch. 2, scène 2-8)
| | |
|---|---|
| PV | 1 500 |
| Faiblesse | Aerial (volant) |
| P1 | Dard Jaune (mono), Essaim (zone faible), Chambrage (debuff attaque). Tous les 3 tours : invoque 2 Abeilles Supportrices (adds, soignent la Reine) |
| P2 (≤ 50 %) | + Miel Royal (soin 15 %, une fois), Pluie de Dards (zone + *Poison*) |
| Interventions | **PV ≤ 50 %** : le Kop Rouge chante « KC ! KC ! » → équipe Attaque +20 % jusqu'à la fin · Premier Aerial en P2 : réplique de Kevin |
| Récompense | K002, E005, 400 XP |

### B03 — Le Grand Mute (ch. 3, scène 3-6)
| | |
|---|---|
| PV | 2 500 |
| P1 | Coupure de Micro (*Muet*), Larsen (zone), Silence Pesant (debuff attaque équipe) |
| P2 (≤ 50 %) | + Mute Général (*Muet* équipe, 2 tours), Écrasement (mono fort) |
| Interventions | **Tour 3** : hologramme de Camil → boss Défense +30 %, Bidou état *Vexé* (Attaque +30 %) · **Premier Mute Général** : Sbire déserteur → Bonbonne d'Air Dorée (retire *Muet*, Souffle max) |
| Récompense | K003, E010, 700 XP |

### B04 — L'Adjudant @everyone (ch. 4, scène 4-6)
| | |
|---|---|
| PV | 3 500 |
| P1 | Annonce Générale (zone), @everyone (*Confusion*), Garde-à-vous ! (*Paralysie*) |
| P2 (≤ 50 %) | + Volume Maximum (buff attaque), Rappel du Règlement (zone forte), Corvée de Chiottes (debuff défense) |
| Interventions | **Tour 2** : Renforts → les sbires font grève, l'invocation échoue (et échoue à chaque fois ensuite) · **PV ≤ 50 %** : Emma à la radio → Panier Repas (soin complet équipe, Robin Atk/Déf +30 %) |
| Récompense | K004, E021, 1 000 XP |

### B05 — Le Juge du Matchmaking (ch. 5, scène 5-4)
| | |
|---|---|
| PV | 4 500 |
| P1 | Verdict (mono fort), MMR Caché (debuff défense équipe), Mauvaise Équipe (*Confusion*) |
| P2 (≤ 50 %) | + Série de Défaites (zone forte), Dodge (esquive + soin 10 %) |
| Interventions | **Tour 3** : chat toxique → Florian état *Tilt* ; puis messages de soutien de l'équipe → le malus de défense de Florian disparaît, le bonus reste · **PV ≤ 50 %** : le tracteur casse la balance → le Juge perd MMR Caché, Défense −30 % |
| Récompense | K005, E031, 1 400 XP |

### B06 — Le Sablier d'Inactivité (ch. 6, scène 6-4)
| | |
|---|---|
| PV | 5 500 |
| P1 | Sable du Sommeil (*Sommeil*), Avertissement d'Inactivité (debuff vitesse équipe), Coup de Sablier (mono) |
| P2 (≤ 50 %) | + Temps Inversé (soin 15 %, une fois), Kick Imminent (zone forte), Sommeil Profond (*Sommeil* sur 2 alliés) |
| Interventions | **Avant le premier tour de Yanis** : rituel des AirPods + sourire → boss *Aveugle* (P1) · **PV ≤ 50 %** : message d'Alex + colis → Café Serré d'Alex (retire *Sommeil*, Vitesse +20 %) |
| Récompense | K006, E041, 1 800 XP |

### B07 — Le Démon du Lag (ch. 7, scène 7-5)
| | |
|---|---|
| PV | 6 500 |
| P1 | Paquet Perdu (debuff précision), Freeze (*Paralysie*), Pic de Latence (mono fort) |
| P2 (≤ 50 %) | + Déconnexion (zone forte), Rollback (soin 15 %, une fois) |
| Interventions | **Tour 3** : Vaiana (gendarme) met une amende → boss Atk et Déf −25 % · **PV ≤ 50 %** : le fan club et l'équipe crient « T'ES TROP BEAU » → boss *Aveugle*, Vitesse −30 % |
| Récompense | K007 (donné par Alex avant), E051, 2 200 XP |

### B08 — Golem de Vaisselle Sale (Final, scène F-3)
| | |
|---|---|
| PV | 3 000 (mini-boss) |
| Attaques | Assiette Volante (mono), Éclaboussure (zone + *Poison*) |
| Note | « Faible contre tout » : défense basse, pas de phase |

### B09 — Camil (Final, scène F-4)
| | |
|---|---|
| PV | 8 000 |
| Contrainte | **Kevin interdit** |
| P1 | Monologue Interminable (*Sommeil*), Ego Surdimensionné (buff défense), Désinvitation (*Banni* 2 tours) |
| P2 (≤ 50 %) | + Point de Vue Supérieur (buff attaque, il monte sur sa caisse), Coup de Talonnette (mono fort), Statue Minuscule (invoque EN071) |
| Interventions | Si Désinvitation touche José : réplique « C'était LUI, le vrai désinviteur ! » · **Tour 3** : personne ne vient à son secours → Camil Atk −30 % · **PV ≤ 50 %** : CE02 (pet de Snow) → Camil tombe de sa caisse, perd son buff d'attaque, Déf −30 % |
| Fin | Cinématique : fils de marionnette, bannissement par Clyde, condamné à la vaisselle |

### B10 — Ceyn, le Modérateur Suprême (boss final, scène F-6)
| | |
|---|---|
| PV | 15 000 |
| P1 « Le Shooting » (100 à 60 %) | Flash (*Aveugle*), Pose de Trois Quarts (esquive +50 %), Chaîne de Pantalon (mono + *Paralysie*) |
| P2 « La Fusion » (60 à 25 %) | Ban Hammer (zone forte), Mute Général (*Muet* équipe, 2 tours), Kick (mono très fort). Dialogues en majuscules |
| P3 « Le Dernier Mot » (< 25 %) | + Signature (zone très forte, son nom en graffiti géant) |
| Interventions | **PV ≤ 60 %** : le Kop Rouge chante « KC ! KC ! » → Ceyn chante avec eux, *Étourdi* 1 tour, perd l'esquive · **Premier Mute Général** : chaque héros **en réserve** intervient avec son effet (table ci-dessous), puis CE02 (Snow) → Ceyn Déf −30 % · **PV = 0** : CE01 version finale (« CEYN. » en chœur), puis cinématique |

**Effets des héros en réserve (B10, intervention 2)**
| Héros | Réplique | Effet |
|---|---|---|
| Bidou | « J'ai gardé une Bonbonne d'Air ! » | Retire *Muet* à l'équipe |
| Yanis | *(AirPod, sourire)* | Ceyn *Aveugle* |
| Alex | « Rempart sur Jordan ! » | Équipe Déf +30 % |
| Florian | « Michel, VAS-Y ! » | Dégâts fixes 800 sur Ceyn |
| Robin | « Les sbires, avec moi ! » | Ceyn Atk −25 % |
| José | « Je suis un mec cool. » | Aucun effet (gag) |
| Kevin | « Calcul de trajectoire : terminé. » | Équipe critique +30 % |
> Jordan est toujours dans l'équipe active ; seuls les 4 héros en réserve interviennent.

---

## 12. Cartes

> Taille indicative en tuiles (RPG Maker : 48 px). Tileset suggéré entre crochets.

### Prologue et Chapitre 1
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M00 | QG de Jordan | Intérieur, cinématique | 15×12 | PC, Switch, canettes, litière, Snow | BGM_QG_Lofi |
| M01 | Généralia (#général) | Ville-hub | 40×35 [ville + décor « messages gravés »] | Place Camil (socle géant + statue minuscule), boutique, auberge, Mur des Mutés, mur de graffitis (Ceyn), fontaine 💀 | BGM_Generalia |
| M02 | Chantier de fouilles | Extérieur | 20×20 | Tranchée en strates, porte de la Crypte | BGM_Generalia |
| M03 | Crypte des Messages Épinglés | Donjon (4 salles) | 4 × 20×15 | Salle des Strates (fresques), salles des Cloches (2 coffres, 1 sbire), Porte des Fondateurs (mot de passe), antichambre (Snow) | BGM_Crypte |
| M04 | Salle du Gardien | Boss | 17×13 | Vitrine du Premier Message | BGM_Boss_1 |

### Chapitre 2
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M10 | Portail #rocket-league | Transition | 10×10 | But géant, cinématique voiture | — |
| M11 | Stade Orbital | Hub de zone | 35×30 [sci-fi + stade] | Tribunes jaunes, Kop Rouge, buvette, kiosque, 5 posters, stand LoL | BGM_Stade |
| M12 | Vestiaire | Intérieur | 15×12 | Casier de Kevin, banc (Ceyn), combat obligatoire | BGM_Stade |
| M13 | Ruche des Gradins | Mini-donjon (3 salles) | 3 × 15×15 | Alvéoles, Commentatrice, coffre du Miel Royal | BGM_Ruche |
| M14 | Terrain | Boss | 25×17 | Boucle, puis boss | BGM_Boss_2 |

### Chapitre 3
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M20 | Pied de la montagne | Extérieur | 25×30 [montagne enneigée] | Panneau « RESPIRATION INTERDITE » | BGM_Cimes |
| M21 | Lac Gelé | Énigme | 20×20 | Glace + rochers (énigme), rocher « Ceyn » | BGM_Cimes |
| M22 | Passage du Yéti | Extérieur | 15×20 | Yéti Roadie (quiz), Fan de Metal, Guide de Montagne (boutique) | BGM_Cimes |
| M23 | Sommet | Boss | 20×15 | Scène en rochers, ampli, 🔇 géant | BGM_Boss_3 |

### Chapitre 4
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M30 | Entrée de la Base | Extérieur | 25×20 [militaire] | Barrière, gardes | BGM_Base_Kazoo |
| M31 | Laverie | Intérieur | 12×10 | Machine à laver géante, combat | BGM_Base_Kazoo |
| M32 | Hangar | Intérieur | 20×15 | Robin, photo d'Emma, ordinateur (Ceyn en bibliographie) | BGM_Base_Calme |
| M33 | Tour de Contrôle | Énigme | 12×12 | 6 interrupteurs, vue sur la piste, Pilote | BGM_Base_Kazoo |
| M34 | Cour et piste | Boss | 30×20 | Discours, puis boss | BGM_Boss_4 |

### Chapitre 5
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M40 | Porte des Enfers | Transition | 15×15 | Inscription, Cerbère à trois têtes | BGM_Enfers |
| M41 | Caverne de Fer | Donjon | 30×25 [lave, roche] | Âmes damnées, Âme Damnée (drague) | BGM_Enfers |
| M42 | Pente de Sisyphe | Énigme | 20×30 | Grille de blocs, 3 dalles VICTOIRE, dalles DÉFAITE | BGM_Enfers |
| M43 | Tribunal | Boss | 20×17 | Balance, trône | BGM_Boss_5 |

### Chapitre 6
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M50 | Lisière du Marais | Extérieur | 25×25 [marais, brume] | Dormeurs, panneau AFK | BGM_Marais |
| M51 | Labyrinthe de Brume | Énigme | 35×35 | Planches, miettes, culs-de-sac, saule (Ceyn), Fée | BGM_Marais |
| M52 | Clairière de Yanis | Boss | 15×15 | Banc, puis boss | BGM_Boss_6 |

### Chapitre 7
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M60 | Route du Ping | Cinématique / courte route | 40×10 | Panneaux ping 50/150/300, voiture | BGM_RoadTrip |
| M61 | Toulouse — Place du Capitole | Ville | 35×30 [ville rose] | Affiches d'Alex, statue, PNJ toulousains, Toulousaine, plaque « Allée Ceyn », boutique | BGM_Toulouse |
| M62 | Ruelle d'Alex | Énigme | 15×15 | Dalles Q W E R, tags-indices | BGM_Toulouse |
| M63 | Chambre d'Alex | Intérieur | 12×10 | Écrans, figurines | BGM_Toulouse_Calme |
| M64 | Capitole de nuit | Boss | 25×17 | Sol fendu | BGM_Boss_7 |

### Interlude et Final
| ID | Nom | Type | Taille | Contenu | BGM |
|---|---|---|---|---|---|
| M70 | Jardin de Camil | Hub (sauvegarde, boutique, équipe) | 25×20 | Barbecue, table, drap pour le PowerPoint, invités | BGM_Barbecue |
| M80 | Porte de la Tour | Transition | 15×15 | 7 encoches | BGM_Tour |
| M81 | Galerie de l'Ego | Énigme | 25×12 | Portraits, miroirs-interrupteurs | BGM_Tour |
| M82 | Salon des Invités | Mini-boss | 20×15 | Table vide, pile de vaisselle | BGM_Boss_Mini |
| M83 | Salle du Trône | Boss | 20×20 | Trône sur 20 marches, caisse, rideau | BGM_Boss_Camil |
| M84 | Console / Défilé | Boss final | 25×20 | Console, puis podium de défilé | BGM_Boss_Final |
| M90 | QG (épilogue) | Cinématique | = M00 | | BGM_QG_Fin |
| M91 | Cuisine éternelle | Post-générique | 12×10 | Évier, vaisselle, Camil | BGM_Vaisselle |

---

## 13. PNJ

> PNJ simples : un sprite générique suffit sauf mention. Les répliques complètes sont dans le script.

### Généralia (M01–M02)
| ID | Nom | Rôle | Réplique type |
|---|---|---|---|
| N001 | Mme Nitro-Pas-Chère | Marchande (tutoriel boutique, prix +30 %) | « Inflation, monsieur. C'est la faute du Modérateur. » |
| N002 | Citoyen Muté | Ambiance | « 😶 👉 🔨 🤖 😭 » |
| N003 | Vieux Bot de Musique | Ambiance (revient au Barbecue) | « Avant on passait de la musique dans les vocaux… » |
| N004 | Enfant de Généralia | Ambiance | « C'est vrai que vous avez connu les dinosaures ? » |
| N005 | Aubergiste du #général | Auberge (soin et sauvegarde) | « Une nuit, 20 pièces. Pour vous, 26. » |
| N006 | Nitro | Drague de José (ch. 1) | « Je coûte 9,99 € par mois. » |
| N007 | Garde Muté | Bloque les sorties avant la fin du ch. 1 | « 🔇 ✋ » |

### Stade Orbital (M11–M14)
| ID | Nom | Rôle |
|---|---|---|
| N010 à N014 | Supporters mutés ×5 | Reçoivent les posters |
| N015 | Abeille Marchande | Buvette, échange Miel Royal / Billet (revient au Barbecue) |
| N016 | Chef du Kop | Reçoit les 3 objets, lance le chant |
| N017 | Commentatrice (fan de Vitality) | Drague de José (ch. 2), revient au Barbecue |
| N018 | Vendeur du stand LoL | Gag de Kevin à la sortie |
| N019 | Abeille Supportrice (ambiance) | « On commence à s'ennuyer, à gagner tout le temps. » |

### Cimes (M20–M23)
| ID | Nom | Rôle |
|---|---|---|
| N020 | Yéti Roadie | Quiz (revient au Barbecue) |
| N021 | Fan de Metal | Drague de José (ch. 3) |
| N022 | Guide de Montagne | Boutique (Pastilles, Croquettes) |

### Base (M30–M34)
| ID | Nom | Rôle |
|---|---|---|
| N030 | Sbires de garde ×2 | Barrière (uniforme obligatoire) |
| N031 | Pilote de Chasse | Drague de José (ch. 4) |
| N032 | Sbire timide | « C'est vrai qu'on a jamais de tickets resto… » |
| N033 | Foule de sbires | Discours (sprites répétés) |

### Enfers (M40–M43)
| ID | Nom | Rôle |
|---|---|---|
| N040 | Cerbère du Classé (3 têtes) | Gag d'entrée (sprite unique) |
| N041 | Âmes damnées | Ambiance (« ff 15 », « c'était gagné ») |
| N042 | Âme Damnée aux cheveux noirs | Drague de José (ch. 5) |
| N043 | Démon-marchand | Boutique (Bière Tiède, Bain de Bouche) |

### Marais (M50–M52)
| ID | Nom | Rôle |
|---|---|---|
| N050 | Dormeurs ×N | Ambiance, se réveillent après le boss |
| N051 | Fée des Lucioles | Drague de José (ch. 6) |
| N052 | Grenouille-marchande | Boutique (Café Serré) |

### Toulouse (M61–M64)
| ID | Nom | Rôle |
|---|---|---|
| N060 | Mamie sur un banc | Ambiance (revient au boss et au Barbecue) |
| N061 | Serveur de terrasse | Ambiance |
| N062 | Enfant toulousain | Ambiance |
| N063 | Fan club d'Alex ×5 | Ambiance + intervention boss |
| N064 | Toulousaine | Drague de José (ch. 7) |
| N065 | Marchande de violettes | Boutique |

### Personnages caméo (sprites uniques)
| ID | Nom | Où |
|---|---|---|
| N090 | Emma | Ch. 4 (voix radio, photo), Barbecue |
| N091 | Vaiana | Ch. 7 (boss), Barbecue |
| N092 | Camil | Hologrammes (ch. 1, 3), boss, post-générique |
| N093 | Ceyn | Final uniquement |
| N094 | Clyde | Ch. 1 → fin |

---

## 14. Énigmes

| ID | Chapitre | Type | Description | Solution | Échec | Aide |
|---|---|---|---|---|---|---|
| P01 | 1 | Objets | 3 Cloches Barrées à poser sur 3 socles | 2 coffres + 1 sbire | — | Clyde |
| P02 | 1 | Mot de passe | Porte des Fondateurs | `RED ROOM` | Message « Mot de passe incorrect » | José donne l'indice |
| P03 | 2 | Objets (quête) | 5 posters, écharpe, billet (via Miel Royal) | Ordre libre | — | Journal de quête |
| P04 | 3 | Glace | Glisser jusqu'à un rocher pour traverser le lac | Tracé à concevoir (6 à 8 mouvements) | Retour au départ | Réplique de Kevin |
| P05 | 3 | Quiz | 3 questions du Yéti | Bard / Du metal / La Red Room | Combat 2 Larsens, puis la question revient | — |
| P06 | 4 | Interrupteurs | 6 interrupteurs (chacun inverse sa rampe et 1 ou 2 voisines) pour écrire ZINGIS | Combinaison unique (à concevoir) | — | Kevin donne la solution après 3 essais |
| P07 | 4 | Dialogue | 3 bons slogans sur 6 | « Pas de ban sans pause café », « Le marteau c'est pour les clous », « Zingis pour tous » | La foule hue, on recommence | — |
| P08 | 5 | Blocs à pousser | Pousser le rocher LP sur 3 dalles VICTOIRE en évitant les dalles DÉFAITE | Grille à concevoir | Rocher en bas (« DÉFAITE. −25 LP ») | — |
| P09 | 6 | Labyrinthe | Suivre les miettes dans la brume (visibilité 2 cases) | Chemin des miettes | Cul-de-sac + combat | — |
| P10 | 7 | Dalles en séquence | Combo de l'insec | Q, Q, W, R | Alarme « FLASH RATÉ » + combat 2 Wards | Jordan donne la solution après 3 essais |
| P11 | I | Dialogue | Ordre des PowerPoint + vote | Libre | — | — |
| P12 | F | Miroirs (interrupteurs) | Tourner les miroirs pour afficher Camil à 1,62 m | Combinaison à concevoir | Combat 2 Reflets Vaniteux | — |

---

## 15. Événements communs (mécaniques récurrentes)

### CE01 — Gag « Ceyn. »
- **Déclencheur** : le joueur examine un objet portant le nom **Ceyn** (graffiti, banc, neige, bibliographie, classement, arbre, plaque de rue), ou scène scriptée.
- **Effet** : chaque membre **présent** de l'équipe dit « Ceyn. » dans une bulle, dans l'ordre de la formation (Bidou : « *(inspire)* Ceyn. »). Puis on rend la main, **sans autre commentaire**.
- **Règle absolue** : aucune musique, aucun zoom, aucun indice. Le joueur doit croire que c'est juste un gag.
- **Variante finale** (F-5) : après le chœur, l'équipe fait 3 pas, s'arrête, puis « … attends. ».
- **Variante boss** (B10) : les 8 le disent **ensemble**, en une seule bulle.
- Occurrences : M01 (mur), M12 (banc), M21 (neige), M32 (thèse), M42/M43 (classement), M51 (saule), M61 (plaque), F-5, F-6, F-7.

### CE02 — Pet de Snow
- **Effet** : animation de Snow qui se retourne, `SE_Prrrt`, nuage vert, puis bulle « Ah, ça pue. » au-dessus d'un ou plusieurs personnages.
- **Sur la carte** : chance faible à chaque déplacement, ou toutes les N minutes, bulle sur un membre au hasard.
- **En combat (scripté)** : l'ennemi ciblé reçoit Défense −30 %.

### CE03 — Drague de José
- **Effet** : `SE_JingleDrague` (composition originale façon « Pierre »), dialogue, `SE_JingleTriste`, `V001 += 1`.
- Une fois par chapitre (+ Barbecue). Succès « Pierre de Kanto » au générique.

### CE04 — Annonce du Modérateur
- **Effet** : `SE_Everyone`, tremblement d'écran, fenêtre de texte stylisée « #annonces · 🔨 Modérateur Fou (BOT) » en haut de l'écran.
- Toujours signée « — *Approuvé par Camil (1,62 m)* ».

### CE05 — Craquement de dos de Jordan
- **Effet** : `SE_Crac`, petite icône « −5 PV » (cosmétique, ne retire rien).
- Quand Jordan se relève dans une scène.

### CE06 — Rituel des AirPods de Yanis
- **Effet** : 6 étapes d'animation séparées par ~1,5 s (lever la main, retirer l'AirPod droit, le regarder, le ranger, *clic*, idem à gauche), puis `SE_Ting` et sourire.
- Le joueur n'a pas la main pendant la séquence. Doit durer **un peu trop longtemps**.

### CE07 — Respiration de Bidou
- Dans les dialogues, insérer « *(inspire)* » comme une pause courte (attente de 20 frames dans RPG Maker).

---

## 16. Switches et variables (flags)

### Switches
| ID | Nom | Mis à ON | Utilisé |
|---|---|---|---|
| S001 | snow_a_clique | P-3, si le joueur refuse de cliquer | 1-1 (réplique de Clyde) |
| S002 | jose_aveu_portugal | 1-3, choix 2 | Barbecue (réplique bonus de José) |
| S003 | quete_bete_blanche_active | 1-1 | Journal de quête |
| S004 | quete_bete_blanche_finie | 1-7 | Snow suit l'équipe |
| S010 | ch1_fini | 1-8 | Débloque #rocket-league, #vocal-1 |
| S011 | ch2_posters_finis | 2-3 (V003 = 5) | Quête Kop |
| S012 | ch2_echarpe | 2-4 | Quête Kop |
| S013 | ch2_billet | 2-5 | Quête Kop |
| S014 | ch2_kop_chante | 2-6 | Accès au terrain, intervention B02 |
| S020 | ch2_fini | 2-10 | Annonce #vocal-1 |
| S021 | bidou_vexe | 3-4, choix 2 | Réplique bonus |
| S022 | quiz_yeti_reussi | 3-3 | Ouvre le passage |
| S030 | ch3_fini | 3-7 | Débloque #annonces |
| S031 | uniformes | 4-2 | Ouvre la barrière, fin de « l'interdit de parler » |
| S032 | zingis_allume | 4-4 | Discours |
| S033 | discours_reussi | 4-5 | Recrue Robin, réserve activée |
| S040 | ch4_fini | 4-7 | Débloque #classé |
| S041 | promotion_reussie | 5-3 | Recrue Florian, porte du Tribunal |
| S050 | ch5_fini | 5-5 | Débloque #afk |
| S060 | ch6_fini | 6-5 | Débloque la Route du Ping |
| S061 | combo_reussi | 7-3 | Porte d'Alex |
| S070 | ch7_fini | 7-6 | Débloque le Jardin et la Tour |
| S080 | barbecue_fini | I-5 | Ouvre la Tour |
| S081 | miroirs_resolus | F-2 | Étage 2 |
| S090 | camil_battu | F-4 | Console |
| S091 | ceyn_revele | F-5 | Boss final |
| S099 | jeu_termine | F-7 | Générique, scène post-générique |

### Variables
| ID | Nom | Rôle |
|---|---|---|
| V001 | rateaux_jose | Compteur des râteaux (affiché au générique) |
| V002 | fragments | Nombre de fragments (0 à 7) |
| V003 | posters | Posters donnés (0 à 5) |
| V004 | cloches | Cloches posées (0 à 3) |
| V005 | quiz_score | Bonnes réponses au quiz |
| V006 | slogans_ok | Bons slogans choisis |
| V007 | essais_interrupteurs | Pour déclencher l'aide de Kevin |
| V008 | essais_combo | Pour déclencher l'aide de Jordan |
| V009 | vote_powerpoint | Gagnant du vote (1 à 8) |
| V010 | chapitre | Chapitre en cours (0 à 9), pour les dialogues de l'auberge et de Clyde |
| V011 | ceyn_vus | Nombre de gags « Ceyn. » déclenchés (pour une réplique de Ceyn au final, optionnelle) |

---

## 17. Cinématiques et scènes scriptées

| ID | Scène | Contenu | Contrôle joueur |
|---|---|---|---|
| C01 | P-1 à P-3 | Soirée vocale, le lien, l'aspiration | Choix (cliquer ou non) |
| C02 | 1-1 | Réveil, Clyde | Non |
| C03 | 1-3 | José, le bocal (« c'est un pet de Snow ») | Choix |
| C04 | 1-8 | Annonce + hologramme de Camil | Non |
| C05 | 2-2 | Kevin en boucle (match qui se rembobine) | Non |
| C06 | 2-7 | Kevin et la photo | Non |
| C07 | 3-4 et 3-5 | Bidou, le cri collectif | Choix |
| C08 | 4-1 | « Vous n'avez pas la permission… » | Non |
| C09 | 4-5 | Discours de grève | Choix (slogans) |
| C10 | 5-2 | Florian écrasé par son rocher | Non |
| C11 | 6-3 | Rituel des AirPods (CE06) | Non |
| C12 | 7-4 | Alex chez lui | Non |
| C13 | 7-6 | La Red Room au complet | Non |
| C14 | I-2 | Les frites | Non |
| C15 | I-4 et I-5 | Invités surprise, la nuit | Dialogues libres |
| C16 | F-4 fin | Fils de marionnette, bannissement de Camil | Non |
| C17 | F-5 | Révélation de Ceyn | Non |
| C18 | F-6 fin | « CEYN. » en chœur | Non |
| C19 | F-7 | Réveil au QG, épilogue | Non |
| C20 | Post-générique | Camil fait la vaisselle | Non |

---

## 18. Audio

### Musiques (BGM)
| ID | Usage | Ambiance |
|---|---|---|
| BGM_QG_Lofi | Prologue | Lo-fi chill avec le *bloop* Discord |
| BGM_Generalia | Ch. 1 | Thème de capitale RPG + *ping* de notification |
| BGM_Crypte | Ch. 1 donjon | Orgue mystérieux |
| BGM_Stade | Ch. 2 | Électro épique synthwave ; « disque rayé » pendant la boucle |
| BGM_Ruche | Ch. 2 donjon | Bourdonnements rythmés |
| BGM_Cimes | Ch. 3 | Riff saturé lointain, étouffé |
| BGM_Base_Kazoo | Ch. 4 | Marche militaire au kazoo |
| BGM_Base_Calme | Ch. 4 hangar | Piano doux |
| BGM_Enfers | Ch. 5 | Chœurs lugubres + *ding* de fin de partie |
| BGM_Marais | Ch. 6 | Berceuse lo-fi lente, bâillements |
| BGM_RoadTrip | Ch. 7 route | Rock FM |
| BGM_Toulouse | Ch. 7 | Guitare ensoleillée, accordéon |
| BGM_Barbecue | Interlude | Guitare acoustique, grillons |
| BGM_Tour | Final | Sombre, montée |
| BGM_Boss_1 à _7 | Boss de chapitre | Variations d'un thème de boss commun |
| BGM_Boss_Camil | Camil | Thème pompeux et ridicule (fanfare trop grande) |
| BGM_Boss_Final | Ceyn | Thème de défilé de mode électro, qui monte en épique |
| BGM_QG_Fin | Épilogue | Reprise douce du thème du QG |
| BGM_Vaisselle | Post-générique | Musique d'attente téléphonique |

### Sons (SE)
`SE_Bloop` (connexion) · `SE_BloopDown` (déconnexion) · `SE_Ding` (notification) · `SE_Everyone` (annonce) · `SE_Prrrt` (Snow) · `SE_Ting` (sourire de Yanis) · `SE_Crac` (dos de Jordan) · `SE_JingleDrague` / `SE_JingleTriste` (José) · `SE_Inspire` (Bidou) · `SE_Buzzer` (stade) · `SE_Rembobinage` · `SE_KC_Chant` (« KC ! KC ! ») · `SE_Sirene` (Vaiana) · `SE_Tracteur` · `SE_Defaite` (« DÉFAITE. −25 LP ») · `SE_Promotion` (fanfare) · `SE_FlashPhoto` (Ceyn) · `SE_BanHammer` · `SE_Clic` (boîtier AirPods).

---

## 19. Liste des assets graphiques

### Personnages (sprite de carte + visage pour les dialogues + battler)
- **Héros** : Jordan, José, Kevin, Bidou, Robin, Florian, Yanis, Alex.
- **Visages par héros** : neutre, content, énervé/vexé, triste, gêné (+ José « drague », Bidou « essoufflé », Yanis « sourire éclatant », Alex « rouge de gêne »).
- **Compagnons** : Snow (marche, assis, pet), Clyde.
- **Antagonistes** : Camil (normal, sur caisse, hologramme), Ceyn (poses de shooting ×3, version fusionnée).
- **Caméos** : Emma, Vaiana (uniforme de gendarme).

### Battlers de boss (grands formats)
Gardien des Épinglés · Reine de la Ruche · Grand Mute · Adjudant @everyone · Juge du Matchmaking · Sablier d'Inactivité · Démon du Lag · Golem de Vaisselle · Camil · Ceyn (2 formes).

### Battlers d'ennemis
24 ennemis communs (section 10). Recolorations possibles (sbires, abeilles).

### Décors spéciaux
- Interface « liste de salons Discord » pour la carte du monde.
- Fenêtre d'annonce du Modérateur.
- Boîte grise « Vous n'avez pas la permission d'envoyer des messages dans ce salon ».
- Affiches et statue d'Alex ; socle géant et statue minuscule de Camil ; portraits de Camil.
- Slides des PowerPoint (8 images de première slide).
- Lettres « ZINGIS » lumineuses sur la piste.

---

## 20. Placeholders à compléter

| Où | Quoi | Qui |
|---|---|---|
| 1-5-a | Vrais messages épinglés du Discord | Jordan |
| 1-7 et F-1 | Vrai premier échange de la Red Room (garder une ligne « Message supprimé » pour Ceyn) | Jordan |
| 3-3 | Questions du quiz sur Bidou (private jokes) | Jordan |
| 5-4 et F-6 | Nom du tracteur de Florian (« Michel » provisoire) | Florian / Jordan |
| 2-2, 2-4, 2-7 | Jordan était-il à Düsseldorf en 2023 ? (le texte reste ambigu) | Jordan |
| Général | Valider que chaque ami est d'accord avec son portrait | Toute la Red Room |

---

## 21. Mon avis, risques et recommandations

**Ce qui fonctionne bien**
- La structure « un salon = un ami = un boss » est claire et facile à découper en lots de travail.
- Les interventions scriptées rendent les combats vivants sans compliquer la technique : ce sont des événements de troupe standards.
- Le gag « Ceyn. » qui cache le twist est le meilleur moment du jeu : à soigner en priorité au montage (rythme, absence totale d'emphase).

**Risques et recommandations**
1. **Périmètre** : 10 boss, 40 cartes, 8 héros, c'est beaucoup pour une petite équipe. Je recommande de produire d'abord une **tranche verticale** (prologue et chapitre 1 complets, avec sons et visages), puis de valider le ton avec la Red Room avant de lancer le reste.
2. **Personnes réelles** : le jeu met en scène de vraies personnes, y compris deux en méchants. Gardez-le **strictement privé**, et faites valider leur portrait par les amis concernés. Pour Camil et Ceyn, l'écriture reste sur l'ego, le look et les gags, sans rien de la vraie vie au-delà de ça. C'est volontaire, à préserver.
3. **Propriété intellectuelle** : références à LoL, Rocket League, Karmine Corp, Vitality, Discord, Pokémon. Pour un projet privé, les clins d'œil textuels vont bien, mais **ne pas réutiliser d'assets officiels** (logos, musiques, sprites, le jingle de Pierre). Créer des équivalents originaux.
4. **Équilibrage** : les chiffres de ce document sont des points de départ. Prévoir un playtest par chapitre, avec un objectif de 2 à 3 tentatives maximum par boss.
5. **Rythme des gags** : les gags récurrents (pet de Snow, « Ah, ça pue », râteaux, prix +30 %) doivent rester rares sur la carte, sinon ils fatiguent. Les déclencher surtout en scène scriptée.

**Moteur** : RPG Maker MZ, pour aller vite et rester dans du RPG classique. Godot seulement si l'équipe a déjà un développeur à l'aise et veut un rendu très personnalisé.

---

## 22. Plan de travail et quand me solliciter

### Phases proposées
| Phase | Contenu | Livrable |
|---|---|---|
| **0. Préproduction** | Choix du moteur, validation des portraits par la Red Room, liste d'assets priorisée | Projet vide + base de données de test |
| **1. Tranche verticale** | Prologue + chapitre 1 complets (cartes, PNJ, Crypte, boss B01, CE01 à CE05) | Version jouable de 30 minutes |
| **2. Production chapitres 2 à 4** | Un chapitre à la fois | Versions jouables successives |
| **3. Production chapitres 5 à 7** | Idem | |
| **4. Barbecue et Final** | Hub, Tour, Camil, Ceyn, épilogue | Jeu complet |
| **5. Polish** | Équilibrage, sons, textes finaux, bugs | Version finale |

### Quand me relancer (et quoi me demander)
| Moment | Ce que je peux produire | Exemple de demande |
|---|---|---|
| Avant chaque chapitre | **Fiche d'intégration détaillée** : chaque événement de carte, page par page, avec conditions, switches et textes exacts | « Fais-moi la fiche d'intégration du chapitre 2 pour RPG Maker MZ. » |
| Pendant le montage | **Dialogues finaux** découpés en boîtes de texte (longueur max par boîte, nom, visage à utiliser) | « Découpe le chapitre 3 en boîtes de dialogue RPG Maker, 3 lignes max, avec le visage à afficher. » |
| PNJ | Répliques supplémentaires, variantes selon l'avancement (`V010`) | « Donne 3 répliques par PNJ de Généralia selon le chapitre. » |
| Combats | **Événements de troupe** détaillés pour chaque boss, valeurs révisées après playtest | « Le Grand Mute est trop dur, voici nos stats : rééquilibre-le. » |
| Objets, compétences | Descriptions courtes (≤ 2 lignes) pour les menus | « Écris les descriptions d'objets et de compétences pour la base de données. » |
| Énigmes | Grilles concrètes (glace, blocs, interrupteurs, miroirs) avec la solution | « Conçois la grille du Lac Gelé en 20×20 avec la solution. » |
| Contenu bonus | Quêtes secondaires, succès, dialogues de l'auberge | « Propose 5 quêtes secondaires courtes. » |
| Retours de la Red Room | Réécriture d'un personnage ou d'une scène | « Florian veut que son tracteur s'appelle X, et trouve sa scène trop longue. » |
| Godot | Format JSON des données (acteurs, compétences, objets, dialogues) | « Convertis les sections 6 à 11 en JSON pour Godot. » |

> **Astuce** : pour chaque demande, pointez-moi vers `story-pipeline/` (script, fiches, cette bible) : tout le contexte y est, je repars de là.
