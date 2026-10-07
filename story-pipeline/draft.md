# RED ROOM — Le Serveur Maudit
### Script v0.2 : Prologue + Chapitre 1 (version détaillée)

> **Conventions** (compatibles RPG Maker et Godot) :
> `[DÉCOR]` décor ou ambiance · `[MUSIQUE]` / `[SFX]` son · `[ÉVÉNEMENT]` action scriptée · `[CHOIX]` choix du joueur · `[COMBAT]` déclenche un combat · `[DISCORD]` faux message affiché dans l'interface Discord du jeu · `[FLAG]` variable de jeu.
> `NOM :` réplique · *(didascalie)*
>
> **Mécanique globale « Ceyn. »** : chaque fois que le nom de Ceyn s'affiche ou est prononcé, chaque membre présent de l'équipe dit « Ceyn. » dans une bulle, à tour de rôle et sans autre commentaire.

---

## PROLOGUE : « Free RP 100% legit »

### SCÈNE P-1 : Le QG, 03 h 47

[DÉCOR] Un appart plongé dans le noir. Un écran allumé, une Switch abandonnée sur le plateau de Mario Party, une forêt de canettes. Une odeur suspecte flotte : un petit nuage vert pixelisé monte d'une litière dans le coin.
[ÉVÉNEMENT] **Snow**, gros chat blanc, est couché *sur* le clavier. Il fixe Jordan sans cligner des yeux.
[MUSIQUE] Le *bloop* de connexion Discord, en boucle, façon lo-fi.
[DISCORD] 🔊 **Red Room — vocal** · 7 connectés

FLORIAN : MAIS IL EST OÙ LE SUPPORT ? IL EST OÙ ??
BIDOU : *(essoufflé)* Je suis… *(inspire)* … juste… *(inspire)* … derrière toi…
FLORIAN : Derrière moi ? Derrière moi y a que ma tombe, Bidou !
BIDOU : Ok. Ok. Je mute. Je suis vexé. Je mute.
[SFX] *bip* : Bidou s'est rendu muet.
JORDAN : Calmez-vous, je vous carry la prochaine. Comme d'hab.
FLORIAN : Ouais bah carry-nous plus vite, l'ancêtre.
KEVIN : Techniquement, si on calcule l'angle d'approche de leur jungler par rapport à la rivière… on était cooked. Genre complètement. Skibidi cooked.
ROBIN : Les gars, je me lève à 5 h. On m'a donné un fusil et pas un GPU, je vous rappelle. C'est un scandale politique.
JOSÉ : Moi je reste, je suis un mec cool. Les mecs cools dorment pas.
JORDAN : Yanis, t'es là ?
*(Silence. Trois secondes. Cinq secondes.)*
YANIS : … ouais.
JORDAN : Tu fais quoi ?
YANIS : … je mange.
JORDAN : Tu manges quoi ?
*(Longue pause.)*
YANIS : … le même sandwich que tout à l'heure.

[SFX] Un *miaou* rauque dans le micro de Jordan.
KEVIN : C'est Snow ? Dis-lui que je l'aime. Et dis-lui de pas chier pendant qu'on joue, on a senti la dernière fois. À travers Discord. C'est scientifiquement impossible, mais on l'a senti.
JORDAN : Il fait ce qu'il veut, c'est le vrai propriétaire de l'appart.

