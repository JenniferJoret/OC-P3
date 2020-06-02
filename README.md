# OHMYFOOD!

## Sommaire
1. [INTRODUCTION](#introduction)
2. [COMPOSITION DU SITE](#composition-du-site)
3. [CARACTÉRISTIQUES TECHNIQUES](#caracteristiques-techniques)
4. [COMPATIBILITÉ](#compatibilite)
5. [CONTACT](#contact)

## INTRODUCTION
[Ohmyfood!](https://jenniferjoret.github.io/OC-P3/index.html) est une entreprise de réservation de restaurants et de composition de menus
en ligne. Notre concept permet aux utilisateurs de réduire leur temps d’attente dans les
restaurants car leur menu est préparé à l’avance. Plus de perte de temps à consulter la
carte !  


## COMPOSITION DU SITE
### Description du site :

- une page d’accueil contenant :
    - Le header, avec le nom de l'entreprise,
    - Le corps de la page (main), contenant les "cartes" des menus et une section “prochainement”,
    - Le footer, comprenant les liens « Mention légales » et « Contactez-nous ».
- 4 pages (à ce jour) contenant chacune le menu d’un restaurant (l'utilisateur sera redirigé sur la bonne page en fonction de la carte choisie sur l'accueil), 
- Une page “Mentions légales”, qui s'ouvre dans une nouvelle fenêtre lors du clic,
- Un lien “Contactez-nous”, qui renvoie vers l'adresse mail de contact d'ohmyfood!,
- le header et le footer sont présents sur toutes les pages,
- le footer rester visible lors du scroll.

### Animations du site :
- Chaque "carte" de l'accueil est dotée d'une animation, qui fait un zoom sur l'image, avec un effet de fondu,
- Dans la section "prochainement", les points de suspension sont animés,
- Les liens “contact” et “mentions légales” se secouent au survol de la souris,
- Les titres représentant les catégories entrées, plats, desserts sont soulignés de gauche à droite au survol de la souris .

## CARACTÉRISTIQUES TECHNIQUES

Le site a été réalisé avec **HTML5** et **SASS**

### HTML
À ce jour, le site comprend un total de 6 pages HTML : 
- ***index.html***, 
- ***la_note_enchantee.html***,
- ***la_palette_du_gout.html***,
- ***le_chic_a_la_francaise.html***,
- ***le_delice_des_papilles.html***,
- ***mentions_legales.html***.

Globalement, les pages sont toutes structurées de la même manière, en-tête (header), contenu (main), pied-de-page (footer).  

L'en-tête et le pied de page sont présents sur toutes les pages du site. Le footer n'a qu'un seul changement, le lien vers la page des mentions légales est absent lorsque l'utilisateur la visite.

En ce qui concerne le contenu de la page : 
- ***index*** est composé d'une _section_ qui contient les différentes "cartes" des menus, et une _section_ contenant "Prochainement".
- ***les différents menus*** sont tous composés de la même façon : 
    - un _span_ contenant le titre noir de la page,
    - une _section_ contenant le titre interne du menu et le reste de la page, lui aussi sectionné en trois parties (entrées, plats, desserts).  
    Ces trois parties sont composées de : 
        - une _div_ contenant les titres de sections et les SVGs associés, 
        - puis des _listes_ contenant l'intitulé des plats et leur prix.  

---------------------------------------
### SASS
>Sass permet d'utiliser des variables CSS, des fonctions, des mixins (une mixin est un morceau de code paramétrable, et réutilisable), et permet également de scinder son code en plusieurs morceaux, le tout avec une rédaction css simplifiée grâce à son imbriquement.  

Dans le dossier SASS, nous avons : 
- Un dossier "**base**", contenant : 
    - ***_reset.scss***, qui consiste à réinitialiser à 0 la valeur de certains éléments HTML certaines différences d'affichage sur les divers navigateurs,
    - ***_fonts.scss***, qui contient toutes les fontes utilisées sur le site,
    - ***_base.scss***, qui comprend les règles générales appliquées à tout le site.  


- Un dossier "**layout**", contenant la mise en forme de divers éléments répétés sur plusieurs pages, dont :
    - ***_header.scss***, qui contient les règles du header, 
    - ***_footer.scss***, qui contient les règles du footer, 
    - ***_menus.scss***, qui contient les règles générales appliquées à tous les menus du site.  


- Un dossier "**pages**", qui contient les règles qui ne sont appliquées qu'à certaines pages en particulier, dont :
    - ***_home.scss***, qui contient les règles propres à la page d'accueil, 
    - ***_mentions_legales.scss***, qui contient les règles propres à la page des mentions légales,
    - et une page de style pour chaque menu (d'autres viendront certainement), dont : 
        - ***_chic_francaise.scss***, pour le menu "Chic à la Française", 
        - ***_delice_papilles.scss***, pour le menu "Délice des Papilles",
        - ***_note_enchantee.scss***, pour le menu "La Note Enchantée",
        - ***_palette_gouts.scss***, pour le menu "La Palette du Goût".  


- Un dossier "**utils**", contenant les fichiers suivants :
    - ***_variables.scss***, qui contient toutes les variables utilisées dans SASS, 
    - ***_mixins.scss***, qui contient les mixins donc (les animations se trouvent ici aussi), 
    - ***_responsive.scss***, qui contient les règles appliquées lors du changement de résolution.

### INFORMATIONS SUR LES IMAGES DU SITE
Un logo et des favicons ont été tout spécialement créés pour le site Ohmyfood!, et chaque image ou dessin présent sur les maquettes a été vectorisé, puis placé dans le fichier "traits-sprites.svg" qui se trouve dans img/menus/.  

> À cause d'un bug de Chromium (qui a été reporté), les SVG contenant des dégradés ne s'affichent pas sur certains navigateurs.  
Certains SVG sont donc dans des fichiers séparés (mais toujours dans le même dossier), et seront intégrés au reste des sprites dès que le bug sera corrigé.
Pour le report du bug, voir [ici](https://bugs.chromium.org/p/chromium/issues/detail?id=751733&q=svg%20sprites&can=2).

## COMPATIBILITÉ

Dans sa première version, publiée le 2/06/20, ce site est compatible avec les dernières versions en date de Chrome, Edge, Firefox, et Safari.

## CONTACT
Vous pouvez joindre l'équipe de OHMYFOOD! à l'adresse suivante : contact@ohmyfood.com.  

Ce site a été réalisé par [Jennifer Joret](https://www.linkedin.com/in/jennifer-joret-14bab1180/), dans le cadre de la formation de développeur web d'[OpenClassrooms](https://openclassrooms.com/).

