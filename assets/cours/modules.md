# Les Modules et Bundler

Sur un navigateur on ne peut pas utiliser `npm` ou `nodejs`, le `package.json` ne sert à rien ...

Heureusement, il éxiste aujourd'hui des `bundlers`. Ce sont des outils qui permettent d'utiliser `nodejs` et `npm` sur votre navigateur !

Ce sont des outils qui s'occupe de « compilé », « offusqué », « optimiser » touts vos fichiers css, html, json, images etc ...

Aujourd'hui incontournable ! Toutes les applications web les plus connus utilise un `bundler`. C'est ce qui nous permet d'installer des libraries, d'utiliser et d'optimiser le css, ou même d'utiliser d'autre langages de programmation comme python, typescript, sass, stylus etc ...

Il en existe beaucoup :

- [WebPack](https://webpack.js.org/)
- [Bun](https://bun.sh/) : C'est aussi un compilateur javascript
- [Parcel](https://parceljs.org/)

## Utiliser `Parcel`

Parcel est un `bundler` très puissant sans aucune configuration nescessaire, il comprend tout seul comme un grand toutes les technologies web moderne (typescript, coffee, sass) ...

### Installer `parcel`

Dans un projet javascript (un dossier avec un `package.json`) installer parcel :

```bash
$ npm i parcel
```

> Dans certain cas, il vous faut installer python : https://www.python.org/ftp/python/3.11.1/python-3.11.1-amd64.exe et visual studio : https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=Community&channel=Release&version=VS2022&source=VSLandingPage&cid=2030&workload=dotnet-dotnetwebcloud&passive=false#dotnet

### Utiliser parcel

Pour utiliser parcel il faut tout d'abord une page html :

```html
<!-- index.html -->
<!DOCTYPE html>
<html>
  <head>
    <title>Mon Site</title>
  </head>
  <body>
    <h1>Coucou les amis</h1>
  </body>
</html>
```

Il faut pour utiliser parcel, lancer la commande suivante :

```bash
$ npx parcel index.html
```
