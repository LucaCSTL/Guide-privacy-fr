# 🔒👨‍💻 Guide privacy fr
Guide en français sur la protection contre l'espionnage de Microsoft sous Windows et de défense pour le maintien de la vie privée sur Internet.

#### Ce guide va parler des connaissances que j’ai acquises quant à ces deux sections ci-dessous qui sont intrinsèquement lié :
* Protection contre l’espionnage sur Windows
* Défense pour le maintien de la vie privée sur Internet

#### Il sera aussi partagé un guide sur de l'OPsec en complément de ce guide là.

## 📝 Introduction

Rentrons dans le vif du sujet.
Nous sommes tous concerné par rapport à cela. Aujourd’hui, la quasi-totalité des gens possèdent un outil numérique leur permettant d’accéder à Internet. Et notamment un ordinateur. Cependant, ce que les gens ne savent pas, ou du moins, ne soupçonnent pas, c’est que dès le moment où ils se sont connectés à Internet, leur identité, et la moindre de leurs actions est enregistré, surveillé et contrôlé. Et cela permet d'établir sur eux un profil numérique. On parle de "double numérique". Ce qui peut à la fois être une façon de la part des grandes groupes (comme n'importe lesquels bien sûr) de se faire de l'argent en revendant ensuite ces précieuses données que les gens leurs transmettent sans soucis en acceptant tous ce qu'ils voient à l'écran. Mais aussi dans un autre cas, cela peut être le complément de quelque chose de plus grave dans le sens que toutes leurs données peuvent être utilisés contre eux un jour. Nous n’allons pas voir ici comment devenir 100% anonyme. Tout simplement car cela n’existe pas. Les gouvernements, disposant de ressources, d’outils et de temps nécessaire pourront un jour ou l’autre savoir. Non, ce qui compte ici, ce n’est pas de chercher l’anonymat parfait, car il n’existe pas, mais de limiter au maximum son empreinte, et leur emprise sur nous et nos données. Et, voir même, pour une protection vraiment avancée, de brouiller les pistes en adoptant les techniques d’OPsec pour les plus rigoureux. Mais ça c’est un sujet que l’on parlera dans un autre guide.

Concentrons-nous sur la base de base.

Tout d’abord, comme indiqué, ce guide concernera avant tout la sécurité pour les gens qui sont sous Windows. Même si sécurité rime davantage avec Linux, aujourd’hui, encore plus de deux tiers de la population ayant un ordinateur sont sous Windows. Cependant, nous allons voir en première partie la défense de vie privée pour notre OS. Ensuite viendra la protection concernant les données que nous partageons sans le vouloir en ligne à travers nos navigateurs. Et cela, est équivalent pour les autres OS. Linux comme MacOS (je me permets de prévoir ce que vont dire les puristes, oui je sais Linux n’est pas un OS à proprement parlé mais un kernel).

*« Mais pourquoi autant s’embêter ? Je n’ai rien à cacher. »* Snowden répondait alors à cette réflexion encore générale dans la tête de la plupart des gens ; « Dire que vous n'avez pas besoin de vous inquiéter de votre vie privée car vous n'avez rien à cacher est comme dire que vous n'avez pas besoin de vous inquiéter de votre liberté d'expression car vous n'avez rien à dire. »

Cette phrase insouciante que pense encore beaucoup de personnes (malgré que la tendance commence progressivement à se faire voir) est parfaite pour illustrer à quel point ceux qui pensent qu'ils n'ont "rien à cacher" ne se soucient absolument du monde dans lequel ils vivent. Vivre en 2026 dans un monde qui est déjà hyper-connecté, et où nos identités, et plus globalement, nos vies, sont inscrites dans un univers numérique/informatique sans prendre conscience que cela peut être risqué, est un niveau de naïveté sans pareil. Ce n’est même pas question de savoir si vous avez fait quelque chose de mal ou de répréhensible aux yeux de la loi, c’est de comprendre que vous êtes surveillé, espionné à votre insu. Et on parle pas là uniquement des petits hackers indépendants. Non, je parle bien par nos gouvernements.
>Rien n’est sans rappeler l’affaire en 2013 avec Snowden, ou encore avec Julian Assange pour ne citer qu’eux, de l’exposition de la surveillance de masse qu’organisaient les services secrets américains.

