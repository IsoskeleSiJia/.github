# Règles d'utilisations | charte ISK 2023

# Sommaire 
* [Informartions générale](#informartions-générale)
* [La charte graphique](#la-charte-grahique)
* [Eléments techniques](#eléments-techniques)

# Informartions générale : 
- Version de Wordpress : 6.2
- Version de php : 8.1.9
- Plugins utilisés : Elementor & Elementor Pro 
- Nom du thème : Hello Elementor | Version : 2.7.1

# La charte grahique : 
## Les couleurs 
- Blanc (#fff) --> fond principal des pages web
    > permet une meilleure lisibilitée
- Bleu (#01083B) --> couleur principale des corps de texte et des titres 
            --> utilisation en fond pour certain bloc spécifique tel que le header ou le footer (dans ce cas, le corps de texte est principalement blanc)
- Rose (#E83C68) --> Utilisé pour mettre en valeur certain élément tels que les mots clefs du titre
- Cyan (#01BAB4) --> Utilisé pour les boutons (en background-color) et autres éléments cliquables ainsi que les éléments grec en décoration 

## Les polices & tailles de police
### Fonts utilisés : 
- font-family : **Montserrat** 
    > font principale pour la page 
- font-family : **Alphabet**
    > utilisé que pour les logos des marques 

### Les tailles de polices : 
- **H1** : pixels | Nom du site 
- **H2** : 24 à 36 pixels | Titre de section 
- **H3** : pixels | sous-titre dont le titre des expertises
- **p** : 16 à 20 pixels | corps de text 
- **btn** : 14 à 18 pixels | Bouton 

## Les maquettes :
- la Home page : [ici](https://xd.adobe.com/view/4aecaec8-16cf-41c1-a3b2-4bb464dd69e0-1fbf/)
- page -1 expertises : [ici]()
- page -2 : [ici]()
- page Fundraising : [ici]()

# Eléments techniques : 
## Les "class" elementor 
### selector 
L'attribut selector est intégré à elementor </br>
Les CSS s'applique directement sur l'élément où le code CSS est intégré 

### les autres "class" : 
#### .animation-header
La classe animation-header à ajouter au widget **headline animation** 
- Style : Tournant
- animation : Drop-In 
- Boucle Infini 

````css
/* Animation header */
.animation-header .elementor-headline-dynamic-text:nth-child(1){
    color:#01BAB4;
}
.animation-header .elementor-headline-dynamic-text:nth-child(2){
    color:#fff;
}
.animation-header .elementor-headline-dynamic-text:nth-child(3){
    color:#E83C68;
}
````

#### .expertise-boite

<!-- css à copier et à préciser dans quelles éléments ils sont intégrés!  -->

#### .clickable
Pour rendre une colonne ou une section clickquable, ajouter la class=".clickable" 
La colonne doit contenir au moins un élément cliquable avec un lien ! 
````css
/* Rendre des colonnes cliquables */
.clickable {
    position: relative;
}

.clickable a:after {
    content: "";
    display: block !IMPORTANT;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    z-index: 1;
}
````
