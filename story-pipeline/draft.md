# RED ROOM — Le Serveur Maudit
### Script v0.7 : Prologue + Chapitres 1 à 5

> **Conventions** (compatibles RPG Maker et Godot) :
> `[DÉCOR]` décor ou ambiance · `[MUSIQUE]` / `[SFX]` son · `[ÉVÉNEMENT]` action scriptée · `[CHOIX]` choix du joueur · `[COMBAT]` déclenche un combat · `[DISCORD]` faux message affiché dans l'interface Discord du jeu · `[FLAG]` variable de jeu.
> `NOM :` réplique · *(didascalie)*
>
> **Mécanique globale « Ceyn. »** : chaque fois que le nom de Ceyn s'affiche ou est prononcé, chaque membre présent de l'équipe dit « Ceyn. » dans une bulle, à tour de rôle et sans autre commentaire.

---

## PROLOGUE : « Free RP 100% legit »

### SCÈNE P-1 : Le QG, 03 h 47

[DÉCOR] Un appart plongé dans le noir. Un écran allumé, une Switch abandonnée sur le plateau de Mario Party, une forêt de canettes. Une odeur suspecte flotte.
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
[ÉVÉNEMENT] Snow se lève sur le clavier, se retourne… *prrrt*. Un petit nuage vert pixelisé.
JORDAN : … ah. Ah, ça pue.
KEVIN : C'est Snow ? Dis-lui que je l'aime. Et dis-lui d'arrêter de péter pendant qu'on joue, on a senti la dernière fois. À travers Discord. C'est scientifiquement impossible, mais on l'a senti.
JORDAN : Il fait ce qu'il veut, c'est le vrai propriétaire de l'appart.

