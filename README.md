# Daktary

## US en cours

US-A1

## Serveurs
Prod : http://www.multibao.org
Pré-prod : http://dev.multibao.org

Hébergement :
* [Github Pages](https://pages.github.com)
* mltb-dktr

## Technologies
Langages :
Accès : http://www.multibao.org/index-dev.html
* [ES6](https://developer.mozilla.org/en-US/docs/Web/JavaScript/New_in_JavaScript/ECMAScript_6_support_in_Mozilla)

Tests unitaires :
Accès : http://www.multibao.org/tests
* [Mocha](https://mochajs.org/)
* [Expect](https://github.com/Automattic/expect.js)

Minification et transpilation (build) :
Accès : http://www.multibao.org
* [Babel](http://babeljs.io) : Transpilation en ES5 et fusion des fichiers
* [UglifyJs](https://github.com/mishoo/UglifyJS) : Minification des fichiers JS
* [UglifyCss](https://github.com/fmarcia/UglifyCSS) : Minification des fichiers CSS

* [npm]() utilisé pour le build
```bash
$ npm install
$ npm run build
```

## Installer le site en local
```bash
$ git clone git@github.com:daktary-team/daktary.git .
$ cd daktary
```

## Serveur local
C'est optionnel, mais les exemples qui suivent sont testés sur un serveur local.

> https://github.com/indexzero/http-server

```bash
$ http-server -p 8000
```

## Pour lancer les tests
Dans un [Firefox](https://www.mozilla.org/fr/firefox/developer/) **récent** lancer :
http://127.0.0.1:8000/tests

## Pour minifier et transpiler
```bash
$ npm install
$ npm run build
```

## Credits
Thomas Wolff : Product Owner
Stéphane Langlois : Développement
Erick Gardin : Intégration
Aymeric Faivre : Web Design
Xavier Caodic : Documentation
Louise Berrotte : Interviews, accompagnement contributeurs
Lilian Ricaud : Affinage Backlog
Claude Aubry : Affinage Backlog
Vincent Ferries : Code review
David Larlet : Code review
David Bruant : Code review
Vincent Agnano : Anywhere

## Suivi des tâches de développement web

## Comment changer les boutons d'accueil lien et titre
- Lien : Dans les fichiers dk.js et dk.min.js présents dans le dossier dist, il faut changer les liens du MUTLIBAO.BUTTON1 ou MULTIBAO.BUTTON2 en les retrouvant dans les fichiers grâce à CTRL+F "MULTIBAO.BUTTON" 
CONSEIL : en mode edit, choisir soft wrap plutôt que no wrap. 
- Titre du bouton : retourner à la racine du site et modifier le fichier config.js et retrouver les MULTIBAO.BUTTON pour changer leur titre entre '. 

## A creuser

### À prévoir
* Classement par le titre
* Merge contribution et breadcrumb parent repo
* Link absolute/relatif
* recherche en home
* Travis
* Simplify tests writes merge on async
* Doc de développement

### Discussion intégration
* Regarder GitBook
* Affichage fiches : [exemple des balises HTML](http://dev.multibao.org/#newick/grill/blob/master/styleguide.md)