Ce qu’il faut savoir, c’est que la capacité de stockage de données de ces systèmes de surveillance de masses augmente chaque année. Vous n'imaginez pas la quantité de donnée, et le type qui est enregistré dans ces centres de données.
Aussi, vous n’avez pas besoin d’avoir fait quelque chose de mal. Il suffit juste qu’un jour, quelqu’un finisse par vous soupçonner, peut importe comment, et qu’ils utilisent leur système pour « remonter le temps » et examiner chacune de vos décisions, chaque ami avec qui vous avez discuté, chaque discussions, photos, mails, déplacement que vous avez fait au cours du temps, et d’ensuite vous attaquer sur cette base pour éveiller les soupçons. Et faire donc passer une personne, à priori innocente, en un malfaiteur. Il le font pour les lanceur d'alertes, les journalistes et certains avocats. Si ces corps de métiers sont si ciblé ce n'est pas pour rien. Imaginez si demain votre pays tombe sous un régime autoritaire voir totalitaire (USA...), qu'en sera-t-il de votre si cher liberté d'expression ? De votre droit à la contestation ? De votre vie privée en général ?

Bon, assez parler, démarrons avec la pratique désormais.


## 🕵️‍♂️ Protection contre l'espionnage de Microsoft avec Windows

### GodMode.
En tout premier lieu, ce que je vous conseillerai d’avoir sur votre bureau, est une page d’interface qui vous permet d’avoir accès à une vaste présentation d’options Windows qui vous permettront de changer/configurer les paramètres que vous souhaitez sans forcément connaître le chemin de destination de ces paramètres là. Cet outil qui permet cela est tout simplement un outil intégré directement dans Windows et qui se nomme « God Mode ». De son vrai nom « Windows Master Control Panel shortcut » ou raccourci du panneau de configuration principal de Windows, le GodMode s’avère très pratique pour avoir au même endroit tous les paramètres simples et avancés de Windows, surtout si vous devez y accéder régulièrement. Donc, pour ce faire, il faut faire :
1. Un clique droit dans un espace libre du bureau / Option Nouveau et sélectionner Dossier.
2. Il faut ensuite le renommer : sélectionner ce Nouveau Dossier / Option Renommer, et copier la séquence suivante tout attaché : « GodMode.{ED7BA470-8E54-465E-825C-99712043E01C} » puis valider par la touche Entrée au clavier. Le dossier change alors d'apparence et n’affiche normalement aucun nom.
3. Faites un double clique droit pour ouvrir le dossier, et voilà le travail.

### netplwiz.
Ce que je vous propose pour continuer avant de s’attaquer directement à ce que fait Microsoft sur vous, c’est d’être sur que personne qui vous est inconnu à de profil utilisateurs sur votre machine. Pour se faire :
1. Il faut ouvrir la fenêtre d’exécutable, en appuyant simultanément sur la touche Windows + r. (ou alors écrire « exécuter » dans la barre de recherche windows)
2. Une fois la fenêtre ouverte, écrire « netplwiz » et faire entrée.
3. Une fenêtre d’autorisation administrateur s’ouvrira alors, et vous demandera confirmation d’ouverture. Cliquez sur « oui ».
4. Une fenêtre s’ouvrira avec une page présentant les utilisateurs configurés sur votre machine. Avec leur nom, leur groupe, privilèges (administrateurs, invités…)
5. Si vous ne voyez aucun intrus sur votre machine, c’est bon. (Attention, cela ne veut pas dire que votre ordinateur n’a pas été hacker, cela veut juste dire que personnes d’autre n’a créé de profil utilisateur dans votre dos)

