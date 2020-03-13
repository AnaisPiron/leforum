# LES DIRECTIVES D'ANYSURFER TESTÉES SUR LE SITE DU FORUM DE LIÈGE
> [Retourner à la racine du repo Le Forum](../../..) \
> Liens : [Les directives d'AnySurfer](https://www.anysurfer.be/fr/en-pratique/directives) & [Le Forum de Liège](https://www.leforum.be/)

## Navigation
### 1.1 La totalité du site est utilisable au moyen du clavier `NON`

Certaines balises sont visibles quand on navigue au clavier (c-à-d avec le TAB) telles que le menu principal.
Mais les liens et les boutons ne sont absolument pas visible sauf si on regarde le lien en bas à gauche de l'écran qui montre le href du lien sur lequel on se trouve). 

Voici un aperçu de ce que l'on voit lorsqu'on TAB :

<img src="./img/navigation_clavier.gif" height="250" width="auto" alt="Le site n'est pas navigable au clavier" />

### 1.2 Les intitulés des liens sont significatifs dans leur contexte `NON`

Les liens (et boutons) ne nous indiquent absolument pas à quoi font référence les liens cliquables.

"réservation" de quoi exactement ?
                    

### 2.1 Le code source est conforme à la spécification du langage `NON`

Voici l'outline du site du Forum de Liège (outline incorrect) :

<img src="./img/outline_leforum.png" alt="an incorrect outline in HTML" width="450" />

Voici l'outline du site d'AnySurfer (outline correct) :

<img src="./img/outline_anysurfer.png" width="350" alt="a correct outline" />

En utilisant le [validateur HTML du W3C](https://validator.w3.org/) pour contrôler chaque page,
nous pouvons constater que le site du forum dépasse la centaine d'erreurs :

<img src="./img/error_test_forum.png" alt="an incorrect outline in HTML" height="250" width="auto" />

En comparaison avec le site du W3C :

<img src="./img/error_test_w3.png" alt="an incorrect outline in HTML" height="250" width="auto"/>

Un même ID est utilisé plusieurs fois. Il manque des ALT dans les images.
Il n'y a pas de header correct. 

### 2.2.1 Chaque page possède un titre significatif `NON`

Aucune des pages n'a de TITLE correct :


<img src="./img/page_title.png" alt="incorrect title pages"/>

Soit ils écrivent uniquement le nom du site, soit le titre de la page.

### 2.2.2 Les pages sont structurées par la sémantique `NON`

Le site n'est constitué que de DIV avec des ID et des liens.

<img src="./img/semantique.png" alt="incorrect title pages" height="250" width="auto"/>

### 2.2.3 La langue principale de chaque page est indiquée `NON`

<img src="./img/langue.png" alt="incorrect title pages" height="auto" width="350"/>

### 2.3.1 Chaque image a un attribut alt `NON`
### 2.3.2 Les images complexes sont décrites par un texte `NON`
### 2.3.3 Les images d'arrière-plan qui contiennent de l'information ont une variante accessible `NON`


Aucune des images n'a d'alternative textuelle. 

### 3.1.1 Les liens sont facilement identifiables comme tels `NON`

Il y en a qui sont bien visibles et soulignés mais pas d'autres. Ils ne sont pas assez mis en valeurs. Certains liens ne sont même pas soulignés et sont confondus avec des textes en gras dans le texte courant.

### 3.2.1 Le contenu de la page suit un ordre logique `NON`

<img src="./img/css_disabled.gif" alt="page illogique sans css" height="auto" width="350"/>

### 4.1.1 Les labels et éléments des formulaires sont intimement liés `NON`

Aucun LABEL donc aucune liaison :

<img src="./img/label_form.png" height="auto" width="450"/>

### 4.1.2 Les champs sans label sont décrits par un tooltip `NON`

Absolument pas, il n'y a que des HOVER ! Et une fois qu'on a cliqué, ça disaprait et n'apparait plus.

<img src="./img/label_form.gif" height="auto" width="450"/>

### 4.1.8 Lors de la validation, les erreurs sont indiquées et expliquées par du texte `NON`

La seule erreur est une ALERT qui dit "veuillez saisir votre nom et prénom" :

<img src="./img/form_alert.png" alt="Veuillez saisir votre nom et votre prénom" height="auto" width="450"/>
