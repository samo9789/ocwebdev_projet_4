## Conseils Projet 4

Nous travaillons sur

- le SEO (Search Engine Optimization)
- axe SEO (Accessibilité)
- Performance

## Constat initial :

Faire des captures d'écran des rapports

- dev tools > lighthouse (performances)
- dev tools > souces > coverage (performances)
- https://sitechecker.pro/ (SEO)
- axeSEO (accéssibilité)

## Github

- Push le projet dans son état initial sur GitHub (branche main)
- Créer une branche `develop` à partir de `main`

```shell
git init
git add . 
git commit -m "initial commit"
git add remote origin <url>
git push 

git checkout -b develop
git push 
```



## Optimisation du code CSS

Sur notre branche `develop`, nettoyer le CSS avec l'outil purgeCSS

https://purgecss.com/CLI.html#usage

```shell
npm install -g purgecss
purgecss --css  css/bootstrap.css  --content index.html page2.html --output styles/
purgecss --css  css/et-line.css  --content index.html page2.html --output styles/
purgecss --css  css/font-awesome.css  --content index.html page2.html --output styles/
```

 Le code CSS peut également être minifié



## Optimisation des *fonts* utilisées

Le site utilise deux polices d'icônes : et-icons et font-awesome

Les icônes des réseaux sociaux se trouvent dans et-icons, les utiliser et supprimer tout ce qui est relatif à font-awesome

## Optimisation des. images

Convertir toutes les bmp en png

Optimiser les images pour éviter d'avoir des images trop lourdes, notement 

- image-de-presentation
- la-chouette-agence-banniere



## Corrections des inclusions de code CSS et JS

Consultez le site avec la console chrome dev tools ouverte et voir sil y a des erreurs

- corriger les inclusions de script sur la page 2.html





## Lister les problèmes

- Lang de la page
- Balise meta title
- Langue des messages d'erreur (validation du formulaire de contact)
- Image BNP
- Texte sous forme d'image (sous titre sur la page d'accueil)
- CSS inutilie (notemment l'inclusion de tout bootstrap)
- Minifier le CSS, le JS, les images
- Titres en orange sur fond coloré illisible
- Nav, renommer page2 en contact
- Le design n'est pas responsive
- Page 2 : l'adresse est écrite en trop petit et sans vraie mise en page
- Page 2 : le sous-titre est trop petit et illisible
- Le texte sous les icônes (page d'accueil) semble trop petit
- Texte sur fond ligné (mangque de lisibilité)
- Le contenu du footer sur la page d'accueil semble provenir d'un mauvais copié/collé 
- Il manque les liens vers les réseaux sociaux
- Semantic des titres (passer de H1 a H2, pas h3) 
- Labels dans le formulaire manquants



## Implémenter les corrections

Commiter le code corigé sur la branche `develop`



**capture d'ecrans APRES**

- lighthouse
- coverage
- https://sitechecker.pro/ (SEO)
- AxSEO