### mrt.
Continuons dans cette lancée de nettoyage de possibles intrusions, avec l’outil « mrt ». Encore un outil conçu par Windows (bon, juste pour clarifier certaines choses, Windows est un bon OS en soit, et offre des logiciels qui font le taff, surtout quand ça concerne sa sécurité, le problème ici est ce qu’il nous cache, de part la politique de Microsoft). mrt est un outil de suppression de logiciels malveillants assez complet. Il permet divers types d’analyses ; Rapides, Complètes et Personnalisées. L’analyse rapide analyse uniquement les zones de l’ordinateur qui sont susceptibles de contenir des logiciels malveillants. La complète elle, comme son nom l’indique, va analyser entièrement le système. Donc plusieurs centaines de milliers de fichiers, voire millions parfois. Et cette opération peut durer sur certains ordinateurs plusieurs heures. Et concernant la personnalisée, elle permet d’effectuer une analyse rapide et d’analyser le contenu d’un dossier spécifique. Donc pour ce faire, vous devez refaire la même première étape que pour netplwiz. Soit :
1. Il faut ouvrir la fenêtre d’exécutable, en appuyant simultanément sur la touche Windows + r. (ou alors écrire « exécuter » dans la barre de recherche windows)
2. Une fois la fenêtre ouverte, écrire « mrt » et faire entrée.
3. Une fenêtre d’autorisation administrateur s’ouvrira alors, et vous demandera confirmation d’ouverture. Cliquez sur « oui ».
4. Une fois la page de bienvenue ouverte, appuyez sur Suivant. Puis choisissez votre type d'analyse à effectuer.

### Paramètres de contrôle de compte d’utilisateur.
Accentuons ensuite, la sécurité concernant les modifications qui peuvent être apporté à votre ordinateur avec les paramètres de contrôle de compte d’utilisateur. Ce paramètre contribue à empêcher les programmes potentiellement suspects de modifier votre ordinateur. Pour ce faire, vous devez ;
1. Écrire dans la barre de recherche Windows ; « Paramètres de contrôle de compte d’utilisateur » et ouvrir le logiciel.
2. Une fois la fenêtre ouverte, faire glisser la barre présente sur la gauche tout en haut dans « Toujours m’avertir ». Ce qui permet d’activer la protection « Toujours m’avertir quand : des applications tentent d’installer des logiciels ou d’apporter des modifications à mon ordinateur + Je modifie des paramètres Windows. »
3. Appuyez sur OK pour confirmer vos modifications.

### Désactivation Peer-to-Peer.
Continuons dans la protection de votre machine, avec la désactivation du Peer-to-Peer (connexion directe entre deux machines qui établissent entre elles les rôles de client et serveur).
* Pour Windows 10 > Cliquez sur le bouton Démarrer > Paramètres > Ouvrir la rubrique Mise à jour et sécurité > Cliquez sur Optimisation de la distribution > Puis désactivez l’option Autoriser les téléchargements à partir d’autres PC.
* Pour Windows 11 > Cliquez sur le bouton Démarrer > Paramètres > Allez dans Windows Update > Options avancées > Puis dans l’onglet Options supplémentaires cliquez sur Optimisation de la distribution > Désactivez Permettre les téléchargements à partir d’autres appareils.