[ÉVÉNEMENT] Une icône grisée clignote dans la liste des membres : **Alex 🌙 Absent**.
JOSÉ : Alex est encore absent. Il veut pas nous voir, c'est officiel.
FLORIAN : Il est trop beau pour nous, voilà le problème.
[DISCORD] **Alex** : je suis là les gars je vous jure 😅 · *(L'icône repasse immédiatement en « Absent ».)*

### SCÈNE P-2 : Le vocal se vide

[ÉVÉNEMENT] Les membres quittent le vocal un par un, chacun avec son petit *bloop* descendant.
ROBIN : Bonne nuit. Vive la lutte. *bloop*
KEVIN : Demain je vous explique pourquoi la Lune est en fait un sigma. *bloop*
FLORIAN : *(très doux)* Bonne nuit les gars, je vous aime. *(Puis, à son écran :)* ET TOI LE ZED, JE TE RETROUVERAI. *bloop*
BIDOU : *(démute)* Bonne n… *(inspire)* … nuit. *bloop*
JOSÉ : Jordan, tu sais que je t'en veux toujours pour le Portugal ?
JORDAN : Je t'ai PAS désinvité, José.
JOSÉ : C'est ce que dirait quelqu'un qui désinvite. Bonne nuit, vieillard. Pense à prendre tes cachets. *bloop*
YANIS : … bonne… *(L'écran reste figé quatre secondes.)* … nuit. *bloop*

[DISCORD] 🔊 **Red Room — vocal** · 1 connecté
[MUSIQUE] Silence. Juste le ventilo du PC. Et Snow qui gratte sa litière, beaucoup trop longtemps.

JORDAN : *(seul)* 29 ans. Une voiture, un appart, un vrai travail. Et je suis encore là à 4 h du mat'. *(Il s'étire. Un craquement de dos résonne, avec une icône « -5 PV ».)* Aïe. Mes lombaires.

### SCÈNE P-3 : Le lien

[SFX] *Ding.* Une notification.
[DISCORD] **#général**
> **Camille** : free RP 100% legit 👉 `redroom.gift/claim` · *(il y a 1 minute)*

JORDAN : … Camille ? Il est encore sur le serveur, lui ? Je croyais qu'on l'avait…
[ÉVÉNEMENT] Sous le message, une seule réaction apparaît : **👀 1**.
[ÉVÉNEMENT] *(Optionnel, si le joueur survole la réaction.)* Une infobulle affiche : « **Ceyn** a réagi avec 👀 ». Le profil indique : *Inactif*.
JORDAN : *(machinalement, comme tout le monde le ferait)* … Ceyn.
> **Note de mise en scène** : le gag doit servir de camouflage à l'indice. Le joueur rit et passe à autre chose. Pas de musique, pas de zoom.

[CHOIX]
1) Cliquer sur le lien.
2) Ne pas cliquer, aller dormir comme un adulte responsable de 29 ans.

*Si 2 :*
JORDAN : Non. J'ai l'âge de ne pas cliquer sur des liens de Camille. J'ai l'âge de beaucoup de choses, d'ailleurs.
[ÉVÉNEMENT] Jordan se lève (craquement de dos). Pendant qu'il se retourne, **Snow** marche lentement sur le clavier : *tap… tap… Entrée.*
[SFX] *Clic.*
JORDAN : SNOW. NON.
SNOW : *(le regarde droit dans les yeux)* … mrrp.
[FLAG] `snow_a_clique = true` *(Clyde y fera référence au chapitre 1.)*

*Si 1 :*
[SFX] *Clic.*
[FLAG] `snow_a_clique = false`

*(Convergence.)*
[ÉVÉNEMENT] L'écran affiche : `Réclamation de votre RP… 12%… 48%… 99%…`, puis : `Bienvenue dans la Red Room. Pour de vrai.`
[ÉVÉNEMENT] L'interface Discord **sort de l'écran**. Les salons s'étirent comme des lianes, la liste des membres s'enroule autour du poignet de Jordan, et le *bloop* de connexion devient un grondement. Snow est soulevé à côté de lui, toujours parfaitement calme, en train de se lécher la patte.
JORDAN : Non non non non, j'ai juste… on a juste cliqué !
[SFX] *BLOOP* titanesque.
[ÉVÉNEMENT] Fondu au blanc.

---

## CHAPITRE 1 : Généralia

### SCÈNE 1-1 : Réveil dans #général

[DÉCOR] Une immense place pavée de **vieux messages** gravés dans la pierre : « mdr », « qui pour une game », « c'est qui qui a pris ma chaise au barbecue ». Des emojis géants servent de statues, et un 💀 de vingt mètres fait office de fontaine. Le ciel est le fond gris de Discord, en mode sombre évidemment.
[MUSIQUE] Thème de **Généralia** : un thème de capitale RPG, avec un sample du *ping* de notification.

