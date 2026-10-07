# RED ROOM — Le Serveur Maudit
### Script v0.4 : Prologue + Chapitres 1 à 3

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
> **Camil** : free RP 100% legit 👉 `redroom.gift/claim` · *(il y a 1 minute)*

JORDAN : … Camil ? Il est encore sur le serveur, lui ? Je croyais qu'on l'avait…
[ÉVÉNEMENT] Sous le message, une seule réaction apparaît : **👀 1**.
[ÉVÉNEMENT] *(Optionnel, si le joueur survole la réaction.)* Une infobulle affiche : « **Ceyn** a réagi avec 👀 ». Le profil indique : *Inactif*.
JORDAN : *(machinalement, comme tout le monde le ferait)* … Ceyn.
> **Note de mise en scène** : le gag doit servir de camouflage à l'indice. Le joueur rit et passe à autre chose. Pas de musique, pas de zoom.

[CHOIX]
1) Cliquer sur le lien.
2) Ne pas cliquer, aller dormir comme un adulte responsable de 29 ans.

*Si 2 :*
JORDAN : Non. J'ai l'âge de ne pas cliquer sur des liens de Camil. J'ai l'âge de beaucoup de choses, d'ailleurs.
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

**A. La Place Camil**
[DÉCOR] L'ancienne grand-place, rebaptisée. Au centre se dresse un **socle gigantesque** de dix mètres de haut, en marbre, avec des colonnes et des dorures. Au sommet trône une **statue de Camil, minuscule**. Il faut une longue-vue pour la voir. Elle prend une pose héroïque, sur la pointe des pieds. Gravure du socle : « *Le Seul Vrai Fondateur (selon lui)* ». *(Le « selon lui » a été rajouté au marqueur par un anonyme.)*
JORDAN : … elle est où, la statue ?
CLYDE : En haut. Plisse les yeux. *(Jordan plisse les yeux.)* Voilà. Le petit point.
JORDAN : Le socle est plus grand que lui.
CLYDE : Il a beaucoup insisté sur le socle.
CLYDE : Il a fait renommer la place la semaine dernière. Avant, ça s'appelait « Place de la Red Room ». Avant ça, « Place des gens qui s'entendent bien ».
JORDAN : Ça a pas duré longtemps, celle-là.
[ÉVÉNEMENT] Une plaque au pied de la statue : « *Tout citoyen est prié de complimenter la statue en passant. — C.* »
[CHOIX]
1) Complimenter la statue.
2) Ne rien dire.
3) Jeter une canette dessus.
*Si 1 :* JORDAN : *(crie vers le haut)* « … BEAU… SOCLE ! » · La statue ne réagit pas. Clyde a l'air déçu de toi.
*Si 2 :* Rien ne se passe. Clyde approuve en silence.
*Si 3 :* La canette n'atteint même pas le sommet du socle. [SFX] *Clong.* Un PNJ applaudit quand même au loin. Objet obtenu : **Respect des Citoyens**, un objet de quête sans utilité, mais qui fait plaisir.

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
> - **Jordan** : *Tir de l'Ancien* (mono), *Brume Ancestrale* (soin de groupe), *Souvenirs du Crétacé* (debuff défense).
> - **José** : *Coup de Pinceau* (mono), *Sprint Néon* (mono rapide), *Tombé de Pantalon Parfait* (buff défense sur soi).
> - Objet : *Relique Puante* (dégâts de zone et poison).
>
> **Ennemis de la zone** :
> - **Spam-bots** : « CLIQUEZ ICI POUR GAGNER », attaques faibles mais nombreuses.
> - **Notifications Fantômes** : attaque « Vous avez 99+ mentions », statut *Confusion*.
> - **Réactions Abandonnées** : des 👍 errants, faibles, ils fuient souvent le combat.
> - **Sbires du Modérateur** : petits marteaux 🔨 sur pattes. Leur attaque *Avertissement* inflige *Muet* (plus de compétences).

#### 1-5-a : La Salle des Strates
[DÉCOR] Un long couloir où les murs sont des messages des années passées, comme des fresques.
[ÉVÉNEMENT] Des **messages épinglés** sont encadrés comme des reliques. José s'arrête devant chacun pour faire le guide.
- « BARBECUE DE LA RED ROOM — samedi, ramenez les saucisses, PAS DE DÉSINVITATION »
  JOSÉ : *(très ému)* … Le jour le plus important de l'histoire de l'humanité. Ils l'ont gravé dans la pierre.
- « Europa Park : RDV 7 h, et Yanis tu pars à 5 h stp »
  JORDAN : Il est arrivé à 9 h.
  JOSÉ : C'était un exploit, pour lui.
- « Worlds RLCS Düsseldorf — demi-finale KC vs Vitality — on y croit les gars » *(La fresque est fissurée. Une petite larme de pierre coule.)*
  JOSÉ : 4-2. On évite d'en parler devant Kevin. Il est encore dans le deuil.
- ❓ *Placeholder : vrais messages épinglés du Discord, à fournir par Jordan.*

#### 1-5-b : Les Trois Notifications Muettes
> Quête à objets : la porte suivante est bloquée par trois cloches de notification qui sonnent sans arrêt. Il faut trouver trois **Cloches Barrées 🔕** dans les salles du donjon (deux dans des coffres, une portée par un Sbire du Modérateur en combat obligatoire) et les poser sur les trois socles.
CLYDE : Astuce de vieux bot : la seule notification qui ne fait jamais mal, c'est celle qu'on a désactivée.
JORDAN : C'est la phrase la plus sage que j'aie entendue de l'année.

[ÉVÉNEMENT] *Trace de la Bête Blanche n° 2* : dans une des salles, un coffre qui fume en vert. L'ouvrir donne **Relique Puante ×2**, et un message : « Vous avez trouvé un trésor. Malheureusement. »
JOSÉ : Il a fait ÇA dans un site classé ?!

