# RED ROOM — Le Serveur Maudit
### Script v0.3 : Prologue + Chapitres 1 et 2

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

> **Contexte** : le Modérateur Fou a enfermé Kevin dans le salon #rocket-league, transformé en stade flottant dans l'espace. Kevin y revit en boucle la finale des Worlds perdue contre **Vitality**, l'ennemi historique. Chaque fois que le but décisif est encaissé, la boucle recommence.
> ❓ *Jordan : c'était bien les Worlds de Lyon (2025) ? Si oui, on peut relier le stade au voyage à Lyon. Le score ou un moment précis du match aiderait aussi.*

### SCÈNE 2-1 : Décollage

[DÉCOR] À la sortie de Généralia, un **portail en forme de but de Rocket League**. Au-dessus, un néon : « #rocket-league — 1 utilisateur (en boucle) ».
CLYDE : Le salon de Kevin. Attention, il n'y a plus de gravité normale là-haut. Le Modérateur a tout réglé sur « Lune ».
JORDAN : Kevin doit être aux anges.
CLYDE : Il est en boucle depuis… *(il calcule)* … quatre cent douze matchs.
JOSÉ : Ah. Donc il est pas aux anges.

[ÉVÉNEMENT] L'équipe traverse le portail. Le saut se fait en voiture : Jordan au volant d'un *Octane* rouge, José à côté, Snow sur le tableau de bord.
JOSÉ : Pourquoi c'est toi qui conduis ?
JORDAN : Je suis le seul qui a le permis et une voiture, José.
JOSÉ : Même dans un monde imaginaire ?
JORDAN : *Surtout* dans un monde imaginaire.
[SFX] Bruit de boost. [ÉVÉNEMENT] Fondu sur un ciel étoilé.

### SCÈNE 2-2 : Le Stade Orbital

[DÉCOR] Une arène de Rocket League **flottant dans l'espace**, posée sur un astéroïde. On voit la Terre au loin, et un satellite qui passe. Les tribunes sont remplies de **spectateurs jaunes et noirs** aux antennes d'abeille, les **Supporters de la Ruche**. De l'autre côté, une seule tribune rouge et vide, sauf un petit drapeau « KC » qui flotte tout seul.
[MUSIQUE] Thème du **Stade Orbital** : électro épique, version synthwave du thème de menu de Rocket League. À chaque reset de la boucle, la musique saute comme un disque rayé.

[ÉVÉNEMENT] Sur le terrain, une voiture bleue fait des acrobaties parfaites : aerials, flip resets, ceiling shots. Au volant, Kevin, casque de cosmonaute sur la tête.
KEVIN : *(dans les haut-parleurs du stade, il commente son propre match)* … Kevin récupère la balle, angle d'approche 37,4 degrés, vitesse optimale, trajectoire parfaite, c'est mathématiquement impossible de rater…
[SFX] *BUZZER.* Un but jaune géant s'affiche : « **VITALITY MARQUE** ». La foule d'abeilles bourdonne de joie.
KEVIN : … c'était mathématiquement impossible de rater.
[ÉVÉNEMENT] Un effet de cassette qu'on rembobine. Tout recommence : la balle revient au centre, le chrono à 5:00.
KEVIN : *(même intonation, mot pour mot)* Kevin récupère la balle, angle d'approche 37,4 degrés…

JORDAN : Il est bloqué.
CLYDE : Quatre cent treize.
JOSÉ : Il fait le même commentaire à chaque fois ?
CLYDE : Mot pour mot. Sauf la fois 207. Il a dit « skibidi ». On sait pas pourquoi.

### SCÈNE 2-3 : Les tribunes (exploration)

> Zone ouverte. Le joueur doit comprendre comment briser la boucle. Trois indices sont à récupérer dans les tribunes.

**A. Le Kop Rouge (la tribune vide)**
[ÉVÉNEMENT] Le petit drapeau KC flotte seul. En s'en approchant, on entend des chants lointains, très faibles : « *KC… KC…* ».
CLYDE : Les supporters de Kevin étaient là, avant. Le Modérateur les a mutés un par un.
JORDAN : Alors on va chanter, nous.
[CHOIX]
1) Chanter « KC ! KC ! »
2) Rester digne, on a 29 ans.
*Si 1 :* JORDAN et JOSÉ : « KC ! KC ! KC ! » · [SFX] Le stade tremble légèrement. Sur le terrain, Kevin tourne la tête une demi-seconde, puis reprend sa boucle.
[FLAG] `indice_chant = true`
*Si 2 :* JORDAN : « Non. J'ai une réputation. » · JOSÉ : « Laquelle ? Le vieux ? » · *(Retour au choix.)*