[ÉVÉNEMENT] Jordan est allongé au milieu de la place. Snow n'est plus là. Un petit robot bleu et rond, un peu rouillé, le pique avec un bâton.
??? : Hé. Hé ho. T'es un utilisateur ? Un vrai ?
JORDAN : *(se relève, craquement de dos)* Aïe. Aïe aïe aïe.
??? : Wow. T'as fait un bruit de fossile.
JORDAN : … t'es qui, toi ?
CLYDE : Clyde. Ancien bot officiel. Mis à la retraite. Personne se souvient de moi, c'est normal, t'inquiète. *(Il scanne Jordan avec un petit laser.)* Bip. Compte détecté. Membre depuis… *(son laser grésille)* … l'Ère Secondaire ? T'as connu les dinosaures, toi ?
JORDAN : Pourquoi tout le monde me dit ça, même ici ?
CLYDE : Parce que c'est écrit sur ton profil, en gros. « Vétéran ». Et « Possède une voiture ». C'est rare ici. Les gens vont te demander des sous.

*Si `snow_a_clique = true` :*
CLYDE : Mes capteurs indiquent que ce n'est pas toi qui as cliqué sur le lien. Un utilisateur à quatre pattes. Très poilu. Très… *(il renifle)* … odorant.
JORDAN : Snow. Il est où, Snow ?!

*Sinon :*
JORDAN : Attends… Snow ! Mon chat ! Il était avec moi !

*(Convergence.)*
CLYDE : Un chat ? Blanc ? *(Il frissonne.)* Tu parles de **la Bête Blanche** ? Elle est apparue cette nuit. Personne l'a vue en entier. On trouve seulement ce qu'elle laisse derrière elle. Des… reliques.
JORDAN : Oh non.
CLYDE : Des reliques qui sentent la fin du monde.
JORDAN : Oh non non non.

CLYDE : Bref. Tu es dans #général. Enfin, ce qu'il en reste. Depuis que le **Modérateur Fou** a pris le contrôle, plus personne parle ici. Les memes ont été bannis, les vocaux mutés et les AFK… *(il baisse la voix)* … kickés dans le Marais.
JORDAN : Et mes potes ? Ils sont où ?
CLYDE : Éparpillés dans les salons. Mais il y en a un pas loin. Il creuse depuis trois jours. Il dit qu'il fait de « l'archéologie ».
JORDAN : … José.

[ÉVÉNEMENT] **Clyde rejoint l'équipe (guide, non combattant).** Tutoriel de déplacement.
[FLAG] `quete_bete_blanche = active` *(Quête secondaire : « La Bête Blanche ». Objectif : retrouver Snow.)*

### SCÈNE 1-2 : Généralia sous le régime (exploration libre)

> Zone ouverte : trois points d'intérêt obligatoires, plus des PNJ optionnels. Le joueur peut les faire dans l'ordre qu'il veut.

**A. La Place Camille**
[DÉCOR] L'ancienne grand-place, rebaptisée. Une statue géante de **Camille**, les bras croisés, le menton levé, sur un socle gravé : « *Le Seul Vrai Fondateur (selon lui)* ». *(Le « selon lui » a été rajouté au marqueur par un anonyme.)*
CLYDE : Il a fait renommer la place la semaine dernière. Avant, ça s'appelait « Place de la Red Room ». Avant ça, « Place des gens qui s'entendent bien ».
JORDAN : Ça a pas duré longtemps, celle-là.
[ÉVÉNEMENT] Une plaque au pied de la statue : « *Tout citoyen est prié de complimenter la statue en passant. — C.* »
[CHOIX]
1) Complimenter la statue.
2) Ne rien dire.
3) Jeter une canette dessus.
*Si 1 :* JORDAN : « … belle… pierre. » · La statue ne réagit pas. Clyde a l'air déçu de toi.
*Si 2 :* Rien ne se passe. Clyde approuve en silence.
*Si 3 :* [SFX] *Clong.* Un PNJ applaudit au loin. Objet obtenu : **Respect des Citoyens**, un objet de quête sans utilité, mais qui fait plaisir.