#### 1-5-c : La Porte des Fondateurs
[DÉCOR] Une grande porte rouge. Au-dessus, une inscription : « *Seuls ceux qui savent d'où vient le nom peuvent entrer.* »
JOSÉ : C'est facile. *(Il pose la main sur la porte. Sa voix se fait plus douce.)* Düsseldorf. Les Worlds de Rocket League, 2023. Notre premier événement. On était dans la même chambre, les fondateurs. Moi, Kevin, Robin, Bidou… La chambre avait une lumière bizarre. Rouge. Toute la nuit, impossible de l'éteindre. Le lendemain, quelqu'un a dit « on est la Red Room », et c'est resté.
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
  - *Coup d'Épingle* : mono.
  - *Épinglage* : statut *Paralysie* un tour sur un allié.
  - *Rappel à l'ordre* : statut *Muet* sur un allié.
  - Faiblesse : la *Relique Puante* fait double effet sur lui.
- **Phase 2 (sous 60 % de PV) : Désinvitation**
  - Le Gardien lance *Retrait d'Invitation* : statut *Banni* sur José (il ne peut pas agir pendant deux tours).
  - Réplique, GARDIEN : « VOUS N'ÊTES PLUS INVITÉ. »
  - JOSÉ *(à la fin du statut, furieux ; buff attaque pour le reste du combat)* : « Personne. Ne. Me. Désinvite. *(Il regarde Jordan.)* Plus jamais. »
  - JORDAN : « Je t'ai JAMAIS désinvité ! »
- **Phase 3 (sous 25 % de PV) : Intervention de Snow**
  - Le Gardien gagne *Suppression* : grosse attaque de zone.
  - Événement scripté au début de la phase : Snow saute de la vitrine, se poste devant le Gardien, le fixe et… dépose une **relique fraîche** sur son socle.
  - GARDIEN : « ODEUR… NON… CONFORME… » · Le boss reçoit un debuff défense pour le reste du combat.
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
> — *Approuvé par Camil, Fondateur, Visionnaire, Meilleur Joueur du Serveur*

[ÉVÉNEMENT] Un projecteur s'allume au sommet du socle. Un hologramme de **Camil** apparaît… à taille réelle. On doit zoomer pour le voir. Il se tient sur une caisse marquée « NE PAS ENLEVER ».
CAMILLE : Citoyens de Généralia. Vous l'avez sûrement remarqué : le serveur va mieux depuis que je m'en occupe.
CITOYEN MUTÉ : 😐
CAMILLE : J'ai toujours dit que la Red Room avait besoin d'un vrai leader. Quelqu'un de talentueux. De brillant. De modeste. *(Il marque une pause pour laisser le temps aux applaudissements. Il n'y en a pas.)* Bref. Moi.
CAMILLE : Jordan, je sais que tu es là. Avec ton chat. Et ton dos. Rentre chez toi, l'ancêtre. Ici, c'est **mon** serveur maintenant.
[ÉVÉNEMENT] L'hologramme se coupe au milieu d'un mot, comme si quelqu'un avait débranché une prise. *(Graine : ce n'est pas Camil qui contrôle la diffusion.)*

JOSÉ : … il a pas changé, hein.
JORDAN : Le même ego. Dans le même petit hologramme.
JOSÉ : Il a mis une caisse. Même en hologramme, il a mis une caisse.
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
- **Graines du twist posées** : 👀 de Ceyn (prologue) ; le cinquième lit de Düsseldorf (1-5-c) ; le message supprimé (1-7) ; l'hologramme de Camil coupé par quelqu'un d'autre (1-8) ; Ceyn brièvement « En ligne » (1-8).

---

## CHAPITRE 2 : Le Stade Orbital

> **Contexte** : le Modérateur Fou a enfermé Kevin dans le salon #rocket-league, transformé en stade flottant dans l'espace. Kevin y revit en boucle la **demi-finale des Worlds RLCS de Düsseldorf (13 août 2023)**, perdue 4-2 par la Karmine Corp contre **Vitality**, l'ennemi historique. C'était le même week-end que la naissance de la Red Room. Kevin n'était pas sur le terrain ce jour-là, il était en tribune ; mais le Modérateur l'a mis à la place des joueurs pour que ça fasse encore plus mal.
>
> **Structure** : arrivée, puis exploration et quête à objets en trois parties, puis Kevin libéré, puis boss.

### SCÈNE 2-1 : Décollage

[DÉCOR] À la sortie de Généralia, un **portail en forme de but de Rocket League**. Au-dessus, un néon : « #rocket-league — 1 utilisateur (en boucle) ».
CLYDE : Le salon de Kevin. Attention, la gravité est bizarre là-haut. Le Modérateur a tout réglé sur « Lune ».
JORDAN : Kevin doit être aux anges.
CLYDE : Il est en boucle depuis… *(il calcule)* … quatre cent douze matchs.
JOSÉ : Ah. Donc il est pas aux anges.

[ÉVÉNEMENT] L'équipe traverse le portail en voiture : Jordan au volant d'un *Octane* rouge, José à côté, Snow sur le tableau de bord.
JOSÉ : Pourquoi c'est toi qui conduis ?
JORDAN : Je suis le seul qui a le permis et une voiture, José.
JOSÉ : Même dans un monde imaginaire ?
JORDAN : *Surtout* dans un monde imaginaire.
[SFX] Bruit de boost. [ÉVÉNEMENT] Fondu sur un ciel étoilé.

### SCÈNE 2-2 : Le Stade Orbital

[DÉCOR] Un stade de Rocket League **posé sur un astéroïde**, au milieu des étoiles. On voit la Terre au loin, et un satellite passe. Une banderole géante : « **WORLDS — DÜSSELDORF — DEMI-FINALE** ». Les tribunes sont remplies de **Supporters de la Ruche**, des spectateurs jaunes et noirs aux antennes d'abeille. En face, la tribune rouge, le **Kop Rouge**, est pleine de supporters KC **mutés** : bouche barrée d'un 🔇, ils sont immobiles et tristes.
[MUSIQUE] Thème du **Stade Orbital** : électro épique, version synthwave du menu de Rocket League. À chaque fin de boucle, la musique saute comme un disque rayé.