### Confidentialité et sécurité.
Alors pour cet ensemble de paramètres disponible dans l’onglet du même nom dans les paramètres Windows, je vous conseil de désactiver les options suivantes :
1. Dans l’onglet Sécurité dans la case Sécurité Windows, vous devez avoir tout coché en vert (Protection contre les virus et menaces, protection du compte, Pare-feu et protection réseau, Contrôle des applications et du navigateur, Sécurité de l’appareil)
2. Dans la case Localiser mon appareil, désactivez l’option.
3. Dans la case Chiffrement de l’appareil, activez l’option si vous estimez cela nécessaire, mais ne sentez pas obligé de le faire si vous n’avez pas de fichiers sensibles ou importants. Vous risquez de vous embêter plus qu’autre choses si vous parvenez à oublier vos identifiants ou l’accès à votre disque dur.
4. Dans l’onglet Autorisations de Windows dans la case Général, désactivez toutes les options présentes.
5. Dans la case Entrée manuscrite et personnalisation de la saisie, désactivez l’option Dictionnaire personnalisé d’entrée manuscrite et de saisie.
6. Dans la case Diagnostics et commentaires, désactivez toutes les cases (Données de diagnostic, Améliorer l’écriture manuscrite et la saisie, Expériences personnalisées, Afficher les données de diagnostic, et supprimez les données de diagnostic déjà présente) Puis cochez l’option Jamais dans la case de Fréquence des commentaires.
7. Dans la case Rechercher, désactivez l’option Rechercher dans l’historique puis effacez l’historique de recherche de l’appareil. Désactivez par la suite les options suivantes dans Rechercher mes comptes : Compte Microsoft et Compte professionnel ou scolaire. Enfin, désactivez également l’option Autoriser les applications de recherche à afficher les résultats.
8. Dans l’onglet Autorisation Windows dans la case Voix, désactivez la Reconnaissance vocale en ligne.
9. Dans l’onglet Autorisation des applications, c’est simple, vous allez désactiver toutes les cases. Seules les cases suivantes peuvent garder leur activation pour un aspect pratique tout même ; Documents, Images, Vidéos, Système de fichiers et Clés d’accès.
10. Dans l’onglet Autorisation de l’application, vous allez uniquement désactiver les cases Activation vocale et Appels téléphoniques.

### AllowCortana 0.
Si vous êtes sur Windows 10, vous pouvez mettre un terme à la curiosité de
Cortana. Pour cela :
1. Allez dans la barre des tâches, saisissez regedit (éditeur du Registre)
2. Lancez l'utilitaire Éditeur de registre.
3. Copiez-collez le chemin suivant dans la barre de navigation de l'éditeur de registre : \HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows
4. Faites un clic droit sur le dossier Windows et sélectionnez Nouveau > Clé.
5. Saisissez « Windows Search » pour nommer la clé qui vient d'être créée.
6. Faites un clic droit dans la fenêtre de droite et sélectionnez Nouveau > Valeur DWORD 32 Bits.
7. Saisissez AllowCortana pour nommer la valeur qui vient d'être créée.
8. Faites un clic droit sur AllowCortana et cliquez sur Modifier.
9. Dans le champ Donnée de la valeur, saisissez 0. Cliquez sur OK.

Vous pouvez fermer l'éditeur de registre : Cortana est maintenant désactivé.
Un redémarrage de l'ordinateur est conseillé. Une fois redémarré,
l'assistant personnel n'apparaît plus dans la barre des tâches.

### Télémétrie.
Nous allons voir désormais comment éteindre le DiagTrack, soit, les informations de télémétrie que recueille Microsoft sur votre machine. Pour ce faire ;
1. Allez dans la barre de recherche Windows, et tapez Services.
2. Vérifiez que le tri des services est effectué en suivant un ordre alphabétique, ensuite descendez jusqu’au service intitulé Expériences des utilisateurs connectés et télémétrie puis double cliquez dessus.
3. Dans la fenêtre qui s’ouvre, dans Général, vous allez sélectionner comme type de démarrage Désactivé.
4. Ensuite, il faut aller dans l’onglet Récupération (toujours dans la fenêtre de Propriétés de Expériences des utilisateurs connectés et télémétrie), et mettre toutes les défaillances en Ne rien faire.
5. Cliquez sur appliquer et tout sera bon.