**B. La Boutique de Mme Nitro-Pas-Chère**
[DÉCOR] Une échoppe de badges, de stickers et de bannières de profil.
MARCHANDE : Un client ! Avec une voiture ! *(Les prix de la boutique augmentent tous de 30 % sous nos yeux.)*
JORDAN : Vous venez de monter vos prix.
MARCHANDE : Inflation, monsieur. C'est la faute du Modérateur.
> **Tutoriel boutique** : présentation de la compétence *Carte Bleue* de Jordan. Elle peut aussi servir à **payer** certains PNJ pour sauter des quêtes, mais à prix « Jordan ».

**C. Le Mur des Mutés**
[DÉCOR] Une rangée de citoyens dont la bouche est barrée d'un 🔇. Ils s'expriment uniquement en emojis.
CITOYEN MUTÉ : 😶 👉 🔨 🤖 😭
CLYDE : Il dit que le Modérateur l'a muté pour avoir posté « ptdr ».
JORDAN : Juste « ptdr » ?
CITOYEN MUTÉ : 😤 ✋ *(Clyde : « Deux fois. »)*

**PNJ optionnels**
- **Utilisateur Supprimé** : « Je me souviens plus de qui j'étais. C'est reposant, en vrai. »
- **Un vieux Bot de Musique** : « Avant on passait de la musique dans les vocaux. Maintenant YouTube m'a… *(grésillement)* … Personne ne se souvient de moi non plus. » *(Clyde et lui se font un câlin de robots retraités.)*
- **Un Enfant de Généralia** : « Monsieur, c'est vrai que vous avez connu les dinosaures ? » / JORDAN : « … oui. Ils jouaient support. »
- **Trace de la Bête Blanche n° 1** : une petite empreinte de patte et un nuage vert. Les PNJ autour se bouchent le nez. Clyde : « Elle est passée par là. Il y a au moins deux heures. Et ça sent encore. »

### SCÈNE 1-3 : Le chantier de fouilles

[DÉCOR] Une tranchée creusée dans le sol de #général. On y voit les **strates de messages** : 2026, 2025, 2024… et tout au fond, une couche marquée « **DÜSSELDORF** ». Des panneaux « Chantier — Ne pas marcher sur l'histoire ».
[ÉVÉNEMENT] José est en tenue d'explorateur : chapeau, foulard, petit pinceau. Son pantalon tombe *parfaitement* sur ses baskets. Il prend une seconde pour vérifier, puis recommence à creuser.

JOSÉ : *(sans se retourner)* Ne marche pas sur la strate 2023. Il y a le premier « gg ez » de Florian, c'est un fossile fragile.
JORDAN : José !
JOSÉ : *(se retourne, pinceau levé)* Jordan. Évidemment. Tu viens me désinviter de mes fouilles aussi ?
JORDAN : Je t'ai jamais désinvité !
JOSÉ : Le Portugal se souvient, Jordan. Le Portugal se souvient.

[CHOIX]
1) « Je t'ai pas désinvité, c'est toi qui pouvais pas venir. »
2) « Ok. Je t'ai désinvité. Pardon. »
3) « T'es stylé avec ce chapeau. »