[ÉVÉNEMENT] *(Cinématique, sans contrôle du joueur.)* Sur le terrain, une voiture bleue fait des acrobaties. Au volant, Kevin, casque de cosmonaute sur la tête. Le tableau d'affichage indique : « **KC 2 – 3 VITALITY · Match 6** ».
KEVIN : *(dans les haut-parleurs du stade, il commente son propre match)* … et Kevin récupère la balle, angle d'approche 37,4 degrés, vitesse optimale, c'est mathématiquement impossible de rater…
[SFX] *BUZZER.* « **VITALITY MARQUE — VITALITY GAGNE LA SÉRIE 4-2** ». Les abeilles bourdonnent de joie.
KEVIN : … c'était mathématiquement impossible de rater.
[ÉVÉNEMENT] Effet de cassette qu'on rembobine. Le tableau revient au début du match 6.
KEVIN : *(même intonation, mot pour mot)* … et Kevin récupère la balle, angle d'approche 37,4 degrés…

JORDAN : Il est bloqué.
CLYDE : Quatre cent treize.
JOSÉ : Mais… Kevin, il jouait même pas ce match. Il était en tribune, avec nous. Il pleurait.
CLYDE : Le Modérateur l'a mis sur le terrain. C'est plus cruel comme ça.
JOSÉ : Il fait le même commentaire à chaque fois ?
CLYDE : Mot pour mot. Sauf la fois 207. Il a dit « skibidi ». On sait pas pourquoi.

[ÉVÉNEMENT] L'équipe tente d'entrer sur le terrain. Une barrière jaune bloque l'accès.
[DISCORD] 🔨 **Modérateur Fou** (BOT) : *Accès au terrain refusé. Motif : ambiance insuffisante. Pour entrer, le stade doit être « en feu ». Bonne chance avec des supporters mutés. 🙂*
CLYDE : Il faut réveiller le stade. Si le Kop Rouge chante, la barrière tombe.
JORDAN : Alors on va le réveiller, ce stade.

> **Quête : « Le Kop Rouge »** (quête à objets, trois parties, dans l'ordre qu'on veut)
> 1. **Les Posters** : ramasser 5 **Posters KC** éparpillés dans le stade et les donner aux supporters mutés.
> 2. **L'Écharpe** : récupérer l'**Écharpe de Kevin** au vestiaire.
> 3. **Le Billet** : récupérer le **Billet Düsseldorf 2023** auprès d'une abeille marchande.
> Quand les trois sont rendus, le Kop Rouge chante et la barrière tombe.

### SCÈNE 2-3 : Les Posters

[ÉVÉNEMENT] Les 5 posters sont cachés sur la carte du stade : un sous les gradins, un dans la buvette, un sur le toit du kiosque à hot-dogs, un dans les mains d'un Sbire du Modérateur (combat), un sous… Snow, qui dort dessus.
*(Poster 5, sous Snow.)*
JORDAN : Snow, bouge.
SNOW : *(ne bouge pas)*
JOSÉ : Il a un problème avec l'autorité, ton chat.
JORDAN : Il a un problème avec tout.
[ÉVÉNEMENT] Le joueur doit acheter **Croquettes Spatiales** à la buvette (prix Jordan) et les poser à côté de Snow. Snow se lève, mange et laisse le poster… et une **Relique Puante** en échange.
JOSÉ : Il paie en nature. C'est un business.

[ÉVÉNEMENT] Chaque poster donné à un supporter muté lui rend la voix. Exemples de répliques :
- SUPPORTER 1 : « … KC ? KC ! J'avais oublié comment on disait ! »
- SUPPORTER 2 : « Merci, mon gars. T'es qui ? » / JORDAN : « Un ancien. » / SUPPORTER 2 : « Ça se voit. »
- SUPPORTER 3 : « Je l'avais, ce poster, dans ma chambre ! Il est encore là d'ailleurs, à côté de celui de Kameto. »
- SUPPORTER 4 : « Faut qu'on chante, mais on n'est pas assez. On a besoin de lui. » *(Il montre Kevin sur le terrain.)*
- SUPPORTER 5 : « T'as pas une voiture, toi ? Tu peux me ramener après ? » / JORDAN : « … non. »

### SCÈNE 2-4 : Le Vestiaire