JOSÉ : Alex a encore pas répondu de la soirée. Il veut pas nous voir, c'est officiel.
FLORIAN : Il est trop beau pour nous, voilà le problème.
[DISCORD] **Alex** : je suis là les gars je vous jure 😅
*(Il n'écrira plus rien du reste de la soirée.)*

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
CLYDE : Un chat ? Blanc ? *(Il frissonne.)* Tu parles de **la Bête Blanche** ? Elle est apparue cette nuit. Personne l'a vue en entier. On sait seulement qu'elle laisse derrière elle des… nuages.
JORDAN : Oh non.
CLYDE : Des nuages verts qui sentent la fin du monde.
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
- **Un mur de graffitis** : au milieu des tags (« GG », « nerf Yasuo », « Florian = pantacourt »), un nom écrit à la bombe : **Ceyn**.
  JORDAN : Ceyn.
  CLYDE : *(ne comprend pas, mais le dit quand même)* … Ceyn ?
  *(Ils repartent comme si de rien n'était.)*
- **Trace de la Bête Blanche n° 1** : une petite empreinte de patte et un nuage vert qui flotte encore. Les PNJ autour se bouchent le nez. Clyde : « Elle est passée par là. Il y a au moins deux heures. Et ça sent encore. »

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
[ÉVÉNEMENT] Il montre, avec un respect infini, un **bocal en verre** fermé, rempli d'une brume verte.
JOSÉ : Un gaz ancien. Préhistorique. Je l'ai trouvé coincé dans la strate de Düsseldorf. Il dégage une aura incroyable. Ça fait trois heures que je l'étudie et j'ai les yeux qui pleurent. C'est l'émotion, je pense.
JORDAN : José.
JOSÉ : Probablement le souffle sacré des fondateurs.
JORDAN : José, c'est un pet de Snow.
*(Long silence.)*
JOSÉ : *(regarde le bocal, regarde Jordan, regarde le bocal)* … ça reste une découverte.
CLYDE : C'est la Bête Blanche.
JOSÉ : La Bête Blanche, c'est SNOW ? *(Il lâche le bocal. Le couvercle saute.)*
[ÉVÉNEMENT] Un nuage vert envahit la tranchée.
JORDAN, JOSÉ, CLYDE : … ah. Ah, ça pue.

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
> - Snow peut intervenir dans certains combats scriptés (un pet, et tout le monde : « Ah, ça pue. »).
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

[ÉVÉNEMENT] *Trace de la Bête Blanche n° 2* : dans une des salles, un coffre qui fume en vert. L'ouvrir libère un nuage vert, et un message : « Le coffre était vide. Mais pas l'air. »
JOSÉ : Ah, ça pue. Il a fait ÇA dans un site classé ?!

#### 1-5-c : La Porte des Fondateurs
[DÉCOR] Une grande porte rouge. Au-dessus, une inscription : « *Seuls ceux qui savent d'où vient le nom peuvent entrer.* »
JOSÉ : C'est facile. *(Il pose la main sur la porte. Sa voix se fait plus douce.)* Düsseldorf. Les Worlds de Rocket League, 2023. Notre premier événement. On était dans la même chambre, les fondateurs. Moi, Kevin, Robin, Bidou… La chambre avait une lumière bizarre. Rouge. Toute la nuit, impossible de l'éteindre. Le lendemain, quelqu'un a dit « on est la Red Room », et c'est resté.
[ÉVÉNEMENT] *(Le joueur tape le mot de passe.)*
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
- **Phase 2 (sous 60 % de PV) : Désinvitation**
  - Le Gardien lance *Retrait d'Invitation* : statut *Banni* sur José (il ne peut pas agir pendant deux tours).
  - Réplique, GARDIEN : « VOUS N'ÊTES PLUS INVITÉ. »
  - JOSÉ *(à la fin du statut, furieux ; buff attaque pour le reste du combat)* : « Personne. Ne. Me. Désinvite. *(Il regarde Jordan.)* Plus jamais. »
  - JORDAN : « Je t'ai JAMAIS désinvité ! »
- **Phase 3 (sous 25 % de PV) : Intervention de Snow**
  - Le Gardien gagne *Suppression* : grosse attaque de zone.
  - Événement scripté au début de la phase : Snow saute de la vitrine, se poste devant le Gardien, lui tourne le dos et… *prrrt*. Un énorme nuage vert.
  - JORDAN, JOSÉ : « Ah, ça pue. »
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

> ❓ *À remplacer par le vrai premier échange si vous l'avez encore.*

JOSÉ : *(doucement)* Ça va paraître bizarre, mais… c'est le truc le plus beau que j'aie jamais déterré.
JORDAN : Plus beau que tes baskets ?
JOSÉ : *(longue réflexion)* … presque.

[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (1/7)**. *Description : « Un morceau de l'histoire de la Red Room. Il en faut sept pour ouvrir la Tour des Modérateurs. »*
[ÉVÉNEMENT] Snow se frotte enfin contre la jambe de Jordan. Ronronnement.
**Snow rejoint l'équipe (compagnon).** *Il suit Jordan sur la carte. De temps en temps, il s'arrête et refuse d'avancer pendant trois secondes. Parfois, sur la carte, il pète : petit nuage vert, et une bulle « Ah, ça pue » au-dessus d'un membre de l'équipe au hasard.*
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
CLYDE : *(tout petit)* La Base d'Annonces est par là. Le Stade Orbital par là. Et le vocal… plus personne ne respire là-haut depuis longtemps.
JOSÉ : Bidou va pas aimer ça.
JORDAN : Bidou aime déjà pas respirer en temps normal.
BIDOU *(voix lointaine, venue du ciel, très faible)* : … j'ai… *(inspire)* … entendu… *(inspire)* … je suis vexé…

[ÉVÉNEMENT] Ouverture de la carte du monde. Les salons **#rocket-league** et **#vocal-1** deviennent accessibles.

**FIN DU CHAPITRE 1**

---

### Récapitulatif chapitre 1 (pour l'intégration)
- **Recrues** : José (combattant), Snow (compagnon), Clyde (guide).
- **Objets clés** : Fragment du Premier Message (1/7).
- **Flags** : `snow_a_clique`, `jose_aveu_portugal`, `rateaux_jose`, `quete_bete_blanche`.
- **Ceyn** : un seul graffiti sur un mur de Généralia (gag uniquement, aucun indice).

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
[ÉVÉNEMENT] Le joueur doit acheter **Croquettes Spatiales** à la buvette (prix Jordan) et les poser à côté de Snow. Snow se lève, mange, laisse le poster… et pète en partant.
JOSÉ : Ah, ça pue. Il paie en nature, ton chat.

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
[ÉVÉNEMENT] Sur le banc du vestiaire, un nom gravé au couteau parmi d'autres : « **Ceyn** ».
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
- **Ceyn** : nom gravé sur un banc du vestiaire (gag uniquement).
- **Suite** : chapitre 3, #vocal-1 et Bidou.

---

## CHAPITRE 3 : Les Cimes Sans Air

> **Contexte** : le salon **#vocal-1** est devenu une montagne où le Modérateur Fou a coupé le son… et l'air. Bidou, métalleux aux cheveux longs, est coincé au sommet avec sa guitare électrique. Seul un vrai **riff de metal** avec un **cri final** peut faire sauter le silence et rouvrir le vocal. Le problème : le cri final est long, et Bidou manque d'air.
> **Moments clés** : l'ascension et l'énigme de glace, le Yéti Roadie et son quiz, Bidou, le riff, le boss.
> **Équipe** : Jordan, José, Kevin, puis Bidou (4 personnages, l'équipe est complète pour la première fois).

### SCÈNE 3-1 : Le pied de la montagne

[DÉCOR] Une montagne grise et enneigée. Au sommet, une énorme icône de **haut-parleur barré 🔇** plantée comme un drapeau. Un panneau en bois à l'entrée du sentier : « **#vocal-1 — RESPIRATION INTERDITE. Par ordre du Modérateur.** » Le son est étouffé, comme sous l'eau.
[MUSIQUE] Thème des **Cimes** : riff de guitare saturée très lointain, comme joué à travers un oreiller.

KEVIN : L'air se raréfie. À cette altitude, le taux d'oxygène baisse d'environ 30 %.
JOSÉ : Et Bidou est en haut ?
KEVIN : Avec ses poumons ? *(Il fait un calcul rapide sur ses doigts.)* En temps normal, il est déjà à la limite. Donc là…
JORDAN : Donc là, faut se dépêcher.
KEVIN : Donc là, c'est un miracle de la biologie. Skibidi miracle.
JOSÉ : Vous entendez ? On dirait… une guitare.
JORDAN : C'est lui. Y a que Bidou pour faire du metal en haut d'une montagne sans air.

> **Ennemis de la zone** : **Micros Coupés** (mono, statut *Muet*), **Larsens Sauvages** (zone, faibles), **Bouchons d'Oreille** (debuff attaque).

### SCÈNE 3-2 : Le Lac Gelé (énigme de dalles)

[DÉCOR] Un lac gelé barre le sentier. De l'autre côté, la suite du chemin. Sur la glace, des rochers éparpillés.
> **Énigme de glace** (classique RPG) : sur la glace, l'équipe glisse en ligne droite jusqu'à toucher un rocher. Il faut trouver le bon enchaînement de directions pour atteindre l'autre rive. Une erreur renvoie au point de départ.
KEVIN : C'est un problème de trajectoire. Laissez-moi faire. *(Il glisse droit dans le décor et revient au départ.)* … j'avais pas pris en compte le frottement.
JOSÉ : Il y a pas de frottement, c'est de la glace.
KEVIN : C'est exactement ce que j'avais pas pris en compte.

[ÉVÉNEMENT] *(Optionnel)* Sur un rocher au milieu du lac, quelqu'un a écrit dans la neige, en grosses lettres : **Ceyn**.
JORDAN : Ceyn.
JOSÉ : Ceyn.
KEVIN : Ceyn.
*(Ils continuent à glisser comme si de rien n'était.)*

### SCÈNE 3-3 : Le Yéti Roadie (quiz)

[DÉCOR] Un passage étroit entre deux falaises, bloqué par une pile de flight cases. Assis dessus, un énorme **Yéti** en t-shirt de groupe de metal noir, bracelets à clous, casque de chantier.
YÉTI ROADIE : HALTE. Personne monte au concert sans pass backstage.
JORDAN : Quel concert ?
YÉTI ROADIE : Le chevelu, là-haut. Ça fait trois jours qu'il essaie de jouer. Il joue fort, mais il s'arrête toujours au moment du cri. *(Il essuie une larme.)* Moi je suis son roadie, maintenant. J'ai décidé tout seul.
JOSÉ : Et comment on a un pass ?
YÉTI ROADIE : Quiz. Trois questions. Si vous connaissez pas le chevelu, vous montez pas.

> **Quiz** (une mauvaise réponse déclenche un combat contre 2 Larsens Sauvages, puis on recommence la question).
> 1. **« Quel champion le chevelu joue sur LoL ? »** — Bard ✅ · Yuumi · Teemo
>    *(Si Yuumi :)* YÉTI : « YUUMI ? Tu veux qu'il te frappe ? »
> 2. **« Qu'est-ce qu'il écoute ? »** — Du metal ✅ · De la K-pop · Des podcasts sur la respiration
>    *(Si podcasts :)* KEVIN : « … c'est pas faux, il en aurait besoin. » · YÉTI : « MAUVAISE RÉPONSE. Mais drôle. »
> 3. **« Comment s'appelle le groupe ? »** — La Red Room ✅ · La Blue Room · Les Amis de Camil
>    *(Si Les Amis de Camil :)* YÉTI : « Ça existe pas, ça. Personne n'est ami avec lui. »
> ❓ *Questions à remplacer ou compléter avec de vraies private jokes sur Bidou.*

YÉTI ROADIE : … trois sur trois. Vous êtes de vrais fans. *(Il pousse les flight cases.)* Allez-y. Et si vous le voyez manquer d'air… soyez gentils. Il est susceptible.
[ÉVÉNEMENT] *Tentative de drague de José (chapitre 3)*. Derrière les flight cases, une **Fan de Metal** en veste à patchs attend le concert. Jingle Pierre.
JOSÉ : *(ajuste son foulard)* Mademoiselle. Archéologue. Stylé. Grand amateur de… musique forte.
FAN DE METAL : Ah ouais ? T'écoutes quoi ?
JOSÉ : *(un temps beaucoup trop long)* … du rock. Genre… du gros rock. *(Il fait le signe des cornes du metal… avec le pouce sorti.)*
FAN DE METAL : *(regarde sa main)* … avec le pouce, c'est « je t'aime » en langue des signes, ça.
JOSÉ : *(regarde sa main)* … et alors ? Ça marche aussi.
[ÉVÉNEMENT] Elle s'éloigne. Jingle triste, version guitare saturée.
[FLAG] `rateaux_jose += 1`

### SCÈNE 3-4 : Bidou

[DÉCOR] Le sommet. Un plateau battu par le vent, sous l'énorme 🔇. Au centre, sur une petite scène improvisée en rochers, **Bidou** : cheveux longs au vent, veste en cuir, guitare électrique branchée sur un ampli qui fume. Il joue un riff, très fort, très bien. Puis il s'approche du micro pour le cri final…
BIDOU : *(cri metal)* RAAAAAAAAAA— *(il s'arrête net, plié en deux)* … *(inspire)* … *(inspire)* … aaaah.
[SFX] Le riff s'éteint. Le 🔇 au-dessus de lui brille plus fort, satisfait.
BIDOU : *(à bout de souffle, les mains sur les genoux)* … toujours… *(inspire)* … au même moment…

JORDAN : BIDOU !
BIDOU : *(se redresse lentement, rejette ses cheveux en arrière, l'air sombre)* … Ah. Vous voilà.
JOSÉ : On est venus te chercher !
BIDOU : Ça fait trois jours. *(Inspire.)* Trois jours que je joue seul sur une montagne. Sans air. Kevin, t'étais où ?
KEVIN : En boucle dans un stade spatial contre Vitality.
BIDOU : *(un temps)* … ok, ça, c'est une vraie excuse. *(Il se tourne vers Jordan.)* Et toi ?
JORDAN : Moi j'ai… euh… combattu une épingle géante.
BIDOU : Une épingle.
JORDAN : Une grosse épingle.

[CHOIX]
1) « Désolé Bidou, on est venus dès qu'on a pu. »
2) « T'aurais pu descendre, aussi. »
3) « Joli riff. Dommage pour la fin. »

*Si 1 :*
BIDOU : *(radouci)* … ok. Ça va. *(Inspire.)* Je vous pardonne. Mais je note.
*Si 2 :*
BIDOU : *(se fige)* Descendre. *(Inspire.)* DESCENDRE ? Avec MES poumons ? Avec un AMPLI ? *(Il se retourne et tourne le dos à l'équipe.)* C'est bon. J'ai compris. Je boude.
[FLAG] `bidou_vexe = true`
JOSÉ : *(chuchote)* Bravo.
KEVIN : *(chuchote)* Il va bouder au moins vingt minutes. J'ai des données.
*(Il faut lui reparler une deuxième fois.)*
BIDOU : … bon. Je boude, mais je vous aide. C'est pas pareil.
*Si 3 :*
BIDOU : *(plisse les yeux)* « Dommage pour la fin » ? *(Inspire.)* Tu crois que c'est facile de faire un cri de metal à 4 000 mètres, sans air, avec MES poumons ?
JOSÉ : Il marque un point.
BIDOU : *(un temps, puis il sourit malgré lui)* … mais ouais. C'est dommage pour la fin.

*(Convergence.)*
BIDOU : Le silence de ce salon, c'est le Modérateur. Pour le briser, il faut le faire sauter. Un riff, plein volume, et un cri final assez long pour faire péter ce 🔇. Le riff, je l'ai. *(Inspire.)* Le cri… j'arrive jamais au bout.
KEVIN : Et si on criait avec toi ?
BIDOU : *(les regarde un par un)* … vous savez crier en metal ?
JOSÉ : Non.
JORDAN : J'ai 29 ans, Bidou, je crie quand je me lève du canapé.
BIDOU : … ça ira.

### SCÈNE 3-5 : Le Riff du Vocal

[ÉVÉNEMENT] Bidou rebranche sa guitare. Jordan, José et Kevin se placent derrière lui comme des choristes très mal préparés.
[MUSIQUE] Le riff démarre, cette fois à plein volume. La neige tremble.
BIDOU : *(au micro)* RED ROOOOOOOM— *(inspire)* — OOOOOM— *(inspire)* — *(il lève la main, plié en deux)* … deux secondes… *(inspire)*
JOSÉ : On attend, on attend.
KEVIN : *(au public imaginaire)* Petite pause technique.
BIDOU : *(se redresse)* … c'est bon. *(Il regarde l'équipe.)* Maintenant. Tous ensemble.
TOUS : *(cri faux, horrible, mais énorme)* RAAAAAAAAAAAAAAAAAAAAAAA !
[SFX] Le 🔇 géant se fissure. Un vrai son revient : le vent, l'écho du riff, le *bloop* lointain de quelqu'un qui se connecte.
[ÉVÉNEMENT] **Bidou rejoint l'équipe.**
BIDOU : *(essoufflé, mais ravi)* C'était… *(inspire)* … immonde. *(Il sourit.)* J'adore.
[ÉVÉNEMENT] Snow, qui était sur l'ampli, saute au sol, s'étire… *prrrt*.
BIDOU : Ah. Ah non. Ça pue. *(Inspire.)* Et j'ai PAS l'air pour ça.

[ÉVÉNEMENT] Le 🔇 se détache de la montagne, tombe devant l'équipe, et se déplie en un énorme golem de métal noir.

### SCÈNE 3-6 : Boss : le Grand Mute

[DÉCOR] Un golem géant en forme de haut-parleur barré. À la place du visage, une barre de volume à zéro.
GRAND MUTE : … … … *(Ses bulles de dialogue sont vides.)*
KEVIN : Il dit rien.
JOSÉ : Il est muté. C'est le boss du silence, il est muté. C'est logique, en fait.
BIDOU : *(fait craquer ses doigts sur le manche)* Moi, je vais le faire parler.

> **Équipe** : Jordan, José, Kevin, Bidou.
> **Compétences de Bidou** (métalleux, joue Bard) : *Riff Saturé* (mono), *Headbang* (zone), *Carillons* (soin de groupe, clin d'œil aux carillons de Bard), *Destin Figé* (statut *Étourdi* sur tous les ennemis, la ult de Bard).
> Sa jauge de magie s'appelle **Souffle**. Quand elle est vide, l'animation le montre plié en deux, les mains sur les genoux.

[COMBAT] **Le Grand Mute** (2 phases, avec interventions)

- **Phase 1**
  - *Coupure de Micro* : statut *Muet* sur un allié.
  - *Larsen* : zone.
  - *Silence Pesant* : debuff attaque sur toute l'équipe.

- **Intervention 1 (au tour 3) : Camil**
  [ÉVÉNEMENT] Un petit projecteur s'allume derrière le boss. Hologramme de **Camil**, debout sur sa caisse « NE PAS ENLEVER ».
  CAMIL : Je vois que vous faites du bruit dans mon serveur. Grand Mute, je t'accorde le rôle **Administrateur**.
  [ÉVÉNEMENT] Le Grand Mute reçoit un **buff défense**, et une couronne dorée flotte au-dessus de lui.
  CAMIL : Et toi, Bidou. Ton metal, c'est du bruit. Et coupe-toi les cheveux, on dirait une serpillière.
  BIDOU : *(se fige)* … pardon ?
  [ÉVÉNEMENT] Bidou reçoit automatiquement le statut *Vexé* : **buff attaque** pour le reste du combat.
  BIDOU : C'est bon. J'ai compris. *(Il monte le volume de l'ampli au maximum.)*
  JORDAN : Camil, t'es sur une caisse.
  CAMIL : C'EST UN PIÉDESTAL. *(L'hologramme se coupe.)*
  *(Kevin ne réagit pas. Il fixe le boss.)*

- **Phase 2 (sous 50 % de PV)**
  - Le Grand Mute gagne *Mute Général* : statut *Muet* sur toute l'équipe (2 tours).
  - Et *Écrasement* : mono, gros dégâts.

- **Intervention 2 (au premier *Mute Général*) : un Sbire déserteur**
  [ÉVÉNEMENT] Un **Sbire du Modérateur** (petit marteau 🔨 sur pattes) arrive en courant sur le côté du terrain, regarde à gauche, à droite, et jette un objet à l'équipe.
  SBIRE : Pssst ! De la part du **Sergent**. *(Il chuchote.)* Il a dit : « Vive la lutte. »
  [ÉVÉNEMENT] Objet reçu : **Bonbonne d'Air Dorée**. Utilisée automatiquement : retire *Muet* à toute l'équipe et remplit le Souffle de Bidou.
  BIDOU : *(inspire à fond, les yeux fermés)* … oh. C'est ça, respirer ? *(Inspire encore.)* C'est incroyable. Je comprends pourquoi vous faites ça tout le temps.
  JOSÉ : « Vive la lutte » ? Y a qu'une personne qui dit ça.
  JORDAN : … Robin.
  [ÉVÉNEMENT] Le sbire repart en courant.
  KEVIN : Robin est sergent chez le Modérateur ? Robin ? Le gars qui fait grève quand on lui demande de ramener des chips ?
  *(Annonce du chapitre 4.)*

- **Fin du combat**
  [ÉVÉNEMENT] Cinématique : Bidou, plein d'air pour la première fois de sa vie, monte sur l'ampli, lance *Destin Figé* et pousse un cri de metal **entier**, sans pause. La barre de volume du golem monte de 0 à 100, puis explose. Le Grand Mute se brise en mille petits 🔇.
  BIDOU : *(il retombe, l'air de la bonbonne est fini)* … ça… *(inspire)* … c'était… *(inspire)* … mon premier cri complet. *(Inspire.)* Quelqu'un a filmé ?
  KEVIN : Non.
  BIDOU : … je suis vexé.

### SCÈNE 3-7 : Le vocal rouvert

[DÉCOR] Le ciel de la montagne se dégage. Le son revient partout : vent, oiseaux, et au loin le Yéti Roadie qui applaudit.
[DISCORD] 🔊 **#vocal-1** · *réouvert*
[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (3/7)**.
[ÉVÉNEMENT] Objet obtenu : **Médiator de Bard**, une arme pour Bidou. *Description : « Gravé d'un petit carillon. Il fait "meep" quand on gratte. »*

BIDOU : Bon. Expliquez-moi tout. Le Modérateur, Camil, le serveur… et pourquoi le chat de Jordan me regarde comme ça ?
JORDAN : Il regarde tout le monde comme ça.
BIDOU : Il me regarde comme si je lui devais de l'argent.
JORDAN : *(un temps)* … tout le monde lui doit de l'argent, en fait. C'est moi qui paye les croquettes.

KEVIN : Si Robin est sergent chez le Modérateur, il est dans la **Base d'Annonces**.
JOSÉ : Robin, dans l'armée du Modérateur. Contre sa volonté. *(Il secoue la tête.)* Encore une fois.
BIDOU : Il doit être… *(inspire)* … furieux.
JORDAN : Furieux, et en train d'organiser une grève. Je le connais.

[ÉVÉNEMENT] Sur la carte du monde, un message du Modérateur Fou défile dans le ciel :
[DISCORD] **#annonces** · 🔨 **Modérateur Fou** (BOT)
> @everyone Le salon #vocal-1 a été rouvert illégalement. Les responsables sont priés de se présenter à la **Base d'Annonces** pour leur sanction. Rappel : la grève est interdite. *(Une grève est en cours.)*
> — *Approuvé par Camil (1,62 m)*

**FIN DU CHAPITRE 3**

---

### Récapitulatif chapitre 3 (pour l'intégration)
- **Recrue** : Bidou (combattant, métalleux, joue Bard). L'équipe atteint 4 personnages.
- **Énigmes** : le Lac Gelé (dalles de glace) et le quiz du Yéti Roadie.
- **Objets clés** : Fragment du Premier Message (3/7), Médiator de Bard.
- **Flags** : `bidou_vexe`, `rateaux_jose`.
- **Boss** : le Grand Mute (2 phases).
  - **Intervention 1** : hologramme de Camil, qui buffe le boss et vexe Bidou (buff attaque pour Bidou).
  - **Intervention 2** : un Sbire déserteur envoyé par « le Sergent » Robin donne la Bonbonne d'Air Dorée.
- **Ceyn** : écrit dans la neige sur le Lac Gelé (gag uniquement).
- **Suite** : chapitre 4, la Base d'Annonces et Robin.

---

## CHAPITRE 4 : La Base d'Annonces

> **Contexte** : le salon **#annonces** est devenu une **base aérienne militaire**. Dans #annonces, seuls les modérateurs ont le droit de parler, alors tout le monde obéit en silence. Robin y a été affecté comme **aviateur**, avec un poste à responsabilité : il commande une escouade de Sbires du Modérateur. À contrecœur, évidemment. La nuit, il travaille en cachette sur sa **thèse**. Et il prépare une **grève générale**.
> **Moments clés** : l'arrivée sans droit de parole, l'infiltration, Robin, la tour de contrôle (interrupteurs), le discours de grève (choix de dialogue), le boss.
> **Équipe** : Jordan, José, Kevin, Bidou, puis Robin (le système de réserve s'active).

### SCÈNE 4-1 : Interdit de parler

[DÉCOR] Une base aérienne grise sous un ciel orange. Des pistes, des hangars, une tour de contrôle. Partout, des haut-parleurs. Des **avions de papier géants** traversent le ciel en traînant des banderoles : « RAPPEL DU RÈGLEMENT », « MISE À JOUR DES CONDITIONS D'UTILISATION ».
[MUSIQUE] Thème de la **Base** : marche militaire, jouée au kazoo.

JORDAN : Bon. On cherche Robin, on…
[ÉVÉNEMENT] La bulle de Jordan est remplacée par une boîte grise :
> *Vous n'avez pas la permission d'envoyer des messages dans ce salon.*
JOSÉ : Qu'est-ce que…
> *Vous n'avez pas la permission d'envoyer des messages dans ce salon.*
KEVIN : *(lève un doigt, ouvre la bouche, la referme)*
BIDOU : *(inspire très fort pour crier)*
> *Vous n'avez pas la permission d'envoyer des messages dans ce salon.*
BIDOU : *(boude en silence)*

[ÉVÉNEMENT] Clyde se met devant l'équipe.
CLYDE : Ah, moi j'ai le droit. Je suis un bot. *(Il se racle la gorge électronique.)* Mes amis vous font dire qu'ils cherchent un certain Robin, et que le petit chevelu est vexé.
[ÉVÉNEMENT] Clyde devient **l'interprète** de l'équipe pendant toute la première partie du chapitre. *(Ça ne dure que deux ou trois scènes : le gag doit rester court.)*

> **Ennemis de la zone** : **Sbires du Modérateur** (mono, statut *Muet*), **Avions de Papier** (mono, rapides), **Haut-Parleurs** (zone, statut *Confusion* : « ANNONCE IMPORTANTE ! »).

### SCÈNE 4-2 : L'infiltration

[DÉCOR] L'entrée de la base. Deux **Sbires de garde** (petits marteaux 🔨 sur pattes) bloquent la barrière.
SBIRE DE GARDE : Civils interdits. Uniforme obligatoire.
CLYDE : *(traduit)* Ils disent qu'il nous faut des uniformes.
[ÉVÉNEMENT] *(Mini-objectif : la laverie de la base, juste à côté. Une machine à laver géante tourne. Il faut attendre la fin du cycle et récupérer 4 uniformes. Un combat contre 2 Haut-Parleurs dans la laverie.)*
[ÉVÉNEMENT] L'équipe enfile les uniformes, tous beaucoup trop grands ou trop petits. Celui de José s'arrête au mollet.
JOSÉ : *(réussit enfin à parler, car le gag de l'interdiction s'arrête dès qu'ils sont en uniforme)* … non. Non non non. Le pantalon tombe PAS sur la paire. Il tombe nulle part. Il s'arrête en plein milieu de ma jambe.
KEVIN : C'est un pantacourt.
JOSÉ : Je suis pas Florian !
BIDOU : Je peux parler ? *(Inspire.)* JE PEUX PARLER ! *(Inspire.)* … j'avais rien à dire, en fait.
SBIRE DE GARDE : *(regarde l'équipe de haut en bas)* … ok. Passez, soldats.
[ÉVÉNEMENT] *Snow*, qui n'a pas d'uniforme, passe tranquillement entre les jambes des gardes. Personne ne dit rien. *prrrt.*
SBIRE DE GARDE : … ah. Ça pue.

### SCÈNE 4-3 : Robin

[DÉCOR] Un hangar plongé dans la pénombre. Un avion de chasse en carton, une rangée de lits de camp. Dans un coin, une petite lampe de bureau : **Robin**, en combinaison d'aviateur, galons sur l'épaule, tape à toute vitesse sur un vieil ordinateur portable. Sur un post-it collé à l'écran : « *Thèse — chapitre 3 — NE PAS SE FAIRE GRILLER* ».
[ÉVÉNEMENT] Sur le mur, une photo de **Emma**, punaisée à côté d'un planning de garde. Un petit cœur dessiné au feutre dessus.

ROBIN : *(sans lever les yeux)* Si c'est pour l'inspection, je dors. Officiellement, je dors.
JORDAN : Robin.
ROBIN : *(lève la tête, ferme l'ordi d'un coup sec)* … Jordan ? *(Il voit les uniformes.)* Pourquoi vous êtes déguisés en soldats ?
JOSÉ : Pour te chercher. Et j'ai un pantacourt, Robin. Un PANTACOURT.
ROBIN : *(se lève, très ému, les serre tous dans ses bras)* Les gars… *(Il recule, regarde Bidou.)* Ça a marché, la bonbonne ?
BIDOU : J'ai respiré, Robin. *(Inspire.)* Pour la première fois de ma vie, j'ai respiré.
ROBIN : *(fier)* Zingis.
KEVIN : Zingis.
JORDAN : Zingis.
CLYDE : *(perdu)* … ça veut dire quoi ?
JORDAN : Tout. Et rien.
ROBIN : C'est Jordan qui l'a inventé. Moi je l'ai juste… perfectionné.

[ÉVÉNEMENT] Robin rouvre son ordinateur pour leur montrer. Titre du document : « *Thèse — Peut-on remplacer un Modérateur par un LLM ? (Spoiler : oui, et en mieux)* ».
ROBIN : Je devais travailler sur l'IA. J'ai fini aviateur, chef d'escouade, à surveiller des marteaux sur pattes. Alors la nuit, j'écris ma thèse. Et le jour, je prépare la révolution.
KEVIN : Tu fais les deux en même temps ?
ROBIN : J'ai un poste à responsabilités. Je suis très organisé.
[ÉVÉNEMENT] *(Gag, optionnel)* Si le joueur examine la bibliographie de la thèse : « *Ceyn et al. (2019). Pourquoi personne ne répond dans #général. Éditions Inactives.* »
ROBIN : Ceyn.
JORDAN : Ceyn.
JOSÉ : Ceyn.
KEVIN : Ceyn.
BIDOU : *(inspire)* Ceyn.
*(Robin referme l'ordi comme si de rien n'était.)*

ROBIN : Bon. Écoutez. Les sbires du Modérateur, je les connais. Ils sont exploités. Pas de pause, pas de congés, ils bannissent des gens 24 h sur 24. Ils veulent faire grève. Mais ils ont peur. Il leur faut un **signal**.
JORDAN : Quel signal ?
ROBIN : Les lumières de la piste. Si on les allume pour écrire le mot de code, tous les sbires de la base le verront. Et ils poseront leurs marteaux.
JOSÉ : C'est quoi, le mot de code ?
ROBIN : *(sourit)* À ton avis.
TOUS : … zingis.
ROBIN : Personne au Modérateur ne pourra le décoder. Ça veut rien dire.

### SCÈNE 4-4 : La Tour de Contrôle (interrupteurs)

[DÉCOR] Le sommet de la tour de contrôle. Une grande vitre donne sur la piste. Un tableau de **6 interrupteurs** commande les rampes lumineuses de la piste.
> **Énigme d'interrupteurs** : chaque interrupteur allume une rampe de lumières sur la piste et en inverse une ou deux voisines. Il faut trouver la combinaison qui écrit **ZINGIS** en lumières. Un indice est affiché en permanence sur la vitre : la vue de la piste, avec les lettres qui se forment au fur et à mesure.
> Au bout de 3 essais ratés, Kevin propose la solution : « C'est de l'algèbre booléenne. J'ai fait ça en L2. Enfin, j'ai dormi pendant, mais j'ai fait ça. »

[ÉVÉNEMENT] *Tentative de drague de José (chapitre 4)*. Dans la tour, une **Pilote de Chasse** en combinaison, casque sous le bras, vérifie la météo. Jingle Pierre.
JOSÉ : *(ajuste le col de son uniforme trop court)* Mademoiselle. Archéologue. Stylé. Soldat, aussi, depuis… vingt minutes.
PILOTE : Désolée, je décolle dans deux minutes.
JOSÉ : Je peux venir ?
PILOTE : C'est un monoplace.
[ÉVÉNEMENT] Par la vitre, on la voit monter dans un jet et décoller à toute vitesse. Jingle triste, couvert par le bruit du réacteur.
JOSÉ : *(regarde le ciel)* Elle a littéralement pris la fuite.
[FLAG] `rateaux_jose += 1`

[ÉVÉNEMENT] Une fois l'énigme résolue, la piste s'illumine. Vu du ciel, en lettres de lumière géantes : **ZINGIS**.
[SFX] Partout dans la base, des petits *clong* : les sbires posent leurs marteaux, un par un.
ROBIN : *(à la fenêtre, ému)* Ça y est. Ils ont vu.

### SCÈNE 4-5 : Le Discours (choix de dialogue)

[DÉCOR] La grande cour de la base. Des centaines de Sbires du Modérateur rassemblés, marteaux au sol, hésitants. Robin monte sur une caisse.
JOSÉ : *(chuchote)* Lui aussi il monte sur une caisse ?
JORDAN : *(chuchote)* Lui, c'est pour qu'on le voie. Pas pour paraître grand.
ROBIN : Camarades sbires !
SBIRES : … ?
ROBIN : Depuis des semaines, on bannit, on mute, on kick. Sans pause. Sans merci. Sans tickets resto.
SBIRE : *(timide)* C'est vrai qu'on a jamais de tickets resto…

> **Choix de dialogue** : Robin demande à Jordan de l'aider à convaincre la foule. Le joueur choisit **3 slogans** parmi 6. Chaque bon slogan fait monter une jauge « Motivation des Sbires ». Il faut 3 bons slogans sur 3 ; en cas d'erreur, la foule hue et on recommence le choix.
> - « Pas de ban sans pause café ! » ✅
> - « Le marteau, c'est pour les clous, pas pour les gens ! » ✅
> - « Zingis pour tous ! » ✅
> - « Travaillez plus ! » ❌ *(ROBIN : « JORDAN. »)*
> - « Achetez Discord Nitro ! » ❌ *(SBIRE : « On est déjà payés en Nitro, c'est le problème. »)*
> - « Vive Camil ! » ❌ *(Silence glacial. Un sbire jette une tomate.)*

[ÉVÉNEMENT] Après trois bons slogans, la foule explose.
SBIRES : GRÈVE ! GRÈVE ! GRÈVE !
ROBIN : *(lève le poing)* VIVE LA LUTTE !
[ÉVÉNEMENT] **Robin rejoint l'équipe.**
> **Système de réserve** : CLYDE : « Vous êtes cinq, mais le serveur limite les combats à quatre. Le cinquième attend sur le banc et peut être échangé entre les tours. » JOSÉ : « Comme au barbecue. Il y a jamais assez de chaises. »

[SFX] Toutes les sirènes de la base se déclenchent. Un haut-parleur géant descend du ciel, accroché à un avion de papier.

### SCÈNE 4-6 : Boss : l'Adjudant @everyone

[DÉCOR] Un **mégaphone géant** à moustache, avec une casquette d'adjudant et des bras mécaniques. Chaque phrase qu'il prononce s'affiche en lettres capitales énormes.
ADJUDANT : GRÈVE NON AUTORISÉE. TOUS LES SBIRES AU RAPPORT. @EVERYONE. @EVERYONE. @EVERYONE.
ROBIN : *(s'avance, en uniforme)* Pas aujourd'hui, mon adjudant.
ADJUDANT : SERGENT ROBIN. VOUS ÊTES CHEF D'ESCOUADE. VOUS AVEZ DES RESPONSABILITÉS.
ROBIN : Justement. *(Il dégaine une épée bien trop grande, à la Garen.)* Ma responsabilité, c'est eux.

> **Compétences de Robin** (aviateur, main Garen) : *JUSTICE DÉMACIENNE* (mono, très gros dégâts), *Frappe Aérienne* (zone), *Grève Générale* (statut *Étourdi* sur tous les ennemis, chance), *Plan de Vol* (buff défense de l'équipe).

[COMBAT] **L'Adjudant @everyone** (2 phases, avec interventions)

- **Phase 1**
  - *Annonce Générale* : zone.
  - *@everyone* : statut *Confusion* sur un allié.
  - *Garde-à-vous !* : statut *Paralysie* sur un allié un tour.

- **Intervention 1 (au tour 2) : la grève**
  [ÉVÉNEMENT] L'Adjudant lance *Renforts* pour invoquer des sbires.
  ADJUDANT : SBIRES ! EN POSITION !
  [ÉVÉNEMENT] Trois sbires arrivent… s'assoient par terre, croisent les bras, et sortent une banderole « EN GRÈVE ».
  SBIRE : Désolé chef. Pause syndicale.
  ADJUDANT : … ???
  [ÉVÉNEMENT] L'invocation échoue. Elle échouera **à chaque tentative** pour le reste du combat.
  ROBIN : *(très fier)* Zingis.

- **Phase 2 (sous 50 % de PV)**
  - L'Adjudant passe en *Volume Maximum* : buff attaque.
  - *Rappel du Règlement* : zone, gros dégâts.
  - *Corvée de Chiottes* : debuff défense sur un allié.

- **Intervention 2 (au début de la phase 2) : Emma**
  [ÉVÉNEMENT] La radio de Robin grésille. Une voix douce.
  EMMA *(radio)* : Robin ? C'est Emma. Ça fait trois jours que t'as pas répondu. Tout va bien ?
  ROBIN : *(rougit, entre deux coups)* Emma ! Euh… oui, oui. Je suis juste… en train de combattre un mégaphone géant. Dans Discord.
  EMMA *(radio)* : … d'accord. Mais t'as mangé ?
  ROBIN : … non.
  EMMA *(radio)* : Je m'en doutais. Je t'envoie quelque chose.
  [ÉVÉNEMENT] Un petit avion de papier rose traverse le terrain et lâche un colis dans les bras de Robin : **Panier Repas d'Emma**. Utilisé automatiquement : **soin complet de l'équipe**, et **buff attaque et défense pour Robin** jusqu'à la fin du combat.
  EMMA *(radio)* : Et rentre pas trop tard. Bisous.
  ROBIN : *(fond complètement)* … bisous.
  JOSÉ : *(les larmes aux yeux)* Ça, c'est l'amour. Ça fait combien de temps, vous deux ?
  ROBIN : Très, très, très longtemps.
  JOSÉ : *(regarde le ciel, là où la pilote a décollé)* Un jour. Un jour, moi aussi.
  ADJUDANT : FIN DES COMMUNICATIONS PERSONNELLES !
  ROBIN : Toi, tu ne parles pas comme ça d'Emma.

- **Fin du combat**
  [ÉVÉNEMENT] Cinématique : Robin fait tournoyer son épée (*Tourniquet* à la Garen), saute, et l'abat sur l'Adjudant en hurlant : « ZIIIIINGIIIIS ! » Le mégaphone se tord, crache un dernier « @everyo… » et s'écrase. Les sbires en grève applaudissent.

### SCÈNE 4-7 : Après la grève

[DÉCOR] La base, de jour. Les sbires ont accroché des banderoles « ZINGIS » partout. Un barbecue s'improvise sur la piste.
[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (4/7)**.
[ÉVÉNEMENT] Objet obtenu : **Galons de Sergent**, accessoire pour Robin. *Description : « Responsabilités +10. Envie d'être là −50. »*

ROBIN : Bon. Je résume. On est dans Discord, le Modérateur a pris le pouvoir, Camil s'est autoproclamé chef, et Jordan a amené son chat.
JORDAN : C'est à peu près ça.
ROBIN : Camil, sur un trône. *(Il secoue la tête.)* Ça m'étonne pas. Un tyran, ça commence toujours par une statue.
JOSÉ : La sienne est minuscule.
ROBIN : Ça commence toujours par une *petite* statue.

JOSÉ : Au fait, Robin. Le Portugal. Toi aussi t'y étais.
ROBIN : Oui ?
JOSÉ : Sans moi.
ROBIN : José, c'est toi qui pouvais pas venir.
JOSÉ : *(se tourne lentement vers Jordan)* Ça, c'est ce qu'on t'a dit de dire.
JORDAN : Je l'ai PAS désinvité !

BIDOU : Et maintenant ? *(Inspire.)* On va où ?
ROBIN : Dans les rapports des sbires, il y a une zone qu'ils appellent les **Enfers du Classé**. Le Modérateur y envoie tous ceux qui perdent leurs parties classées. Et il paraît qu'un type en pantacourt y pousse un rocher depuis trois jours, en hurlant que c'est pas sa faute.
TOUS : … Florian.

[ÉVÉNEMENT] Sur la carte du monde, un message du Modérateur Fou défile dans le ciel, avec des fautes de frappe :
[DISCORD] **#annonces** · 🔨 **Modérateur Fou** (BOT)
> @everyone La base d'annonces est temporairement fermée pour cause de grvèe. Rappel : le salon **#classé** reste ouvert. Bonne chance pour remonter.
> — *Approuvé par Camil (1,62 m)*
ROBIN : Il a écrit « grvèe ». Il panique.
KEVIN : Zingis.

**FIN DU CHAPITRE 4**

---

### Récapitulatif chapitre 4 (pour l'intégration)
- **Recrue** : Robin (combattant, aviateur, main Garen). **Le système de réserve s'active** (5 personnages, 4 en combat).
- **Gags** : Clyde interprète (« Vous n'avez pas la permission d'envoyer des messages dans ce salon ») ; uniforme en pantacourt pour José ; « zingis ».
- **Énigmes** : la laverie (mini-objectif), les interrupteurs de la Tour (écrire ZINGIS sur la piste), le discours (choix de slogans).
- **Objets clés** : Fragment du Premier Message (4/7), Galons de Sergent, Panier Repas d'Emma (scripté).
- **Flags** : `rateaux_jose`.
- **Boss** : l'Adjudant @everyone (2 phases).
  - **Intervention 1** : les sbires invoqués font grève, l'invocation échoue.
  - **Intervention 2** : Emma à la radio envoie un panier repas (soin de l'équipe, buff de Robin).
- **Ceyn** : dans la bibliographie de la thèse de Robin (gag uniquement).
- **Clin d'œil** : Emma (photo dans le hangar et intervention radio).
- **Suite** : chapitre 5, les Enfers du Classé et Florian.

---

## CHAPITRE 5 : Les Enfers du Classé

> **Contexte** : le salon **#classé** est devenu les **Enfers**, un monde souterrain inspiré des enfers grecs, où le Modérateur envoie tous les joueurs qui perdent leurs parties classées. Les étages portent le nom des rangs : Fer tout en bas, puis Bronze, Argent… Florian y est condamné, comme **Sisyphe**, à pousser un rocher géant marqué « **LP** » jusqu'en haut de la pente. Chaque fois qu'il approche du sommet, une défaite le fait redescendre.
> **Florian** : campagnard en pantacourt, ADC Zeri, gros rageux en jeu, un amour dans la vie. Ses phrases : « C'est moi le meilleur », « J'ai juste pas de chance », « C'est pas ma faute ».
> **Moments clés** : la descente, Florian et son rocher, l'énigme du rocher (blocs à pousser), le boss.
> **Équipe** : Jordan, José, Kevin, Bidou, Robin (réserve), puis Florian.

### SCÈNE 5-1 : La descente

[DÉCOR] Au bout d'un chemin de la carte, une immense porte de pierre noire. Au-dessus, gravé : « **#classé — Vous qui entrez ici, abandonnez tout espoir de LP.** » Derrière, un escalier qui descend dans une lumière rouge.
[MUSIQUE] Thème des **Enfers** : chœurs lugubres, ponctués du petit *ding* de fin de partie classée.

ROBIN : Les Enfers du Classé. Les sbires disent que personne n'en est jamais remonté.
KEVIN : Statistiquement, c'est faux. Il y a toujours quelqu'un qui remonte. C'est le principe d'un classement.
BIDOU : *(inspire)* Il fait chaud, non ?
JORDAN : C'est les Enfers, Bidou.
BIDOU : Je sais. Mais il fait CHAUD.

[DÉCOR] Une caverne immense. Des rivières de lave. Des panneaux qui indiquent les étages : « **FER IV** », « **FER III** »… Des âmes damnées errent, le regard vide, en marmonnant « ff 15 », « report jungle », « c'était gagné ».
[ÉVÉNEMENT] À l'entrée, un **chien à trois têtes** couché en travers du chemin : le **Cerbère du Classé**. Ses trois têtes portent trois casquettes : TOP, MID, JUNGLE.
TÊTE TOP : Grr. Pourquoi vous êtes là ?
TÊTE MID : Grr. C'est la faute du jungler.
TÊTE JUNGLE : Grr. C'est PAS la faute du jungler.
[ÉVÉNEMENT] Les trois têtes se mettent à se disputer entre elles, et oublient complètement l'équipe.
JORDAN : … on passe ?
KEVIN : On passe.

> **Ennemis de la zone** : **Âmes Toxiques** (mono, debuff attaque : « t'es nul »), **Inters** (gros dégâts mono, mais défense très faible), **AFK Errants** (ne font rien pendant 2 tours, puis frappent fort), **Flammes du Chat** (zone, statut *Brûlure*).

### SCÈNE 5-2 : Florian et son rocher

[DÉCOR] Une pente gigantesque qui monte vers une lueur lointaine. Le sol est découpé en bandes : Fer, Bronze, Argent… Au milieu, un **rocher énorme** gravé « **LP** », et derrière, en train de le pousser de toutes ses forces : **Florian**, en pantacourt, chemise à carreaux, bottes de campagne, une casquette de tracteur sur la tête.
FLORIAN : *(en poussant)* Allez… allez… Bronze II… encore un peu… je suis meilleur que ça… je suis MEILLEUR QUE ÇA…
[ÉVÉNEMENT] Le rocher atteint presque la bande « ARGENT ». Une grosse voix tombe du plafond :
> **DÉFAITE.** −25 LP.
[ÉVÉNEMENT] Le rocher repart en arrière, roule sur Florian, et redescend toute la pente jusqu'en bas. *Boum.*
FLORIAN : *(sous le rocher, étouffé)* … C'ÉTAIT PAS MA FAUTE. C'ÉTAIT LE JUNGLER. Y AVAIT MÊME PAS DE JUNGLER, ET C'ÉTAIT QUAND MÊME SA FAUTE.

JORDAN : FLORIAN !
FLORIAN : *(se dégage, plein de poussière, et se retourne. Toute la rage disparaît d'un coup.)* … les gars ? *(Il court vers eux et les serre tous dans ses bras.)* Les gars, je vous aime. Je vous aime trop. Ça fait trois jours. Trois jours que je pousse ce caillou.
ROBIN : C'est Sisyphe, en fait.
FLORIAN : C'est qui, lui ? Il est quel rang ?
KEVIN : C'est un personnage de la mythologie grecque. Il pousse un rocher pour l'éternité.
FLORIAN : *(très sérieux)* Et il a jamais réussi ?
KEVIN : Non.
FLORIAN : Il devait avoir un mauvais jungler.

JOSÉ : Pourquoi tu t'arrêtes pas, tout simplement ?
FLORIAN : M'arrêter ? *(Il désigne le haut de la pente.)* José. Je suis meilleur que Bronze. Tout le monde le sait. C'est juste que j'ai pas de chance. Mes équipes sont maudites. Je suis le meilleur joueur des Enfers, et je suis coincé en bas.
BIDOU : *(inspire)* T'as essayé… de pas tilter ?
FLORIAN : *(un temps)* … je tilte pas. *(Il donne un coup de pied dans un caillou.)* JE TILTE PAS. *(Le caillou rebondit et lui retombe sur le pied.)* … ok. Un peu.

[ÉVÉNEMENT] *Tentative de drague de José (chapitre 5)*. Une **Âme Damnée** aux cheveux noirs est assise sur un rocher, au bord de la lave. Jingle Pierre, version orgue des enfers.
JOSÉ : *(ajuste son foulard malgré la chaleur)* Mademoiselle. Archéologue. Stylé. On pourrait remonter ensemble, vous et moi.
ÂME DAMNÉE : T'es quel rang ?
JOSÉ : Je joue pas à LoL.
ÂME DAMNÉE : *(se lève)* Alors t'as rien à faire en enfer. *(Elle disparaît dans un nuage de soufre.)*
JOSÉ : … c'est la première fois qu'on me rejette pour ne PAS être en enfer.
[FLAG] `rateaux_jose += 1`

### SCÈNE 5-3 : L'énigme du Rocher (blocs à pousser)

FLORIAN : Le seul moyen de sortir, c'est d'arriver en haut. La porte de la **Promotion**. Mais elle s'ouvre que si on pose le rocher sur les trois dalles de victoire. Et j'y arrive jamais tout seul.
JORDAN : Alors pousse pas tout seul.
FLORIAN : *(le regarde)* … c'est pas le genre de la maison.
ROBIN : C'est le principe d'une équipe, Florian.
FLORIAN : *(un temps, puis il soupire)* Ok. Mais si ça rate, c'est la faute de Kevin.
KEVIN : Pourquoi moi ?!
FLORIAN : T'aimes pas LoL. Ça porte malheur.
KEVIN : J'ai rien contre LoL, je veux juste pas y jouer !

> **Énigme de blocs à pousser** (classique RPG Maker) : la pente est une grille. Le rocher LP se pousse case par case dans la direction où on marche. Il faut l'amener successivement sur **trois dalles « VICTOIRE »** (la série de promotion). S'il touche une dalle rouge « DÉFAITE », il redescend tout en bas et l'énigme recommence (avec la voix : « DÉFAITE. −25 LP. »).
> Entre la 2ᵉ et la 3ᵉ dalle, un **combat obligatoire** : 3 Âmes Toxiques qui « flame » Florian. Après le combat, il est encore plus déterminé.

[ÉVÉNEMENT] *(Après la 2ᵉ dalle.)* Le rocher est presque en haut. Florian s'arrête, essoufflé.
FLORIAN : C'est toujours là que ça rate. Toujours au même endroit.
BIDOU : *(inspire)* Moi aussi… je rate toujours… au même endroit. *(Inspire.)* Le cri final. Mais avec les autres, j'y suis arrivé.
FLORIAN : *(le regarde)* … t'as raison, mon Bidou. *(Il pose ses mains sur le rocher, à côté des autres.)* Allez. Tous ensemble.

[ÉVÉNEMENT] Le rocher atteint la 3ᵉ dalle. Une fanfare retentit.
> **PROMOTION RÉUSSIE.** Argent IV.
FLORIAN : *(à genoux, les bras en l'air)* ARGENT ! ARGENT !! *(Il se relève et serre tout le monde.)* Je vous l'avais dit. C'est moi le meilleur.
JOSÉ : On a poussé avec toi.
FLORIAN : Oui, mais c'est moi qui avais l'idée de pousser.
[ÉVÉNEMENT] **Florian rejoint l'équipe.**

[ÉVÉNEMENT] La porte de la Promotion s'ouvre… sur une salle de tribunal immense. Au fond, sur un trône de pierre, une silhouette géante tient une balance dorée.

### SCÈNE 5-4 : Boss : le Juge du Matchmaking

[DÉCOR] Un démon géant en toge noire, avec un masque blanc sans visage. Sa balance dorée a deux plateaux : « TA FAUTE » et « PAS TA FAUTE ». Le plateau « TA FAUTE » est cloué en bas.
JUGE DU MATCHMAKING : FLORIAN. TU AS ÉTÉ PROMU SANS AUTORISATION. LE MATCHMAKING A DÉCIDÉ : TU APPARTIENS AU BRONZE.
FLORIAN : Le matchmaking, il m'a toujours mis avec des inters.
JUGE DU MATCHMAKING : LE MATCHMAKING EST JUSTE. LE MATCHMAKING NE SE TROMPE JAMAIS. C'EST TOUJOURS TA FAUTE.
FLORIAN : *(se fige, les yeux pleins de flammes)* … qu'est-ce que t'as dit ?

> **Équipe** : Florian est obligatoirement dans l'équipe pour ce combat. Le joueur choisit les 3 autres.
> **Compétences de Florian** (ADC, Zeri) : *Rafale Électrique* (mono), *Tir de Tracteur* (zone), *Rage de Tilt* (buff attaque sur soi : « ET TOI LE ZED… »), *Câlin* (soin mono, parce que c'est un amour).

[COMBAT] **Le Juge du Matchmaking** (2 phases, avec interventions)

- **Phase 1**
  - *Verdict* : mono, gros dégâts.
  - *MMR Caché* : debuff défense sur toute l'équipe.
  - *Mauvaise Équipe* : statut *Confusion* sur un allié (« Ton équipe te lâche »).

- **Intervention 1 (au tour 3) : le chat toxique**
  [ÉVÉNEMENT] Des fantômes de coéquipiers apparaissent autour du terrain et écrivent dans le chat, en bulles flottantes :
  > « ff 15 » · « report Zeri » · « adc diff » · « uninstall »
  FLORIAN : *(tremble de rage)* ADC DIFF ? ADC DIFF ?!
  [ÉVÉNEMENT] Florian reçoit automatiquement le statut *Tilt* : **buff attaque**, mais **debuff défense**.
  [ÉVÉNEMENT] Puis, une à une, les bulles de l'équipe apparaissent par-dessus le chat toxique :
  JORDAN : « gg Florian, t'es chaud »
  ROBIN : « zingis Florian »
  BIDOU : « … *(inspire)* … bien joué »
  JOSÉ : « t'as un beau pantacourt »
  KEVIN : « je comprends rien à ce jeu mais t'es fort »
  [ÉVÉNEMENT] Les fantômes toxiques se dissipent. Le debuff défense de Florian disparaît, le buff attaque reste.
  FLORIAN : *(ému, en tirant)* … les gars. Je vous aime. *(Il tire encore.)* JE VOUS AIME.

- **Phase 2 (sous 50 % de PV)**
  - Le Juge gagne *Série de Défaites* : zone, gros dégâts.
  - *Dodge* : il esquive une attaque et se soigne de 10 %.

- **Intervention 2 (au début de la phase 2) : le tracteur**
  [SFX] Un bruit de moteur diesel. *Teuf-teuf-teuf.*
  [ÉVÉNEMENT] Un **vieux tracteur rouge** défonce le mur du tribunal. Personne au volant, juste un poste de radio qui passe de l'accordéon.
  FLORIAN : *(les larmes aux yeux)* … Michel ?
  JORDAN : Ton tracteur s'appelle Michel ?
  FLORIAN : Il m'a retrouvé. Même en enfer. *(Il saute au volant.)*
  [ÉVÉNEMENT] Le tracteur roule sur la balance du Juge et la casse. Le Juge perd son *MMR Caché* et reçoit un **debuff défense** pour le reste du combat.
  JUGE DU MATCHMAKING : MA BALANCE ! SANS ELLE, JE NE PEUX PLUS DÉCIDER DE QUI C'EST LA FAUTE !
  FLORIAN : Ben voilà. Maintenant, c'est la faute de personne.
  ❓ *Le nom « Michel » est un placeholder : Florian a peut-être un vrai tracteur, ou un nom à mettre.*

- **Fin du combat**
  [ÉVÉNEMENT] Cinématique : Florian, debout sur le tracteur, tire une dernière *Rafale Électrique* façon ult de Zeri, qui traverse le masque du Juge. Le Juge se fissure et disparaît dans une gerbe d'étincelles.
  JUGE DU MATCHMAKING : *(en disparaissant)* … ce n'était… pas… ma faute…
  FLORIAN : *(très calme)* Ah. Maintenant tu comprends.

### SCÈNE 5-5 : La remontée

[DÉCOR] Un escalier de lumière s'ouvre au fond du tribunal et remonte vers la surface. Les âmes damnées des Enfers lèvent la tête : certaines commencent à monter, elles aussi.
[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (5/7)**.
[ÉVÉNEMENT] Objet obtenu : **Pantacourt Légendaire**, une armure pour Florian. *Description : « S'arrête exactement au genou. Résistance au feu +20. Résistance au jugement des autres +100. »*
JOSÉ : *(regarde le pantacourt)* … il est beau, en vrai.
FLORIAN : Merci. *(Un temps.)* Tu veux le même ?
JOSÉ : *(très vite)* Non.

[ÉVÉNEMENT] *(Gag, optionnel)* Au pied de l'escalier, un grand tableau de pierre : le classement des Enfers. Tout en bas de la liste : « **Ceyn** — Fer IV — 0 LP ».
FLORIAN : Ceyn.
ROBIN : Ceyn.
JORDAN : Ceyn.
KEVIN : Ceyn.
BIDOU : *(inspire)* Ceyn.
JOSÉ : Ceyn.
FLORIAN : *(regarde son propre rang, Argent IV, puis le tableau)* … bon. Je me sens mieux.

FLORIAN : Bon. Les gars. Pour être honnête… *(Il hésite, se gratte la nuque.)* Les défaites, là… peut-être que, parfois, c'était un tout petit peu ma faute.
*(Tout le monde se fige.)*
KEVIN : Il a dit quoi ?
ROBIN : Je crois qu'il a dit…
FLORIAN : Non, je rigole. C'était le jungler.
JORDAN : *(soulagé)* Ah, ouf. J'ai cru que t'étais possédé.

BIDOU : Et maintenant ? *(Inspire.)* Il reste qui ?
JORDAN : Yanis. Et Alex.
ROBIN : Les sbires parlent d'un **Marais**, où le Modérateur jette tous les utilisateurs AFK.
JOSÉ : Un endroit où tout le monde est inactif et où rien ne bouge ?
TOUS : … Yanis.

[ÉVÉNEMENT] Sur la carte du monde, un message du Modérateur Fou défile dans le ciel :
[DISCORD] **#annonces** · 🔨 **Modérateur Fou** (BOT)
> @everyone Un utilisateur a été promu Argent IV sans autorisation. Les promotions sont suspendues jusqu'à nouvel ordre. Rappel : le **Marais d'AFK** est une zone de repos obligatoire. Personne n'en sort.
> — *Approuvé par Camil (1,62 m)*
FLORIAN : *(fier)* Ils parlent de moi.

**FIN DU CHAPITRE 5**

---

### Récapitulatif chapitre 5 (pour l'intégration)
- **Recrue** : Florian (combattant, ADC Zeri, campagnard en pantacourt). 6 personnages, 4 en combat.
- **Zone** : les Enfers du Classé (étages par rang, Cerbère à trois têtes TOP / MID / JUNGLE).
- **Énigme** : le Rocher LP (blocs à pousser sur trois dalles « VICTOIRE », dalles « DÉFAITE » qui font recommencer).
- **Objets clés** : Fragment du Premier Message (5/7), Pantacourt Légendaire.
- **Flags** : `rateaux_jose`.
- **Boss** : le Juge du Matchmaking (2 phases).
  - **Intervention 1** : le chat toxique fait tilter Florian, puis les messages de soutien de l'équipe le calment.
  - **Intervention 2** : son tracteur « Michel » ❓ défonce le mur et casse la balance du Juge.
- **Ceyn** : dernier du classement des Enfers (gag uniquement).
- **Suite** : chapitre 6, le Marais d'AFK et Yanis.