*Si 1 :*
JOSÉ : C'est exactement ce que dirait quelqu'un qui désinvite.
*Si 2 :*
JOSÉ : *(choqué)* … tu AVOUES ? *(Il range son pinceau, très digne.)* Je te pardonne. Parce que je suis un mec cool.
[FLAG] `jose_aveu_portugal = true` *(Réplique bonus dans l'interlude du Barbecue.)*
*Si 3 :*
JOSÉ : *(immédiatement radouci)* Je sais. Regarde comment le pantalon tombe sur la paire. Tu vois ça ? Ça aussi c'est de l'archéologie. C'est un savoir ancestral. *(Il plisse les yeux.)* Toi aussi t'es un savoir ancestral, remarque.

*(Convergence.)*
JOSÉ : Bon. T'as vu ce qui se passe ? Tout le serveur est cassé. Moi j'ai atterri ici, et je me suis dit : tant qu'à faire, autant fouiller. Et regarde ce que j'ai trouvé ce matin.
[ÉVÉNEMENT] Il sort d'une caisse, avec des gants et un respect infini, un **petit objet brun** posé sur un coussin de velours. Un nuage vert s'en échappe.
JOSÉ : Un artefact. Préhistorique. Il dégage une aura incroyable. Ça fait trois heures que je l'étudie et j'ai les yeux qui pleurent. C'est l'émotion, je pense.
JORDAN : José.
JOSÉ : Probablement une offrande rituelle de l'époque Düsseldorf.
JORDAN : José, c'est un caca de Snow.
*(Long silence.)*
JOSÉ : *(regarde l'objet, regarde Jordan, regarde l'objet)* … ça reste un artefact.
CLYDE : C'est la Bête Blanche.
JOSÉ : La Bête Blanche, c'est SNOW ? *(Il lâche le coussin.)* J'ai dormi à côté. J'ai DORMI à côté, Jordan.

[ÉVÉNEMENT] Objet obtenu : **Relique Puante ×1**. *Description : « Un artefact de très grande valeur olfactive. Utilisable en combat : empoisonne tous les ennemis. Snow en produit gratuitement et sans limite. »*

JOSÉ : Bref. Ma vraie découverte, c'est ça.
[ÉVÉNEMENT] Il montre au fond de la tranchée une porte de pierre scellée, gravée d'une **épingle 📌** géante. Une petite empreinte de patte est visible devant.
JOSÉ : La **Crypte des Messages Épinglés**. Les anciens disent qu'elle contient le premier message de la Red Room. Celui de Düsseldorf.
JORDAN : C'est qui, « les anciens » ?
JOSÉ : Moi. Je l'ai dit hier. À Clyde.
CLYDE : Il l'a dit.
JORDAN : Et les traces de pattes, là, ça va vers la crypte.
JOSÉ : Ton chat est entré dans mon site archéologique ? *(Il ajuste son chapeau.)* Bon. On y va. Mais si on trouve un trésor, c'est moi qui le mets au musée.

### SCÈNE 1-4 : Intermède : la passante

[ÉVÉNEMENT] Une PNJ traverse la place : **Nitro**, en tenue scintillante violette.
[ÉVÉNEMENT] José se redresse, ajuste son foulard et vérifie la tombée de son pantalon. Il s'avance avec une démarche « mec cool ». Jingle de drague, façon Pierre dans Pokémon.
JOSÉ : Mademoiselle. Archéologue. Stylé. Disponible.
NITRO : Je coûte 9,99 € par mois.
JOSÉ : … je peux faire un essai gratuit ?
NITRO : Non.
[ÉVÉNEMENT] Elle s'éloigne. Jingle triste.
NITRO : *(se retourne, vers Jordan)* Vous, par contre, vous avez une voiture, non ?
JORDAN : J'ai 29 ans, madame.
NITRO : *(le regarde de haut en bas)* Ah oui. On dirait plus.
[ÉVÉNEMENT] Elle part pour de bon.
JOSÉ : *(revient vers Jordan, imperturbable)* Elle reviendra.
JORDAN : Elle reviendra pas.
JOSÉ : Elles reviennent toujours. *(Pause.)* Enfin. Une fois, peut-être, une est revenue.
[FLAG] `rateaux_jose += 1`

> **Note gameplay** : chaque chapitre contient une PNJ féminine et une tentative de drague de José, toujours ratée. Compteur caché « Râteaux de José » ; succès « Pierre de Kanto » débloqué à la fin du jeu.

### SCÈNE 1-5 : La Crypte des Messages Épinglés (donjon)

[ÉVÉNEMENT] **José rejoint l'équipe.**
JOSÉ : Je vous préviens, j'ai jamais joué de RPG. Moi c'est Neon. Je cours vite et je réfléchis après.
JORDAN : C'est exactement ta façon de jouer dans la vraie vie, en fait.
JOSÉ : Et ça me réussit. Regarde-moi.
JORDAN : Je te regarde. Ton chapeau est à l'envers.
JOSÉ : *(le remet droit, très vite)* C'était un choix.

> **Tutoriel combat** :
> - **Jordan** : *Tir de l'Ancien* (longue portée), *Brume Ancestrale* (soin de groupe), *Douleurs Lombaires* (passif, 5 % de chance de rater son tour, « Aïe »).
> - **José** : *Sprint Néon* (agit toujours en premier), *Je suis un mec cool* (immunisé à la peur), *Tombé de pantalon parfait* (buff de charisme ; inefficace contre les ennemies, qui ont l'air de s'en ficher).
> - Objet : *Relique Puante* (poison de zone).
>
> **Ennemis de la zone** :
> - **Spam-bots** : « CLIQUEZ ICI POUR GAGNER », attaques faibles mais nombreuses.
> - **Notifications Fantômes** : attaque « Vous avez 99+ mentions », statut *Distrait*.
> - **Réactions Abandonnées** : des 👍 errants. Ils fuient si on leur répond « ok ».
> - **Sbires du Modérateur** : petits marteaux 🔨 sur pattes. Leur attaque *Avertissement* fait passer un allié en *Muet* (plus de compétences).

#### 1-5-a : La Salle des Strates
[DÉCOR] Un long couloir où les murs sont des messages des années passées, comme des fresques.
[ÉVÉNEMENT] Des **messages épinglés** sont encadrés comme des reliques. José s'arrête devant chacun pour faire le guide.
- « BARBECUE DE LA RED ROOM — samedi, ramenez les saucisses, PAS DE DÉSINVITATION »
  JOSÉ : *(très ému)* … Le jour le plus important de l'histoire de l'humanité. Ils l'ont gravé dans la pierre.
- « Europa Park : RDV 7 h, et Yanis tu pars à 5 h stp »
  JORDAN : Il est arrivé à 9 h.
  JOSÉ : C'était un exploit, pour lui.
- « Worlds Rocket League — on y croit les gars » *(La fresque est fissurée. Une petite larme de pierre coule.)*
  JOSÉ : On évite d'en parler devant Kevin. Il est encore dans le deuil.
- ❓ *Placeholder : vrais messages épinglés du Discord, à fournir par Jordan.*

#### 1-5-b : Énigme : le Couloir des Notifications
> Puzzle : des dalles de notification s'allument. En marcher sur une déclenche un *ding* et fait apparaître un ennemi. Le joueur doit passer par les dalles grises, celles des notifications **désactivées**.
CLYDE : Astuce de vieux bot : la seule notification qui ne fait jamais mal, c'est celle qu'on a désactivée.
JORDAN : C'est la phrase la plus sage que j'aie entendue de l'année.

[ÉVÉNEMENT] *Trace de la Bête Blanche n° 2* : au milieu du puzzle, une dalle verte qui fume. Si le joueur marche dessus : -10 PV à toute l'équipe, statut *Nausée* pendant trois combats.
JOSÉ : Il a fait ÇA dans un site classé ?!

#### 1-5-c : La Porte des Fondateurs
[DÉCOR] Une grande porte rouge. Au-dessus, une inscription : « *Seuls ceux qui savent d'où vient le nom peuvent entrer.* »
JOSÉ : C'est facile. *(Il pose la main sur la porte. Sa voix se fait plus douce.)* Düsseldorf. Le premier événement Rocket League. On était dans la même chambre, les fondateurs. Moi, Kevin, Robin, Bidou… La chambre avait une lumière bizarre. Rouge. Toute la nuit, impossible de l'éteindre. Le lendemain, quelqu'un a dit « on est la Red Room », et c'est resté.
JORDAN : Vous étiez quatre ?
JOSÉ : Ouais, quatre. *(Pause.)* Enfin… il y avait cinq lits. Je sais plus pourquoi. Peut-être qu'il y avait un lit en trop.
[ÉVÉNEMENT] *(Pas d'insistance. Le joueur tape le mot de passe.)*
> Saisie : `RED ROOM`
[ÉVÉNEMENT] La porte s'ouvre. Une lumière rouge baigne la salle suivante. Le thème musical passe en version douce, orgue et ping de notification.

#### 1-5-d : Mini-rencontre : la Bête Blanche
[ÉVÉNEMENT] Dans l'antichambre : un bruit de grattage, un nuage vert. Une silhouette blanche massive dans l'ombre, deux yeux qui brillent.
CLYDE : *(caché derrière Jordan)* LA BÊTE BLANCHE.
[ÉVÉNEMENT] La silhouette sort de l'ombre. C'est Snow, totalement normal, assis sur une épingle dorée géante qu'il refuse de lâcher.
JORDAN : Snow ! Viens là, mon gros.
SNOW : *(le regarde, puis se retourne et s'éloigne dans la salle du boss)* … mrrp.
JOSÉ : Il t'ignore.
JORDAN : Il fait toujours ça. C'est ce qui fait son charme.
JOSÉ : Il a un charme, ce chat ? Il a un PROBLÈME DIGESTIF, ce chat.

### SCÈNE 1-6 : Boss : le Gardien des Épinglés

[DÉCOR] Une salle ronde baignée de rouge. Au centre, un socle avec un message sous verre : le **premier message de la Red Room**, brouillé, illisible. Snow est assis *sur* la vitrine.
[ÉVÉNEMENT] Une gigantesque **épingle 📌** se déplie comme un insecte en métal.
GARDIEN DES ÉPINGLÉS : CONTENU NON CONFORME. CE MESSAGE CONTIENT : HUMOUR. AMITIÉ. FAUTES D'ORTHOGRAPHE. SUPPRESSION REQUISE.
GARDIEN DES ÉPINGLÉS : *(se tourne vers Snow)* ET UN ANIMAL. LES ANIMAUX SONT INTERDITS DANS LES ARCHIVES.
SNOW : *(le fixe et, très lentement, fait tomber un petit objet de la vitrine)*
JOSÉ : Supprimer un message de Düsseldorf ? C'est du vandalisme archéologique.
JORDAN : Et personne touche à mon chat. Sauf moi. Pour nettoyer la litière.

[COMBAT] **Gardien des Épinglés** (boss tutoriel, 3 phases)
- **Phase 1 : Archivage**
  - *Épinglage* : immobilise un allié un tour.
  - *Rappel à l'ordre* : inflige *Muet*.
  - Faiblesse : *Fouille des messages épinglés* de José, qui « désépingle » le boss et lui retire son armure.
- **Phase 2 (sous 60 % de PV) : Désinvitation**
  - Le Gardien lance *Retrait d'Invitation* : José est expulsé du combat pendant deux tours.
  - Réplique, GARDIEN : « VOUS N'ÊTES PLUS INVITÉ. »
  - JOSÉ *(revient au bout de deux tours, furieux ; bonus d'attaque permanent pour le combat)* : « Personne. Ne. Me. Désinvite. *(Il regarde Jordan.)* Plus jamais. »
  - JORDAN : « Je t'ai JAMAIS désinvité ! »
- **Phase 3 (sous 25 % de PV) : Intervention de Snow**
  - Le Gardien vise la vitrine pour effacer le message.
  - Événement automatique : Snow saute de la vitrine, se poste devant le Gardien, le fixe et… dépose une **relique fraîche** sur son socle.
  - GARDIEN : « ODEUR… NON… CONFORME… » · Le boss subit *Nausée* (défense divisée par deux).
  - Le joueur finit le combat.

### SCÈNE 1-7 : Le premier message

[ÉVÉNEMENT] Le Gardien s'effondre en petites punaises. Le verre se brise et le premier message devient lisible :
[DISCORD] **#général**, il y a très longtemps
> **José** : on est la red room maintenant
> **Bidou** : pk
> **Kevin** : la lumière est rouge frérot
> *[Message supprimé]*
> **Robin** : vote à main levée : adopté

> ❓ *À remplacer par le vrai premier échange si vous l'avez encore. Garder une ligne « Message supprimé » : c'est une graine du twist (c'est Ceyn qui l'avait écrite).*

JOSÉ : *(doucement)* Ça va paraître bizarre, mais… c'est le truc le plus beau que j'aie jamais déterré.
JORDAN : Plus beau que tes baskets ?
JOSÉ : *(longue réflexion)* … presque.
JORDAN : Et le message supprimé, là, c'était qui ?
JOSÉ : Aucune idée. *(Il se gratte la tête sous son chapeau.)* Quelqu'un qui a dit un truc et qui l'a regretté, je suppose. Ça arrive à tout le monde.

[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (1/7)**. *Description : « Un morceau de l'histoire de la Red Room. Il en faut sept pour ouvrir la Tour des Modérateurs. »*
[ÉVÉNEMENT] Snow se frotte enfin contre la jambe de Jordan. Ronronnement.
**Snow rejoint l'équipe (compagnon).** *Il suit Jordan sur la carte. De temps en temps, il s'arrête et refuse d'avancer pendant trois secondes. Il génère une Relique Puante tous les 10 combats.*
[FLAG] `quete_bete_blanche = terminee`
JOSÉ : Le premier qui le met dans mon sac de fouilles, je le désinvite.
JORDAN : Ah ! Tu vois que ça existe, désinviter quelqu'un !
JOSÉ : … c'est pas pareil.

### SCÈNE 1-8 : L'annonce

[SFX] Un *@everyone* résonne dans tout Généralia, si fort que les statues d'emojis tremblent.
[ÉVÉNEMENT] Retour à la surface. Le ciel affiche un message géant, en lettres rouges :
[DISCORD] **#annonces** · 🔨 **Modérateur Fou** (BOT)
> @everyone Des utilisateurs non autorisés ont été détectés dans #général. Rappel du règlement :
> 1) Pas de memes. 2) Pas de vocal. 3) Pas d'AFK. 4) Pas d'amis. 5) Pas de chats.
> Merci de votre compréhension.
> — *Approuvé par Camille, Fondateur, Visionnaire, Meilleur Joueur du Serveur*

[ÉVÉNEMENT] Un hologramme géant de **Camille** apparaît au-dessus de sa statue, prenant exactement la même pose qu'elle.
CAMILLE : Citoyens de Généralia. Vous l'avez sûrement remarqué : le serveur va mieux depuis que je m'en occupe.
CITOYEN MUTÉ : 😐
CAMILLE : J'ai toujours dit que la Red Room avait besoin d'un vrai leader. Quelqu'un de talentueux. De brillant. De modeste. *(Il marque une pause pour laisser le temps aux applaudissements. Il n'y en a pas.)* Bref. Moi.
CAMILLE : Jordan, je sais que tu es là. Avec ton chat. Et ton dos. Rentre chez toi, l'ancêtre. Ici, c'est **mon** serveur maintenant.
[ÉVÉNEMENT] L'hologramme se coupe au milieu d'un mot, comme si quelqu'un avait débranché une prise. *(Graine : ce n'est pas Camille qui contrôle la diffusion.)*