[DÉCOR] Un vestiaire désert. Un casier au nom de Kevin. Dedans : un diplôme d'ingénieur encadré, un poster de fusée, une maquette de satellite… et un post-it « *si on perd je pars sur Mars* ».
[ÉVÉNEMENT] Objet obtenu : **Écharpe de Kevin**. *Description : « Bleu KC. Elle sent encore les larmes de 2023. Et un peu le kebab. »*
[ÉVÉNEMENT] Au fond du casier, une photo de la Red Room en tribune à Düsseldorf. Tout le monde porte une écharpe, et Kevin est au centre, bras levés.
JOSÉ : C'était juste avant la demi-finale. On y croyait tellement.
JORDAN : C'est le week-end où vous êtes devenus la Red Room, non ?
JOSÉ : Ouais. On a perdu le match, et on a gagné un groupe. *(Un temps.)* C'est un bon échange, en vrai.
[ÉVÉNEMENT] *(Graine discrète.)* Au dos de la photo, un petit tampon : « *Photo : Ceyn* ».
[ÉVÉNEMENT] Mécanique « Ceyn. » :
JORDAN : Ceyn.
JOSÉ : Ceyn.
CLYDE : *(il ne connaît pas le gag, mais il le fait quand même, par politesse)* … Ceyn ?
[ÉVÉNEMENT] *(Ils rangent la photo et reprennent comme si de rien n'était.)*
[ÉVÉNEMENT] Objet obtenu : **Photo de Düsseldorf** (objet clé).

[ÉVÉNEMENT] *(Combat obligatoire à la sortie du vestiaire : 3 Sbires du Modérateur et 1 Abeille Videur.)*
ABEILLE VIDEUR : Bzz. Vestiaire réservé aux vainqueurs.
JOSÉ : Alors t'as rien à faire là non plus, t'es un videur.

### SCÈNE 2-5 : Le Billet

[DÉCOR] Une buvette tenue par une **Abeille Marchande** en tablier jaune.
ABEILLE MARCHANDE : Bzz. Bienvenue. Hot-dog en apesanteur, 12 €. *(Elle voit Jordan.)* Pour vous, 18 €. Vous avez une voiture.
JORDAN : Comment vous savez ça ?!
ABEILLE MARCHANDE : C'est écrit sur votre profil, monsieur. En gros.

[ÉVÉNEMENT] Le **Billet Düsseldorf 2023** est épinglé derrière le comptoir, comme un trophée.
ABEILLE MARCHANDE : Ça ? C'est un souvenir. Un supporter KC l'a laissé tomber en partant. Il pleurait trop pour le ramasser.
JOSÉ : C'était Kevin.
ABEILLE MARCHANDE : Je vous le donne… contre un **Miel Royal**. La Reine nous en prive, depuis qu'elle a gagné 413 fois. Elle garde tout pour elle.

> Le **Miel Royal** se trouve dans la **Ruche des Gradins**, un petit donjon de trois salles sous la tribune jaune. Ennemis : **Abeilles Ouvrières** (mono, faibles), **Frelons Ultras** (mono, statut *Poison*), **Chambreurs Jaunes** (debuff attaque : « T'as perdu en 2023 ! »). Le Miel Royal est dans un coffre au fond.

[ÉVÉNEMENT] *Tentative de drague de José (chapitre 2)*, dans la Ruche des Gradins. Une **Commentatrice** en tailleur révise ses fiches dans un coin. Jingle Pierre.
JOSÉ : *(ajuste son foulard)* Mademoiselle. Archéologue. Stylé. J'ai un rapport assez fort avec la balle, moi aussi.
COMMENTATRICE : *(sourit)* Oh, c'est mignon. Vous êtes supporter de qui ?
JOSÉ : Karmine, évidemment.
COMMENTATRICE : *(son sourire disparaît)* Je suis Vitality depuis 2016.
[ÉVÉNEMENT] Silence. José recule de trois pas, sans la quitter des yeux.
JOSÉ : Désolé. J'ai des principes.
[ÉVÉNEMENT] Jingle triste, mais *fier*.
[FLAG] `rateaux_jose += 1` *(Variante : celui-là, c'est José qui l'a mis.)*
JORDAN : C'est la première fois que c'est toi qui refuses.
JOSÉ : Il y a des choses plus importantes que l'amour, Jordan. Il y a la rivalité.

[ÉVÉNEMENT] Retour à la buvette avec le Miel Royal.
ABEILLE MARCHANDE : Bzz ! Marché conclu. Tenez. *(Elle tend le billet, puis hésite.)* Entre nous… on commence à s'ennuyer, à gagner tout le temps. 413 fois le même match. On aimerait bien voir autre chose.
[ÉVÉNEMENT] Objet obtenu : **Billet Düsseldorf 2023**.

### SCÈNE 2-6 : Le Kop Rouge chante

[ÉVÉNEMENT] Les trois objets sont rendus au chef du Kop Rouge, un supporter massif avec un tambour.
CHEF DU KOP : Les posters. L'écharpe. Le billet. *(Il serre l'écharpe contre lui.)* Ok. On est prêts. Mais c'est vous qui lancez.
[CHOIX]
1) Lancer « KC ! KC ! KC ! »
2) Rester digne, on a 29 ans.
*Si 2 :* JORDAN : « Non. J'ai une réputation. » · JOSÉ : « Laquelle ? Le vieux ? » · *(Retour au choix.)*
*Si 1 :*
JORDAN et JOSÉ : KC ! KC ! KC !
[SFX] Le tambour suit. Puis tout le Kop Rouge. Le stade tremble.
[MUSIQUE] Le thème du stade repart, sans saut de disque cette fois.
[ÉVÉNEMENT] La barrière jaune vole en éclats. Sur le terrain, Kevin s'arrête au milieu de son commentaire et lève la tête vers la tribune.

### SCÈNE 2-7 : Kevin

[ÉVÉNEMENT] L'équipe descend sur le terrain. La boucle se fige : la balle reste suspendue en l'air, juste avant le but décisif.
KEVIN : *(sans les regarder)* … angle d'approche 37,4 degrés…
JORDAN : KEVIN !
KEVIN : *(se fige, les regarde enfin)* … Jordan ? José ? *(Un temps.)* Vous êtes pas censés être là. Dans ma simulation, vous êtes dans les tribunes et vous pleurez.
JOSÉ : On pleurait pas.
KEVIN : José, j'ai 413 enregistrements de toi en train de pleurer.

[ÉVÉNEMENT] Jordan lui tend la **Photo de Düsseldorf**.
KEVIN : *(regarde la photo)* … on y croyait vraiment, hein.
JORDAN : Ouais.
KEVIN : Le pire, c'est que je jouais même pas. J'étais en tribune avec vous. Mais je l'ai recalculé tellement de fois que je sais plus ce que j'aurais dû faire. Les angles, les rebonds, le boost… J'ai simulé 14 millions de futurs. On perd dans tous. *(Un temps.)* Sauf un, où la balle est un sigma. Mais c'est pas réaliste.
JOSÉ : Mec, t'étais pas joueur. Tu pouvais rien faire.
KEVIN : C'est justement ça qui me rend fou.
JORDAN : Ce week-end-là, on a perdu un match. Mais la Red Room est née. Regarde la photo.
KEVIN : *(regarde encore. Il sourit enfin.)* … ouais. On a perdu le match. On a gagné une chambre avec une lumière rouge qui s'éteignait pas.
JOSÉ : Et des amis.
KEVIN : Et des amis. *(Il remet son casque.)* Bon. On le rejoue, ce match ? Pas pour changer le passé. Juste pour leur mettre une raclée une fois dans ma vie.
JORDAN : Une fois dans *la* vie. Moi, j'en ai déjà vécu plusieurs.
KEVIN : C'est vrai que t'as connu les premiers Worlds. Ceux en pierre.