### Pare-feu Windows.
Si vous souhaitez empêcher un logiciel d’accéder à internet, voici ce que vous pouvez faire :
1. Dans la barre de recherche (en bas à gauche de la barre des tâches), tapez Panneau de configuration, ce qui ouvre une fenêtre avec de nombreuses icônes de réglages.
2. Cliquez sur l’icône Système et sécurité, puis sur la rubrique Pare-feu Windows Defender (sur Windows 11, il se peut que le chemin soit très légèrement différent pour Windows 10)
3. Cliquez sur Paramètres avancés dans la rubrique à gauche. Cela ouvrira le Pare-feu Windows Defender avec des fonctions avancées de sécurité.
4. Dans le volet de gauche, cliquez sur Règles de trafic sortant, puis dans le volet d’actions à droite, cliquez sur Nouvelle règle, ce qui ouvre une nouvelle fenêtre de définition.
5. Choisir le programme concerné en pointant son .exe situé dans C:\Program Files (x86), ou C:\Program Files.
6. Finaliser l’opération en cochant Bloquer la connexion, puis Suivant, puis Terminer pour valider (après avoir nommée cette nouvelle règle).

---

Pour terminer cette première section sur la protection de votre machine contre les traceurs Microsoft comme autres, je vais désormais en bonus, vous partager trois éléments. Le premier, est un logiciel de qualité qui permet de résumer une grosse partie et plus encore des configurations que l’on a apportées, mais plus simplement. Ce logiciel se nomme **Wintoys** et est disponible dans le Microsoft Store. Je vous laisse le découvrir par vous-même ;)

Le deuxième élément bonus que je vous partage, est une commande qui permet de rendre toutes les données de votre disque dur irrécupérable (du moins, à 99%, la véritable manière de les rendres irrécupérable c’est d’y foutre le feu, de le broyer, puis de l’envoyer dans les entrailles de la terre, et encore...). Attention ! Cette manipulation est risquée, et convient d’être utilisée uniquement si vous êtes sûr de vouloir supprimer définitivement **TOUTES** vos données présentes sur votre disque dur.
#### La commande CIPHER /w permet d'effacer l'espace libre d'un disque dur ou clé USB ou SSD sans utiliser un logiciel tiers.
* Cette commande va se mettre à remplir l'espace libre par des données aléatoires, plus précisément des fichiers de large taille pour rendre la récupération des données à partir de l'espace libre impossible.
* CIPHER /w est fiable et sécurisée car elle n'écrit pas directement sur le disque dur mais passe par le système de fichiers en écrivant des fichiers avec des données aléatoires.
Maintenant averti, pour activer cette action, il vous suffit de suivre ces étapes :
1. Faites touche windows + r en même temps. Cela ouvrira la fenêtre d’invite de commande exécuter.
2. Taper « cipher /w:c: » et valider par Entrée. (NB : Remplacer si nécessaire la lettre c: par celle d’un autre disque dur. L’opération peut être longue, car le nombre de données à écrire est important. Il convient de n’utiliser cet outil, que si l’on est sûr de n’avoir aucun fichier à récupérer)

Enfin, le dernier élément bonus est une autre commande, mais qui sert à supprimer tous les bloatwares, la télémétrie (si pas déjà fait manuellement), et pleins de petits parasites graphique comme la pub, la recherche bing, Cortana, Windows Copilot…
Cette commande provient d’un projet GitHub open source donc vous pourrez vérifier par vous-même le code si vous le souhaitez, et voir en détails tous les éléments qui seront supprimés. Voici le lien du projet : <https://github.com/Raphire/Win11Debloat>

Et voici directement la commande à rentrer dans le Power Shell en mode administrateur :
**`& ([scriptblock]::Create((irm "https://debloat.raphi.re/")))`**
> Une fois la commande et l’installation validée, une nouvelle page PowerShell s’ouvrira, et vous aurez un choix quant au mode d’optimisation à choisir. Sélectionnez l’option 1 (Default mode) pour appliquer les choix par défaut, l’option 2 pour modifier des options du script (Custom mode), et l’option 3 si vous souhaitez choisir quelle application supprimer, et lesquelles garder. Une fois l’option choisie, appuyez sur entrée et laissez le script faire. Ne vous inquiétez pas si votre écran de bureau est repassé en noir durant quelques secondes durant le processus, c’est normal, car votre ordinateur redémarre le Process Windows Explorer pour appliquer les changements.