JOSÉ : … il a pas changé, hein.
JORDAN : Le même ego, en hologramme de trente mètres.
CLYDE : *(tout petit)* La Caserne d'Annonces est par là. Le Stade Orbital par là. Et le vocal… plus personne ne respire là-haut depuis longtemps.
JOSÉ : Bidou va pas aimer ça.
JORDAN : Bidou aime déjà pas respirer en temps normal.
BIDOU *(voix lointaine, venue du ciel, très faible)* : … j'ai… *(inspire)* … entendu… *(inspire)* … je suis vexé…

[ÉVÉNEMENT] Ouverture de la carte du monde. Les salons **#rocket-league**, **#vocal-1** et **#memes** deviennent accessibles.
[ÉVÉNEMENT] Plan final du chapitre, très bref : dans la liste des membres en bas à droite de l'écran, **Ceyn** passe d'*Inactif* à *En ligne* pendant une demi-seconde, puis redevient *Inactif*.
[ÉVÉNEMENT] *(Si le joueur a l'œil : la mécanique « Ceyn. » se déclenche.)*
JOSÉ : Ceyn.
JORDAN : Ceyn.
[ÉVÉNEMENT] *(Puis ils reprennent leur route comme si de rien n'était.)*

**FIN DU CHAPITRE 1**

---

### Récapitulatif chapitre 1 (pour l'intégration)
- **Recrues** : José (combattant), Snow (compagnon), Clyde (guide).
- **Objets clés** : Fragment du Premier Message (1/7), Relique Puante.
- **Flags** : `snow_a_clique`, `jose_aveu_portugal`, `rateaux_jose`, `quete_bete_blanche`.
- **Graines du twist posées** : 👀 de Ceyn (prologue) ; le cinquième lit de Düsseldorf (1-5-c) ; le message supprimé (1-7) ; l'hologramme de Camille coupé par quelqu'un d'autre (1-8) ; Ceyn brièvement « En ligne » (1-8).
