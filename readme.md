# L'Auberge de Peyrabeille

Version électronique du livre que Paul d'Albigny a consacré à l'histoire de la
célèbre auberge "rouge".

Cet ebook est basé sur la 1° édition parue en 1886, disponible sur le site
Gallica de la BNF (http://gallica.bnf.fr/ark:/12148/bpt6k5802450t).


## Numérotation des pages

A l'écran, je fais apparaitre les numéros de pages qui correspondent à la
première édition de 1886. Cela facilite la relecture et la comparaison avec le
texte d'origine.

Ces numéros de page sont masqués à l'impression, car ils ne sont pas
synchronisés avec la pagination obtenue lors d'une impression au format A4
portrait.

Malgré tout, la table des matières indique les numéros de pages de l'édition
originale aussi bien à l'écran qu'à l'imprimante.


## Pages blanches

Dans l'édition d'origine, on trouve des pages blanches avant certains chapitres,
pour que ceux-ci démarrent sur une page de droite. Ces pages blanches sont ici
définies sous la forme : `<div class="blank"></div>` :

* A l'écran, ces pages blanches sont matérialisées par une dizaine de lignes
vides.
* A l'impression, ces pages blanches ne sont pas rendues.

Pour que les nouveaux chapitres commencent sur une page de droite, les titres
`h1` ou `h2.top` en début de chapitre ont une propriété CSS `page-break-before:
right`. Malheureusement, cette propriété n'est pas prise en compte par tous les
navigateurs, la plupart se contentant d'effectuer un saut de page, sans insérer
une page vide pour démarrer sur une page de droite.

Par conséquent, pour avoir au minimum une page blanche au dos de la couverture
(et au dos de la page à propos qui n'existe pas dans l'édition d'origine), une
balise `<div class="verso"></div>` a été utilisée.

A l'écran, cette classe est matérialisée par une dizaine de lignes vides. A
l'impression, elle est rendue sous forme d'une page vide grâce à la propriété
CSS `page-break-before: always`.

A l'avenir, cette classe "verso" pourrait aussi être utilisée pour forcer
manuellement d'autres pages vides là où cela s'avèrera nécessaire dans le cas
d'une impression au format A4 portrait.
