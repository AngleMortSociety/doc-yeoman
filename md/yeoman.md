
# Yeoman

[Yeoman][] est un module qui vous permet de démarrer rapidement de nouveaux projets web en vous conseillant les meilleurs outils et pratiques pour rester productif.

Pour cela, le site officiel propose des générateurs de projets. Un générateur est un plugin qui peut être exécuté dans le Terminal avec la commande `yo` afin de générer des projets complets ou uniquement des parties spécifiques.

A l’aide de ces générateurs, l'équipe officielle promeut le « flux de travail Yeoman ». Ce flux de travail est une composition robuste et durable côté client, comprenant des outils et des frameworks qui peuvent aider les développeurs à créer rapidement des applications web solides et esthétiques. Yeoman s'occupe de vous fournir tout le nécessaire pour commencer simplement une configuration de votre projet.

Avec une architecture modulaire qui peut évoluer sans contrainte, Yeoman mise sur le succès et les leçons tirées de plusieurs communautés open-source pour s’assurer que les développeurs utilisent les meilleures pratiques le plus intelligemment possible.

Yeoman, avec ses plugins, vous permet de vous concentrer sur le développement de votre application plutôt que sur les détails techniques à mettre en œuvre pour le bon fonctionnement des outils.

## Installation

### Pré-requis

Pour l'installation de Yeoman, il est nécessaire que [Node.js][] soit installé et accessible sur votre machine. Si vous ne savez pas si c'est le cas, vous pouvez le vérifier avec la commande suivante :

```bash
node -v
```

Si le Terminal ne retourne rien, il vous faudra alors vous rendre sur le site officiel de [Node.js][] pour le télécharger et l’installer.

### Outils

Yeoman utilise [Grunt][], [Bower][] ou [Gulp][] comme modules complémentaires. Vous devrez utiliser `npm` pour les installer si vous ne les avez pas. La commande suivante installe Yeoman, Bower et Grunt :

```bash
npm install -g yo bower grunt-cli
```

## Utilisation

La première étape consiste à chercher le générateur que vous souhaitez utiliser pour démarrer votre projet. Pour cela, il faut se rendre sur cette [page][].

A titre d'exemple, entrez dans le champ de recherche le nom suivant : `webapp`. Dans la liste, vous pouvez cliquer sur un élément afin d'obtenir plus de renseignements sur celui-ci. Une fois le générateur correspondant à votre besoin localisé, il est nécessaire de l'installer afin que Yeoman puisse télécharger son contenu et effectuer toutes les tâches qui lui sont relatives. Pour ce faire, dans le Terminal, entrez la commande suivante :

```bash
npm install -g generator-webapp
```

C'est le générateur de projet par défaut pour réaliser des applications web. Il est à noter que les générateurs doivent être installés globalement (option *g*, pour *global*) et ne sont donc pas liés à un projet spécifique. Cette étape terminée, vous pouvez créer un dossier pour votre nouveau projet :

```bash
mkdir mon-projet-yo
```

Ensuite, entrez dans celui-ci :

```bash
cd mon-projet-yo
```

Et finalement, initialisez le projet :

```bash
yo webapp
```

La ligne de commande interactive vous proposera un certain nombre de choix afin de configurer le projet en fonction de vos besoins. Il est possible de choisir les composants suivants : [HTML5 Boilerplate][], [jQuery][], [Modernizr][] et [Bootstrap][]. Chaque projet contient des tâches Grunt préconfigurées afin de vous aider dans la gestion de votre flux de travail.

Le générateur `webapp` est le plugin considéré comme le plus simple pour démarrer une application web. Il existe également des générateurs de frameworks qui peuvent être utilisés pour échafauder un projet, des modèles, des contrôleurs, etc.

Pour obtenir de l'aide sur la commande et lister tous les générateurs disponibles sur le système :

```bash
yo --help
```

Il est aussi possible de lancer la commande `yo` sans argument pour obtenir la liste des générateurs et en choisir un pour créer un nouveau projet. A partir de ce menu, il est également possible d'obtenir de l'aide, d'installer de nouveaux générateurs ou de faire une mise à jour des modules installés sur le système.

[Yeoman]: http://yeoman.io "Yeoman - Site officiel"
[Node.js]: http://nodejs.org "Node.js - Site officiel"
[Grunt]: http://gruntjs.com "Grunt - Site officiel"
[Bower]: http://bower.io "Bower - Site officiel"
[Gulp]: http://gulpjs.com "Gulp - Site officiel"
[page]: http://yeoman.io/generators "Yeoman : discovering generators - Site officiel"
[HTML5 Boilerplate]: http://html5boilerplate.com "HTML5 Boilerplate - Site officiel"
[jQuery]: http://jquery.com "jQuery - Site officiel"
[Modernizr]: http://modernizr.com "Modernizr - Site officiel"
[Bootstrap]: http://getbootstrap.com "Bootstrap - Site officiel"