## 🛡️ Défense pour le maintien de la vie privée sur Internet

Le choix en tout premier lieu d’un navigateur est extrêmement important. Appliquer tous ces conseils et techniques, mais utiliser Edge, Chrome ou Opera sera complètement paradoxale.

Pourquoi je parle de ces navigateurs là comme exemple ? Tout simplement car ce sont parmis les plus utilisé et les moins sûre. Edge, tient de microsoft, pas besoin de développer plus (envoie de rapports d’utilisation de l’utilisateur, fingerprinting, télémétrie, etc, etc.), Chrome, c’est Google, pareille je ne devrai pas dévellopper davantage vous avez compris la chanson. Et pour Opera, c’est tout simplement le fait qu’une entreprise chinoise a racheté Opera en 2016. Est-ce que j’ai besoin de vous expliquer pourquoi il faudrait mieux l’éviter ? Je ne pense pas !

Donc, concernant les navigateurs, (les plus intéressants à utiliser car globalement fiable), je vous conseillerai :
* Firefox (sous configuration stricte),
* DuckDuckGo,
* LibreWolf,
* Mullvad Browser,
* Brave.
Les trois premiers après Firefox sont basé sur ce dernier. Brave quant à lui est basé sous Chronium. Concernant les trois premiers modèles (après Firefox default), ils sont axé sécurité et anonymat. (Brave est surtout utilisé pour le blocage de pubs et autres parasites intersites mais est aussi utilisé pour la sécurité et l’anonymat). Ces navigateurs configurent automatiquement plusieurs paramètres dans ce sens par défaut. Mais je vous conseille d’y ajouter des couches supplémentaires si vous souhaitez vraiment avoir le moins de tracabilité.

Pour les navigateurs sous Firefox, vous allez configurer / vérifier les paramètres suivants :
- Vous allez vous rendre dans les paramètres, et aller dans la rubrique « Recherche », une fois dedans, vous allez sélectionner le choix de moteur de recherche pour DuckDuckGo. À partir de maintenant, vous ne ferez plus vos recherche via Google.
- Ensuite, le plus gros, vous allez aller dans la rubrique suivante, intitulé : « Vie privée et sécurité ». Vous allez par la suite sélectionner le module « Stricte » dans la section « Protection renforcée contre le pistage ». Pensez cependant, à laiser cocher l’option « Résoudre les problèmes majeurs des sites », car le choix d’option stricte va tout de même faire que certains sites ne fonctionneront pas comme prévu. (Si cela vous arrive sur un site en particulier que vous devez absolument réjoindre, mettez en protection Standard le temps de l’utilisation).
    * Après cela, activez le paramètre « Demander aux sites web de ne pas vendre ni partager mes données » sous la section « Préférences de confidentialité des sites web ». Cela permet de signaler un refus des publicités ciblées ou une demande générale de limiter la vente ou le partage de vos données personnelles.
    * Continuons, toujours dans la rubrique « Vie privée et sécurité », après dans la section « Cookies et données de sites », cochez en bas de cette section, le paramètre suivant : « Supprimer les cookies et les données des sites à la fermeture de Firefox ». Certes vous aurez à vous reconnecter à chaque nouvelle session, mais au moins cela diminue dragstiquement le vol de vos données enregistrés à chacune de vos connexions.
    * Ensuite, dans la section « Mot de passe », décochez « Proposer d’enregistrer les mots de passes ». Tout simplement car vos mots de passes ne doivent jamais être enregistré dans votre navigateur par votre navigateur. Utilisez, si vous souhaitez quand même que cela ne soit pas trop barbant à la longue, l’extention ProtonPass avec code supplémentaire en paramétrant son verouillage toutes les une minute d’inutilisation. Vous aurez accès à votre gestionnaire de mot de passe fiable et complet, mais bloquer avec un code. Cependant, si vous souhaitez qu’aucun de vos mots de passe puisse être présent, même indirectement dans votre navigateurs, utilisez alors ProtonPass en tant que logiciel bureau, ou KeePassXC pour encore plus de sécurité. (KeePassXC ne dispose pas de synchronisation Cloud contrairement à ProtonPass)
    * Ensuite, pour les sections « Moyen de paiment » et « Adresses de facturation », bon, vous vous en doutez, mais désactivez les options réspective à chacune de ces deux sections (si activé déjà).
    * Pour l’historique, dans les règles de conservation, choississez la règle « Ne jamais conserver l’historique ». Et dans le paramètre « Effacer l’historique », cliquez dessus et sélectionner toutes les cases afin que les données sélectionné soient toutes effacé à chaque fermeture de Firefox.
    * Dans les permissions maintenant, ouvrez les paramètres de chaque permissions (localisation, caméra, son, etc.) et faites « Bloquer les nouvelles demandes d’accès à votre localisation » pour chaque paramètres disposant de cette option (sauf notifications). Par la suite, cochez les les deux options de fins suivantes : « Bloquer les popups et les redirections tierces » et « Prévenir lorsque les sites essaient d’installer des modules complémentaires ».
    * Ensuite, pour la section « Collecte de donneés par Firefox et utilisation », c’est simple, vous décochez tout.
    * Dans la section « Sécurité », vous cochez les trois options sous « Protection contre les contenus trompeurs et les logiciels dangereux » .
    * Concernant le mode HTTPS uniquement, vous sélectionnez « Activer le mode HTTPS uniquement dans toutes les fenêtres ».
    * Enfin, concernant l’activation du DNS via HTTPS, sélectionner l’option « Protection Maximale », en choissant soit Cloudflare, NextDNS, ou Quad9 comme fournisseur DNS. Si votre utilisation sur internet est rallentit, ou est impossible par moment, utilisez la protection renforcé à la place de la maximale.
