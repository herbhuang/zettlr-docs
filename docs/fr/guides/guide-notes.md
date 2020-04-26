# Guide : Zettlr comme application de prise de notes

![Zettlr as a Note-Taking app](../img/zettlr_notes.png)

Vous voulez utiliser Zettlr comme moyen de prendre des notes avec. Bien que Zettlr dispose de beaucoup plus de fonctionnalités, il est conçu comme une application mince et minimale, de sorte qu'il est facile de configurer Zettlr comme une application de prise de notes. Ce guide vous montre les paramètres à utiliser et comment prendre réellement des notes.

> Grâce à ce guide, vous pouvez configurer Zettlr pour remplacer des applications telles que OneNote, Evernote ou nvALT.

## Étape 1 : Configurez Zettlr pour qu'il ait l'air aussi minimal que possible.

Tout d'abord, allez dans l'onglet "Paramètres" (appuyez sur `Cmd/Ctrl+,` ou cliquez sur le rouage dans la barre d'outils). Dans les paramètres, veillez à régler les paramètres en fonction de cette liste :

- Onglet General
    - Snippets (_bribes, brèves_) : Off
    - Barre latérale : Thin (_étroite_)
- Onglet Editeur
    - Dictionnaires : n'en sélectionner aucun (ils ralentissent le démarrage de l'application et ne sont pas nécessaires pour les notes simples)
    - Lignes muettes : Off

Les autres paramètres ne sont pas nécessaires pour une application de prise de notes et peuvent donc être ignorés.

## Étape 2 : Créez un dossier pour vos notes

Il est maintenant temps de créer un dossier pour vos notes. L'idéal serait de le placer dans un dossier synchronisé en ligne afin que vous puissiez y accéder de partout, et pas seulement de votre ordinateur actuel. Le nom de ce dossier dépend entièrement de vous, mais "Notes" peut être un bon point de départ, très simple. Si vous souhaitez utiliser différentes catégories pour les notes, vous pouvez créer des dossiers racine supplémentaires et les garder ouverts. De cette façon, vous pouvez nommer vos catégories en fonction de ce que vous y stockez :

- Students: "University", "Lectures", "Private"
- Teachers: "School"/"University", "Courses"
- Researcher: "University", "Research", "My Research Project"
- Journalist: "Topic 1", "Topic 2", "Topic 3", "Press Conferences"
- Writer: "My Novel", "Thoughts and Ideas", "Characters"
- Administrative Worker: "ToDo", "Meetings"
- etc. …

Choisissez des répertoires en utilisant les catégories dont vous avez personnellement besoin. N'oubliez pas que vous pouvez toujours réorganiser cela et faire glisser les fichiers si votre flux de travail change. L'avantage d'utiliser différents dossiers _root_ est que chaque dossier est indépendant de l'autre. Ainsi, vous pouvez toujours garder la liste des répertoires cachée et ne la remonter que si vous devez changer de " bloc-notes ".

**Alternative**: Au lieu d'utiliser plusieurs dossiers racine, vous pouvez également adopter l'approche par sous-répertoires. De cette façon, la liste des répertoires ne ressemble pas à une collection de catégories ou de "cahiers", mais ressemble à un véritable répertoire (je parle de la façon dont cela vous _apparaît_, car le visuel est également un aspect important pour une écriture efficace). Mais l'avantage de cette approche est que vous n'avez jamais besoin de sortir la liste des répertoires, mais vous pouvez changer de " bloc-notes " en commençant par cliquer avec `ALT`- or `Ctrl`sur le "bloc notes"/répertoire courant puis en cliquant sur un autre bloc-notes. Zettlr utilisera alors ce dernier comme répertoire courant dans lequel vous pourrez stocker des notes.

## Étape 3 : Pensez à un système de nommage de vos notes

Au fil du temps, vos carnets de notes _seront_ remplis de notes. Chaque séminaire, chaque réunion et chaque atelier apportera sa contribution à votre bloc-notes. Et si vous avez des pensées soudaines que vous voulez noter avant de les perdre, il est également recommandé de prendre une nouvelle note. Alors que faire pour ne pas perdre l'ordre de votre système ?

Zettlr propose plusieurs moyens de classer, trier et retrouver vos fichiers. Si vous connaissez le nom du fichier, il est alors facile d'y accéder : Il vous suffit de commencer à taper le nom du fichier dans la barre de recherche globale. Zettlr complétera automatiquement le nom pour vous. Il prend le premier fichier qui contient ce que vous avez déjà écrit, donc continuez à écrire le nom du fichier jusqu'à ce que Zettlr complète automatiquement le bon fichier. Ensuite, appuyez sur`Return` et il ouvrira le dossier.

En général, vos dossiers doivent suivre un certain schéma. Par exemple, si l'heure est importante (comme pour les ateliers, les congrès ou les conférences), il est préférable d'utiliser la date dans le format standard international (AAAA-MM-JJ, par exemple 2018-10-12) comme première partie de vos noms de fichiers. De cette façon, Zettlr triera automatiquement les fichiers de la manière par défaut (où un 2 est supérieur à un 1, par exemple), de sorte que les fichiers les plus récents se trouvent par défaut en bas. Pour les placer en haut, il suffit de changer le tri de A-Z à Z-A. En utilisant cette approche, il devient facile de trouver les anciennes notes, car vous vous souvenez normalement de la date approximative à laquelle un atelier ou une réunion a eu lieu et vous pouvez faire défiler la liste jusqu'à ce que vous la trouviez.

Si le temps n'est pas important, une autre approche est nécessaire. Si vous conservez des dossiers de notes pour différents concepts, processus ou comme une sorte de manuel, il peut être préférable d'utiliser des catégories comme première partie du nom du dossier. Par exemple, si vous prenez des notes sur le fonctionnement des logiciels dans votre bureau, il peut être bon de les trier par processus. Les noms de fichiers ressembleraient alors à ceci :

- HowTo - Finance - Excel
- HowTo - Finance - Company Database
- HowTo - Meetings - Beamer
- HowTo - Meetings - Conference Call

De cette façon, vous pouvez facilement trouver ce que vous cherchez en cherchant d'abord les dossiers qui commencent par " HowTo " et ensuite en faisant défiler jusqu'à ce que vous trouviez le processus (Finances, Réunions, Directives pour le courrier, etc...).

Vous pouvez même utiliser une combinaison de ces éléments. Le résultat final est le suivant : Gardez toujours à l'esprit que Zettlr trie par nom de fichier, donc nommez vos fichiers en conséquence pour minimiser le temps à passer avant de trouver un fichier.

## Étape 4 : Écrivez !

Maintenant que tous vos dossiers sont définis et que vous avez une idée générale de l'aspect que doivent avoir vos noms de fichiers, vous pouvez créer des notes en cliquant simplement sur `Cmd/Ctrl+N`. Saisissez votre nom (vous n'avez pas besoin d'ajouter d'extension de nom de fichier) et appuyez sur `Return` pour créer le fichier. Il sera automatiquement ouvert. Zettlr créera toujours les fichiers dans le carnet que vous avez sélectionné. Si vous souhaitez déplacer des fichiers d'un ordinateur portable à un autre, il vous suffit de faire glisser le fichier et de le déposer sur l'ordinateur portable dans lequel vous souhaitez le déplacer.

## Suivant : Tutoriel sur le markdown

Maintenant, vous pourriez être intéressé de savoir comment écrire rapidement et efficacement en utilisant Zettlr. Rendez-vous sur notre [tutoriel Markdown](../reference/markdown-basics.md) !