**B. La Cabine des Commentateurs**
[DÉCOR] Un studio vitré au-dessus du terrain. Dedans, un robot-commentateur en costume jaune et une **Commentatrice** en tailleur.
[ÉVÉNEMENT] *Tentative de drague de José (chapitre 2).* Jingle Pierre.
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

[ÉVÉNEMENT] Sur le pupitre de la cabine, un écran affiche les **statistiques de Kevin** sur les 413 boucles.
> Tirs : 4 130 · Arrêts : 8 260 · Buts : 0 · Buts encaissés en fin de match : 413 · Phrase la plus prononcée : « angle d'approche » (413) · Deuxième phrase : « skibidi » (1)
CLYDE : La boucle est bloquée sur le moment du but. Tant qu'il le revit à l'identique, ça recommence. Il faut qu'il se passe quelque chose de **différent**.
[FLAG] `indice_stats = true`

**C. Le Vestiaire**
[DÉCOR] Un casier au nom de Kevin. Dedans : un diplôme d'ingénieur encadré, un poster de fusée, une maquette de satellite… et un post-it « *si on perd je pars sur Mars* ».
[ÉVÉNEMENT] Au fond du casier, une photo de la Red Room au complet devant un stade, tous en maillot. Kevin est au centre, bras levés.
JOSÉ : C'était avant la finale. Il y croyait tellement.
JORDAN : On y croyait tous.
[ÉVÉNEMENT] *(Graine discrète.)* Au dos de la photo, un petit tampon : « *Photo : Ceyn* ».
[ÉVÉNEMENT] Mécanique « Ceyn. » :
JORDAN : Ceyn.
JOSÉ : Ceyn.
CLYDE : *(il ne connaît pas le gag, mais il le fait quand même, par politesse)* … Ceyn ?
[ÉVÉNEMENT] *(Ils rangent la photo et reprennent comme si de rien n'était.)*
[FLAG] `indice_vestiaire = true`

**PNJ optionnels**
- **Une Abeille Supportrice** : « Bzz. Ça fait 413 fois qu'on gagne. Honnêtement, on commence à s'ennuyer. On peut pas gagner contre quelqu'un d'autre ? »
- **Un vendeur de hot-dogs spatial** : « Hot-dog en apesanteur, 12 €. » *(À Jordan :)* « Pour vous, 18 €. Vous avez une voiture. »
- **Une bannière LoL abandonnée** (« LEC — Summer Split ») : si le joueur l'examine, Kevin hurle depuis le terrain, sans sortir de sa boucle : « ENLEVEZ ÇA DE MON STADE. »

### SCÈNE 2-4 : Entrer dans la boucle

[ÉVÉNEMENT] Quand les trois indices sont trouvés, Clyde ouvre un accès au terrain.
CLYDE : Si vous entrez sur le terrain, vous entrez dans la boucle. Vous allez revivre la même minute avec lui. À vous de la changer.
JORDAN : Et si on n'y arrive pas ?
CLYDE : Vous serez commentateurs pour l'éternité.
JOSÉ : Ça va, il y a pire comme métier.

[ÉVÉNEMENT] L'équipe descend sur le terrain. La boucle les absorbe : effet de rembobinage, chrono à **1:00**.
KEVIN : *(sans les regarder)* Kevin récupère la balle, angle d'approche 37,4 degrés…
JORDAN : KEVIN !
KEVIN : *(se fige, les regarde enfin)* … Jordan ? José ? *(Un temps.)* Vous êtes pas censés être là. Dans ma simulation, vous êtes dans les tribunes, et vous pleurez.
JOSÉ : On pleurait pas.
KEVIN : José, j'ai 413 enregistrements de toi en train de pleurer.

> **Mécanique de boucle (puzzle)** : le joueur dispose d'une minute de match par essai. Il doit faire **trois choses différentes** pendant la boucle, une par indice trouvé. Chaque essai raté rembobine la minute, avec une réplique différente de Kevin, de plus en plus brainrot.
>
> 1. **Le chant** (`indice_chant`) : faire chanter le Kop Rouge. Les supporters mutés se remettent à chanter : « KC ! KC ! ».
> 2. **Les stats** (`indice_stats`) : utiliser *Souvenirs du Crétacé* de Jordan sur le gardien jaune pour révéler sa faiblesse (« Il défend toujours à gauche. Je l'ai vu en 1998. »).
> 3. **La photo** (`indice_vestiaire`) : montrer la photo d'équipe à Kevin.
>
> **Bonus caché** : poser Snow sur la balle. Snow refuse de bouger, le ballon ne peut plus avancer, et l'arbitre siffle « **ballon bloqué par un chat** ». Kevin : « Ça, c'est pas dans mes calculs. »

**Répliques de Kevin à chaque échec** (dans l'ordre) :
1. « Statistiquement, on perd. J'ai simulé 14 millions de futurs. On perd dans tous. »
2. « Sauf un. Dans un futur, le ballon est un sigma. Mais c'est pas réaliste. »
3. « La gravité de cet astéroïde est de 0,16 g, la balle part à 98 km/h… c'est cooked. Skibidi cooked. Rizz-less. »
4. « J'ai un doctorat. Enfin presque. Et je suis en train de dire "skibidi" dans l'espace. Mes parents seraient tellement fiers. »
5. « Vous savez qu'Elon pourrait m'embaucher, hein ? Il cherche des ingénieurs. Il cherche pas des gens qui perdent contre Vitality. »

### SCÈNE 2-5 : La photo

[ÉVÉNEMENT] Une fois les trois actions réalisées, la boucle se fige au moment exact du but. La balle reste suspendue devant la cage de Kevin.
KEVIN : *(regarde la photo)* … on y croyait vraiment, hein.
JORDAN : Ouais.
KEVIN : J'ai calculé tout ce qui pouvait se passer pendant ce match. Les angles, les rebonds, le boost. Mais j'avais pas calculé que ça ferait aussi mal de perdre contre *eux*.
JOSÉ : Personne calcule ça. C'est pour ça qu'on est supporters et pas ingénieurs.
KEVIN : Je suis les deux.
JOSÉ : Ben c'est pour ça que t'as deux fois plus mal.
*(Un temps.)*
KEVIN : *(sourit enfin)* Ok. Ok. On la rejoue. Pas pour changer le passé. Juste pour… le kiffer.
JORDAN : Et pour leur mettre une raclée.
KEVIN : *(rabat sa visière)* Ça aussi, c'est dans mes calculs.

[ÉVÉNEMENT] **Kevin rejoint l'équipe.** La boucle se brise comme une vitre. Le chrono passe en **PROLONGATION**.
[ÉVÉNEMENT] Les abeilles du stade se rassemblent au centre du terrain et fusionnent dans un bourdonnement assourdissant.

### SCÈNE 2-6 : Boss : la Reine de la Ruche

[DÉCOR] Une gigantesque **reine abeille jaune et noire**, couronnée, avec des réacteurs de Rocket League à la place des ailes.
REINE DE LA RUCHE : BZZZ. 413 VICTOIRES. 413. VOUS POUVEZ PAS GAGNER. C'EST ÉCRIT DANS LES STATS.
KEVIN : Les stats, c'est moi qui les écris.
REINE DE LA RUCHE : … BZZ ?

> **Équipe imposée pour ce combat** : Jordan, José, Kevin. Snow est en tribune.
>
> **Compétences de Kevin débloquées** :
> - *Aerial* : attaque aérienne, ignore la défense des ennemis volants.
> - *Calcul de trajectoire* : le prochain coup est un critique garanti.
> - *Mode Brainrot* : effet aléatoire parmi « Skibidi » (dégâts ×3), « Ohio » (Kevin s'attaque lui-même) et « Rizz » (charme l'ennemi un tour).
> - *Décollage* : fuite de combat garantie (désactivée contre les boss : « Même moi je peux pas fuir ça »).

[COMBAT] **La Reine de la Ruche** (3 phases)
- **Mécanique centrale : le ballon.** Un ballon géant rebondit dans l'arène. Chaque tour, il se rapproche du but de l'équipe (jauge de 0 à 5). À 5, c'est un « but encaissé » : dégâts massifs à toute l'équipe. Les attaques physiques et *Aerial* repoussent le ballon vers le but adverse ; un **but marqué** étourdit la Reine un tour.
- **Phase 1 : Coup d'envoi**
  - *Essaim* : invoque deux **Abeilles Supportrices** qui soignent la Reine.
  - *Piqûre jaune* : poison sur un allié.
  - Réplique, REINE : « BZZ. VOUS AVEZ DÉJÀ PERDU UNE FOIS. VOUS ÊTES HABITUÉS. »
- **Phase 2 (sous 60 %) : Prolongation**
  - La Reine utilise *Rembobinage* : elle tente de relancer la boucle et soigne 20 % de ses PV.
  - Le chant « KC ! KC ! » du Kop Rouge **annule le Rembobinage** si `indice_chant = true`. Sinon, il faut le contrer avec une *Relique Puante* (« Les abeilles détestent ça. Tout le monde déteste ça. »).
  - Réplique, KEVIN : « Pas cette fois. Je ferme la boucle. Comme une fonction récursive bien écrite. »
- **Phase 3 (sous 25 %) : But en or**
  - La Reine se met en **défense totale** devant son but. Seul un *Calcul de trajectoire* suivi d'un *Aerial* peut marquer.
  - Si le joueur tente autre chose : KEVIN : « Non non non, angle d'approche, Jordan ! 37,4 degrés ! »
  - Quand le but est marqué : cinématique. Le ballon traverse la Reine, qui explose en confettis jaunes. Le stade s'illumine en rouge.

### SCÈNE 2-7 : Après le match

[ÉVÉNEMENT] Le tableau d'affichage clignote : « **RED ROOM 1 – 0 VITALITY** ». Puis, juste en dessous, en petit : « *(Ce résultat n'a aucune valeur officielle.)* »
KEVIN : *(fixe l'écran)* Ça change rien à la vraie finale.
JORDAN : Non.
KEVIN : *(sourit jusqu'aux oreilles)* Mais putain, ça fait du bien.
JOSÉ : Mec, t'as les yeux qui brillent.
KEVIN : C'est la poussière cosmique. *(Un temps.)* Et l'émotion. Mais surtout la poussière cosmique.

[ÉVÉNEMENT] Le Kop Rouge se remplit : les supporters mutés retrouvent la voix et chantent. Snow est au premier rang, il ne chante pas.
[ÉVÉNEMENT] Objet obtenu : **Fragment du Premier Message (2/7)**. Il tombe du ciel au centre du terrain.
[ÉVÉNEMENT] Objet obtenu : **Maillot de Finale**, une armure pour Kevin. *Description : « Encore un peu humide de larmes. Défense +15. »*

KEVIN : Bon. Vous m'expliquez ce qui se passe ? Pourquoi on est dans Discord, pourquoi j'étais en boucle, et pourquoi y a un chat dans l'espace ?
JORDAN : C'est le Modérateur Fou. Et apparemment, Camil est derrière.
KEVIN : Camil ? *(Il réfléchit.)* Statistiquement, ça tient. Il a jamais supporté qu'on fasse des trucs sans lui.
JOSÉ : Il a fait une statue de lui. Minuscule. Sur un socle immense.
KEVIN : *(très sérieux)* Il compense. C'est de la physique de base. Plus la masse est petite, plus le socle doit être grand pour garder le même… ego.
JOSÉ : C'est vrai, ça ?
KEVIN : Non. Mais ça sonnait bien.

[ÉVÉNEMENT] Kevin regarde la Terre au loin.
KEVIN : Vous savez quoi ? Quand on sortira d'ici, je postule chez SpaceX. Pour de vrai.
JORDAN : Tu dis ça depuis trois ans.
KEVIN : Oui. Mais là, j'ai battu une reine abeille dans l'espace. J'ai de l'expérience terrain.

### SCÈNE 2-8 : Sortie du stade

[ÉVÉNEMENT] Retour vers le portail. Une bannière LoL est restée accrochée au-dessus de la sortie.
KEVIN : Non. Je passe pas sous ça.
JORDAN : Kevin, c'est une bannière.
KEVIN : C'est une bannière **LoL**. C'est pire.
[ÉVÉNEMENT] *(Le joueur doit faire le tour du stade pour sortir. Trente secondes de détour. Kevin est satisfait.)*

[ÉVÉNEMENT] Sur la carte du monde, un nouveau message du Modérateur Fou défile dans le ciel :
[DISCORD] **#annonces** · 🔨 **Modérateur Fou** (BOT)
> @everyone Un utilisateur a quitté la boucle sans autorisation. Une enquête est ouverte. Rappel : le salon **#vocal-1** est fermé jusqu'à nouvel ordre. Toute respiration y est interdite.
> — *Approuvé par Camil (1,62 m avec talonnettes)*

KEVIN : Toute respiration est interdite ? Mais Bidou…
JOSÉ : Bidou respire déjà à moitié en temps normal.
JORDAN : Alors on n'a pas de temps à perdre.

**FIN DU CHAPITRE 2**

---

### Récapitulatif chapitre 2 (pour l'intégration)
- **Recrue** : Kevin (combattant).
- **Objets clés** : Fragment du Premier Message (2/7), Maillot de Finale.
- **Flags** : `indice_chant`, `indice_stats`, `indice_vestiaire`, `rateaux_jose` (variante « refus par principe »).
- **Mécaniques nouvelles** : puzzle de boucle temporelle (une minute par essai), ballon et jauge de but en combat.
- **Graines du twist** : le tampon « Photo : Ceyn » au dos de la photo d'équipe (photographe = ses photos de mode).
- **Suite naturelle** : chapitre 3, #vocal-1 et Bidou.