- Maintenant, passons à la dernière étape de ce chapitre sur la défense et maintient de la vie privée sur Internet ! Nous allons parler des extensions. Il faut savoir en toute première chose que plus vous avez d'extensions, plus vous êtes à risques. La plupart des extensions peuvent (et doivent) pour fonctionner, avoir accès à ce qu'il se passe sur la page que vous consulter. De plus, l'accumulation d'extensions à pour effet de vous syphonner de la RAM. Alors ici, nous allons voir deux extensions puissantes, fiables, audité et reconnu pour vous protéger encore plus des potentiels attaques ou suivis.
    * La première est « uBlock Origin » développé par Raymond Hill. C’est un bloqueur de nuisances efficace, qui ménagera également votre processeur et votre mémoire vive. Tout en vous permettant de le personnaliser si bon vous souhaite, et de vous donner la possibilité de « zapper » des affichages nuisibles sur votre écran si le cas présent. Avec l’outil qui à la forme d’un éclair, vous pourrez faire disparaître de votre écran, une zone (textuel ou graphique) qui vous dérange sur l’affichage de la page que vous consulltez (effacement d’une zone visuel présent sur l’affichage client bien sûr).
    * La seconde extension qui va être importante à avoir est « NoScript Security Suite » développé par Giorgio Maone. Qui est un module qui autorise le contenu actif des sites auxquels vous faites confiance et protège des attaques par XSS et détournement de clic, « Spectre », « Meltdown » et d’autres failles JavaScript. Vous pouvez sélectionner le niveau de protection contre ces failles là site par site. C’est assez personnalisable mais prenez en compte que plus vous mettrez de restrictions (il se peut que certains soient mises automatiquement aussi), plus les sites que vous consulterez pourront avoir du mal à se charger/s’afficher. C’est à double tranchant ! Maintenant que vous avez les clés en mains pour sécuriser votre navigateur, vous avez donc aussi la possibilité de faire des compromis si cela vous convient !