[ÉVÉNEMENT] **Kevin rejoint l'équipe.** La boucle se brise comme une vitre. Le tableau d'affichage passe en **PROLONGATION**.
[ÉVÉNEMENT] Les abeilles des tribunes s'envolent, se rassemblent au centre du terrain et fusionnent dans un bourdonnement assourdissant.

### SCÈNE 2-8 : Boss : la Reine de la Ruche

[DÉCOR] Une gigantesque **reine abeille jaune et noire**, couronnée, avec des réacteurs de Rocket League à la place des ailes. Elle porte un maillot floqué « 4-2 ».
REINE DE LA RUCHE : BZZZ. 413 VICTOIRES. 413. VOUS POUVEZ PAS GAGNER. C'EST ÉCRIT DANS LES STATS.
KEVIN : Les stats, c'est moi qui les fais.
REINE DE LA RUCHE : … BZZ ?

> **Équipe pour ce combat** : Jordan, José, Kevin. Snow et Clyde sont en tribune.
>
> **Compétences de Kevin** : *Aerial* (mono, gros dégâts), *Démolition* (zone), *Calcul de Trajectoire* (buff précision et critique sur un allié), *Boost* (buff vitesse de l'équipe).

[COMBAT] **La Reine de la Ruche** (2 phases)
- **Phase 1 : Match 6**
  - *Dard Jaune* : mono.
  - *Essaim* : zone, faibles dégâts.
  - *Chambrage* : debuff attaque sur un allié (« BZZ, 2023 ! »).
  - Tous les 3 tours, elle invoque **2 Abeilles Supportrices** (adds faibles qui la soignent un peu à chaque tour).
  - Faiblesse : *Aerial* (dégâts ×1,5, « elle vole, c'est de la physique »).
- **Phase 2 (sous 50 % de PV) : Prolongation**
  - Événement scripté : le Kop Rouge chante « KC ! KC ! », et toute l'équipe reçoit un buff attaque pour le reste du combat.
  - REINE : « BZZ… CE BRUIT… ARRÊTEZ CE BRUIT… »
  - Elle gagne *Miel Royal* (soin de 15 % de ses PV, une seule fois) et *Pluie de Dards* (zone + statut *Poison*).
  - Réplique de Kevin au premier *Aerial* de la phase : « Angle d'approche : 37,4 degrés. Cette fois, ça rentre. »
- **Fin du combat** : cinématique. Kevin fait un dernier *Aerial* et traverse la Reine, qui explose en confettis jaunes. Le stade s'illumine en rouge.

### SCÈNE 2-9 : Après le match

[ÉVÉNEMENT] Le tableau d'affichage clignote : « **RED ROOM 1 – 0 VITALITY** ». Puis, juste en dessous, en petit : « *(Ce résultat n'a aucune valeur officielle.)* »
KEVIN : *(fixe l'écran)* Ça change rien à la vraie demi-finale.
JORDAN : Non.
KEVIN : *(sourit jusqu'aux oreilles)* Mais putain, ça fait du bien.
JOSÉ : Mec, t'as les yeux qui brillent.
KEVIN : C'est la poussière cosmique. *(Un temps.)* Et l'émotion. Mais surtout la poussière cosmique.

[ÉVÉNEMENT] Le Kop Rouge chante. Snow est au premier rang, il ne chante pas.
[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (2/7)**. Il tombe du ciel au centre du terrain.
[ÉVÉNEMENT] Objet obtenu : **Maillot de la Demi-Finale**, une armure pour Kevin. *Description : « Encore un peu humide de larmes. Défense +15. »*

KEVIN : Bon. Vous m'expliquez ce qui se passe ? Pourquoi on est dans Discord, pourquoi j'étais en boucle, et pourquoi y a un chat dans l'espace ?
JORDAN : Le serveur a été corrompu. Un bot, le Modérateur Fou, a tout pris en main. On doit retrouver tout le monde.
KEVIN : Ok. Donc c'est un problème d'infrastructure. *(Il réfléchit.)* J'adore les problèmes d'infrastructure. C'est comme une fusée, mais avec des gens.
JOSÉ : Et le chat ?
KEVIN : Le chat, c'est un problème qu'aucune science ne peut résoudre.

[ÉVÉNEMENT] Kevin regarde la Terre au loin.
KEVIN : Vous savez quoi ? Quand on sortira d'ici, je postule chez SpaceX. Pour de vrai.
JORDAN : Tu dis ça depuis trois ans.
KEVIN : Oui. Mais là, j'ai battu une reine abeille dans l'espace. J'ai de l'expérience terrain. *(Un temps.)* Ça, c'est du CV maxxing.

### SCÈNE 2-10 : Sortie du stade

[ÉVÉNEMENT] Retour vers le portail. Sur le chemin, un stand avec une banderole : « **VENEZ ESSAYER LEAGUE OF LEGENDS ! INSTALLATION EN 2 MINUTES !** », avec un PC allumé et un vendeur souriant.
VENDEUR : Monsieur ! Vous avez une tête de jungler !
KEVIN : Non.
VENDEUR : Juste une partie !
KEVIN : J'ai rien contre le jeu. Je veux juste pas y jouer. C'est différent.
JORDAN : Kevin, c'est juste un stand, tu passes devant.
KEVIN : Si je passe devant, il va m'installer le jeu. Ils font toujours ça.
[ÉVÉNEMENT] *(Kevin fait faire à toute l'équipe un petit détour derrière les gradins. Dix secondes. Il est satisfait.)*

[ÉVÉNEMENT] Sur la carte du monde, un nouveau message du Modérateur Fou défile dans le ciel :
[DISCORD] **#annonces** · 🔨 **Modérateur Fou** (BOT)
> @everyone Un utilisateur a quitté la boucle sans autorisation. Une enquête est ouverte. Rappel : le salon **#vocal-1** est fermé jusqu'à nouvel ordre. Toute respiration y est interdite.
> — *Approuvé par Camil (1,62 m)*

KEVIN : Toute respiration est interdite ? Mais Bidou…
JOSÉ : Bidou respire déjà à moitié en temps normal.
JORDAN : Alors on n'a pas de temps à perdre.

**FIN DU CHAPITRE 2**

---

### Récapitulatif chapitre 2 (pour l'intégration)
- **Recrue** : Kevin (combattant).
- **Quête principale** : « Le Kop Rouge » : 5 Posters KC, Écharpe de Kevin, Billet Düsseldorf 2023 (contre un Miel Royal trouvé dans la Ruche des Gradins).
- **Objets clés** : Photo de Düsseldorf, Fragment du Premier Message (2/7), Maillot de la Demi-Finale.
- **Flags** : `rateaux_jose` (variante « refus par principe »).
- **Mini-donjon** : la Ruche des Gradins (3 salles).
- **Boss** : la Reine de la Ruche (2 phases, attaques, invocations et soin standards).
- **Graines du twist** : le tampon « Photo : Ceyn » au dos de la photo de Düsseldorf.
- **Suite** : chapitre 3, #vocal-1 et Bidou.

---

## CHAPITRE 3 : Les Cimes Sans Air

> **Contexte** : le salon **#vocal-1** est devenu une montagne où le Modérateur Fou a coupé le son… et l'air. Bidou est coincé au sommet. Il essaie de chanter la **Chanson du Vocal**, la seule chose capable de rouvrir le salon, mais il n'a jamais assez de souffle pour la finir.
> **Moments clés** : l'ascension, Bidou vexé, les bonbonnes d'air, la chanson, le boss.
> **Équipe** : Jordan, José, Kevin, puis Bidou (4 personnages, l'équipe est complète pour la première fois).

### SCÈNE 3-1 : Le pied de la montagne

[DÉCOR] Une montagne grise et enneigée. Au sommet, une énorme icône de **haut-parleur barré 🔇** plantée comme un drapeau. Un panneau en bois à l'entrée du sentier : « **#vocal-1 — RESPIRATION INTERDITE. Par ordre du Modérateur.** » Le son est étouffé, comme sous l'eau.
[MUSIQUE] Thème des **Cimes** : flûte de montagne, mais les notes s'arrêtent avant la fin de chaque phrase musicale.

[ÉVÉNEMENT] Les bulles de dialogue sont **plus petites** dans cette zone, avec une police plus fine.
KEVIN : L'air se raréfie. À cette altitude, le taux d'oxygène baisse d'environ 30 %.
JOSÉ : Et Bidou est en haut ?
KEVIN : Avec ses poumons ? *(Il fait un calcul rapide sur ses doigts.)* Il respire à peu près 40 % d'un humain normal. En temps normal. Donc là…
JORDAN : Donc là, faut se dépêcher.
KEVIN : Donc là, c'est un miracle de la biologie. Skibidi miracle.

[ÉVÉNEMENT] *(Ascension : courte carte de montagne avec 2 ou 3 combats aléatoires.)*
> **Ennemis de la zone** : **Micros Coupés** (mono, statut *Muet*), **Larsens Sauvages** (zone, faibles), **Échos** (ils répètent la dernière attaque utilisée par l'équipe).

### SCÈNE 3-2 : Le refuge (tentative de drague de José)

[DÉCOR] Un petit refuge à mi-chemin. Une **Guide de Montagne** en doudoune violette, avec un petit rond rouge ⛔ flottant au-dessus de sa tête : statut Discord « **Ne pas déranger** ».
[ÉVÉNEMENT] Jingle Pierre.
JOSÉ : *(ajuste son foulard, essoufflé)* Mademoiselle. Archéologue. Stylé. Alpiniste, aussi, depuis… dix minutes.
GUIDE : *(montre le rond rouge au-dessus de sa tête, sans un mot)*
JOSÉ : … c'est quoi ?
KEVIN : Statut « Ne pas déranger ». Ses notifications sont coupées. Tu pourrais lui écrire un poème, techniquement, elle le recevrait jamais.
JOSÉ : *(très digne)* Le plus triste, c'est qu'elle saura jamais ce qu'elle a raté.
[FLAG] `rateaux_jose += 1`
[ÉVÉNEMENT] Elle vend des **Pastilles pour la Gorge** (soin de *Muet*). Prix Jordan : +30 %.

### SCÈNE 3-3 : Bidou

[DÉCOR] Le sommet. Un plateau battu par le vent, sous l'énorme 🔇. Au centre, Bidou, assis en tailleur, avec un luth. Il gratte une corde, inspire, ouvre la bouche…
BIDOU : *(chantant)* ♪ Oh vocal… ♪ *(inspire)* ♪ … ouvre-toi… ♪ *(inspire)* ♪ … pour que… ♪ *(inspire. Inspire. Rien ne vient.)*
[SFX] La note s'éteint. Le 🔇 au-dessus de lui brille plus fort, satisfait.
BIDOU : *(pose le luth, à bout de souffle)* … toujours… le même… couplet…

JORDAN : BIDOU !
BIDOU : *(se retourne lentement, l'air sombre)* … Ah. Vous voilà.
JOSÉ : On est venus te chercher !
BIDOU : Ça fait trois jours. *(Inspire.)* Trois jours que je chante seul sur une montagne. Sans air. Kevin, t'étais où ?
KEVIN : En boucle dans un stade spatial contre Vitality.
BIDOU : *(un temps)* … ok, ça, c'est une vraie excuse. *(Il se tourne vers Jordan.)* Et toi ?
JORDAN : Moi j'ai… euh… combattu une épingle géante.
BIDOU : Une épingle.
JORDAN : Une grosse épingle.

[CHOIX]
1) « Désolé Bidou, on est venus dès qu'on a pu. »
2) « T'aurais pu descendre, aussi. »
3) « Tu tiens le coup ? T'as pas l'air trop essoufflé. »

*Si 1 :*
BIDOU : *(radouci)* … ok. Ça va. *(Inspire.)* Je vous pardonne. Mais je note.
*Si 2 :*
BIDOU : *(se fige)* Descendre. *(Inspire.)* DESCENDRE ? Avec MES poumons ? Tu sais combien il y a de marches ?! *(Il se retourne et tourne le dos à l'équipe.)* C'est bon. J'ai compris. Je boude.
[FLAG] `bidou_vexe = true`
JOSÉ : *(chuchote)* Bravo.
KEVIN : *(chuchote)* Il va bouder au moins vingt minutes. J'ai des données.
*(Il faut lui reparler une deuxième fois. Il accepte, en grommelant.)*
BIDOU : … bon. Je boude, mais je vous aide. C'est pas pareil.
*Si 3 :*
BIDOU : *(plisse les yeux)* « Pas trop essoufflé » ? *(Inspire.)* Je suis au sommet d'une montagne sans air, Jordan. Je suis au MAXIMUM de l'essoufflement. Je suis le champion du monde de l'essoufflement.
JOSÉ : Et il est dans son élément.
BIDOU : *(un temps, puis il sourit malgré lui)* … un peu, ouais.

*(Convergence.)*
BIDOU : La Chanson du Vocal. Si je la chante en entier, le salon se rouvre, et tout le monde retrouve la voix. Le problème… c'est le dernier couplet. Il est trop long. J'ai jamais assez d'air.
KEVIN : Il te faut de l'oxygène en bouteille.
BIDOU : Le Modérateur a caché trois **Bonbonnes d'Air** sur la montagne. *(Inspire.)* Je les ai vues. J'avais juste pas le souffle d'aller les chercher.

> **Quête : « Trois Bonbonnes »** (quête à objets)
> - **Bonbonne 1** : dans une grotte, gardée par 3 Micros Coupés (combat).
> - **Bonbonne 2** : chez la Guide de Montagne. Elle est en « Ne pas déranger », donc on ne peut pas lui parler. Il faut **attendre** qu'elle passe « En ligne » : sortir du refuge et revenir. Elle la donne gratuitement : « Pour le petit monsieur qui chante. On l'entend depuis trois jours. Il chante faux, mais il chante. »
> - **Bonbonne 3** : au bord d'une falaise. Snow est assis dessus et refuse de bouger. Il faut lui donner des **Croquettes Spatiales** (il en reste du chapitre 2, ou la Guide en vend). Snow laisse la bonbonne… et une Relique Puante.
> BIDOU *(en voyant la Relique)* : Ah non. Non non. Pas ici. Il y a déjà pas d'air.

### SCÈNE 3-4 : La Chanson du Vocal

[ÉVÉNEMENT] Retour au sommet avec les trois bonbonnes. Bidou en prend une, inspire un grand coup, et reprend son luth.
BIDOU : *(chantant)* ♪ Oh vocal, ouvre-toi, pour que tous les copains… ♪
[ÉVÉNEMENT] Il enchaîne, de plus en plus fort. Le 🔇 au-dessus de lui commence à trembler.
BIDOU : ♪ … reviennent un soir, autour d'un bon barbecue… ♪ *(deuxième bonbonne)* ♪ … de Düsseldorf à Lyon, de Toulouse à Europa Park… ♪ *(troisième bonbonne)* ♪ … et au Portugal… ♪
JOSÉ : *(à voix basse)* Où j'étais désinvité.
JORDAN : *(à voix basse)* José, pas maintenant.
BIDOU : ♪ … et pour le dernier couplet… ♪ *(Il inspire. La bonbonne est vide.)* ♪ … pour… le… ♪
[SFX] La note se brise. Silence.
BIDOU : *(à genoux, désespéré)* … toujours. Toujours le dernier couplet.

[ÉVÉNEMENT] Un temps. Jordan s'avance.
JORDAN : Alors on le chante avec toi.
KEVIN : Mathématiquement, quatre paires de poumons, c'est plus que une.
JOSÉ : Et demie. Pour Bidou, on compte une demie.
BIDOU : *(regarde José)* … je suis vexé. *(Inspire.)* Mais allez-y.
[ÉVÉNEMENT] Les quatre chantent ensemble le dernier couplet, faux, mais fort.
TOUS : ♪ … ET LA RED ROOM CHANTERA, MÊME SANS AIR, MÊME SANS VOIX ! ♪
[SFX] Le 🔇 géant se fissure. Un vrai son revient : le vent, les oiseaux, le *bloop* lointain de quelqu'un qui se connecte.
[ÉVÉNEMENT] **Bidou rejoint l'équipe.**
BIDOU : *(ému, essoufflé)* C'était… *(inspire)* … pas mal. Pour des amateurs.

[ÉVÉNEMENT] Le 🔇 se détache de la montagne, tombe devant l'équipe, et se déplie en un énorme golem de métal noir.

### SCÈNE 3-5 : Boss : le Grand Mute

[DÉCOR] Un golem géant en forme de haut-parleur barré. À la place du visage, une barre de volume à zéro.
GRAND MUTE : … … … *(Ses bulles de dialogue sont vides.)*
KEVIN : Il dit rien.
JOSÉ : Il est muté. C'est le boss du silence, il est muté. C'est logique, en fait.
BIDOU : *(sort son luth)* Moi, je vais le faire parler.

> **Équipe** : Jordan, José, Kevin, Bidou.
> **Compétences de Bidou** : *Ballade (inachevée)* (soin mono), *Refrain Essoufflé* (soin de groupe), *Note Vexée* (mono), *Bouderie* (buff attaque sur soi, debuff défense sur soi).
> Rappel : sa jauge de magie s'appelle **Souffle**. Quand elle est vide, l'animation le montre plié en deux.

[COMBAT] **Le Grand Mute** (2 phases, avec interventions)

- **Phase 1**
  - *Coupure de Micro* : statut *Muet* sur un allié.
  - *Larsen* : zone.
  - *Silence Pesant* : debuff attaque sur toute l'équipe.

- **Intervention 1 (au tour 3) : Camil**
  [ÉVÉNEMENT] Un petit projecteur s'allume derrière le boss. Hologramme de **Camil**, debout sur sa caisse « NE PAS ENLEVER ».
  CAMIL : Je vois que vous faites du bruit dans mon serveur. Grand Mute, je t'accorde le rôle **Administrateur**.
  [ÉVÉNEMENT] Le Grand Mute reçoit un **buff défense** et une couronne dorée qui flotte au-dessus de lui.
  CAMIL : Et toi, Bidou. Franchement, tu chantes comme une cornemuse percée.
  BIDOU : *(se fige)* … pardon ?
  [ÉVÉNEMENT] Bidou reçoit automatiquement le statut *Vexé* : **buff attaque** pour le reste du combat.
  BIDOU : C'est bon. J'ai compris. *(Il serre son luth.)* Je vais te le chanter, ton dernier couplet.
  JORDAN : Camil, t'es sur une caisse.
  CAMIL : C'EST UN PIÉDESTAL. *(L'hologramme se coupe.)*
  *(Kevin ne réagit pas. Il fixe le boss.)*

- **Phase 2 (sous 50 % de PV)**
  - Le Grand Mute gagne *Mute Général* : statut *Muet* sur toute l'équipe (2 tours).
  - Et *Écrasement* : mono, gros dégâts.

- **Intervention 2 (au premier *Mute Général*) : un Sbire déserteur**
  [ÉVÉNEMENT] Un **Sbire du Modérateur** (petit marteau 🔨 sur pattes) arrive en courant sur le côté du terrain, regarde à gauche, à droite, et jette un objet à l'équipe.
  SBIRE : Pssst ! De la part du **Sergent**. *(Il chuchote.)* Il a dit : « Vive la lutte. »
  [ÉVÉNEMENT] Objet reçu : **Bonbonne d'Air Dorée**. Utilisée automatiquement : retire *Muet* à toute l'équipe et rend le Souffle de Bidou au maximum.
  JOSÉ : « Vive la lutte » ? Y a qu'une personne qui dit ça.
  JORDAN : … Robin.
  [ÉVÉNEMENT] Le sbire repart en courant.
  KEVIN : Robin est sergent chez le Modérateur ? *(Un temps.)* Robin ? Le gars qui fait grève quand on lui demande de ramener des chips ?
  *(Graine du chapitre 4.)*

- **Fin du combat**
  [ÉVÉNEMENT] Cinématique : Bidou se met devant l'équipe, inspire un très grand coup grâce à la Bonbonne Dorée et chante **une seule note**, longue, magnifique, interminable. La barre de volume du golem monte de 0 à 100, puis explose. Le Grand Mute se brise en mille petits 🔇.
  BIDOU : *(à bout de souffle, mais triomphant)* … ça… *(inspire)* … c'était… *(inspire)* … le dernier couplet.

### SCÈNE 3-6 : Le vocal rouvert

[DÉCOR] Le ciel de la montagne se dégage. Le son revient partout : vent, oiseaux, notifications.
[DISCORD] 🔊 **#vocal-1** · *réouvert*
[ÉVÉNEMENT] Dans la liste du vocal qui s'affiche à l'écran, quelques noms grisés s'allument un instant : *Robin (en service)*, *Florian (en colère)*, *Yanis (en train de manger)*… et **Ceyn** 🔇, connecté et muet, qui disparaît aussitôt.
[ÉVÉNEMENT] Mécanique « Ceyn. » :
JORDAN : Ceyn.
JOSÉ : Ceyn.
KEVIN : Ceyn.
BIDOU : *(inspire)* … Ceyn.
[ÉVÉNEMENT] *(Ils reprennent comme si de rien n'était.)*

[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (3/7)**.
[ÉVÉNEMENT] Objet obtenu : **Luth à Souffle Long**, une arme pour Bidou. *Description : « Accordé pour les chansons courtes. Très courtes. »*

BIDOU : Bon. Expliquez-moi tout. Le Modérateur, Camil, le serveur… et pourquoi le chat de Jordan me regarde comme ça ?
JORDAN : Il regarde tout le monde comme ça.
BIDOU : Il me regarde comme si je lui devais de l'argent.
JORDAN : *(un temps)* … tout le monde lui doit de l'argent, en fait. C'est moi qui paye les croquettes.

KEVIN : Si Robin est sergent chez le Modérateur, il est dans la **Caserne d'Annonces**.
JOSÉ : Robin, dans l'armée du Modérateur. Contre sa volonté. *(Il secoue la tête.)* Encore une fois.
BIDOU : Il doit être… *(inspire)* … furieux.
JORDAN : Furieux, et en train d'organiser une grève. Je le connais.

[ÉVÉNEMENT] Sur la carte du monde, un message du Modérateur Fou défile dans le ciel :
[DISCORD] **#annonces** · 🔨 **Modérateur Fou** (BOT)
> @everyone Le salon #vocal-1 a été rouvert illégalement. Les responsables sont priés de se présenter à la **Caserne d'Annonces** pour leur sanction. Rappel : la grève est interdite. *(Une grève est en cours.)*
> — *Approuvé par Camil (1,62 m)*

**FIN DU CHAPITRE 3**

---

### Récapitulatif chapitre 3 (pour l'intégration)
- **Recrue** : Bidou (combattant). L'équipe atteint 4 personnages.
- **Quête** : « Trois Bonbonnes » (grotte avec combat, PNJ en « Ne pas déranger », Snow).
- **Objets clés** : Fragment du Premier Message (3/7), Luth à Souffle Long, Pastilles pour la Gorge (soin de *Muet*).
- **Flags** : `bidou_vexe`, `rateaux_jose`.
- **Boss** : le Grand Mute (2 phases).
  - **Intervention 1** : hologramme de Camil, qui buffe le boss et vexe Bidou (buff attaque pour Bidou).
  - **Intervention 2** : un Sbire déserteur envoyé par « le Sergent » (Robin) donne la Bonbonne d'Air Dorée.
- **Graines** : Ceyn connecté muet dans la liste du vocal ; Robin annoncé comme sergent résistant.
- **Suite** : chapitre 4, la Caserne d'Annonces et Robin.
- ❓ *Quel barde Bidou joue-t-il (Bard, Seraphine, Sona…) ? On pourra en glisser une référence dans ses animations.*
