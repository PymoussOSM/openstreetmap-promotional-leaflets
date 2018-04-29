# OpenStreetMap Promotional Leaflets

![photo](https://raw.github.com/gravitystorm/openstreetmap-promotional-leaflets/master/leaflets.jpg)

![photo](https://raw.github.com/gravitystorm/openstreetmap-promotional-leaflets/master/leaflets2.jpg)

Ce dépot contient les fichiers source d'un flyer OSM (en français)
créé à l'origine par Frederik Ramm <frederik@remote.org> et
des contributeurs de la liste talk-de en janvier 2008, puis
mis à jour, traduit, re-mis à jour et re-traduit au cours des 
années. Cette version a été téléchargée sur Github par Andy Allan <andy@gravitystorm.co.uk>
et plus tard modifié à nouveau par Frederik Ramm pour FOSSGIS.

Tous les contenus sont dans le domaine public sauf ceux dérivés de OSM
qui sont CC BY-SA et sauf pour les logos non-OSM.

Le dépliant est conçu pour le format DIN A7 en taille finale (105mm de haut et 74mm de large),
avec 8 pages dans un pli en zigzag ("Leporello"), et impression en couleur.

Le dépliant a été fait avec Inkscape ; osmflyer1.svg et osmflyer2.svg
sont les faces avant et arrière.

Quelques remarques au cas où vous voudriez le recréer vous-même :

* `berlin-background.png` est essentiellement un rendu Osmarender de Berlin datant de 4 ans,
utilisant une feuille de style standard mais avec toutes les légendes supprimées,
et le fichier PNG résultant traité avec Gimp comme ceci :

  Convertissez d'abord en niveaux de gris, puis utilisez `couleurs-> curves`
pour réduire le contraste, puis revenez en RVB, puis utilisez` colors-> colorify`
pour lui donner une belle teinte.

* L'image du globe en couverture a été faite avec Marble, la technique est grossièrement décrite ici : http://wiki.openstreetmap.org/wiki/Marble

* Pour générer les cartes png haute résolution, utilisez les commandes suivantes
`~/src/nik2img/nik2img.py -d 2479 1356 -z 14 -c -0.128056 51.508056 --scale-factor 3 ~/src/openstreetmap-carto/osm-carto.xml london.png`
`~/src/nik2img/nik2img.py -d 1974 2902 -z 15 -c -3.19864 55.95 --scale-factor 3 ~/src/openstreetmap-carto/osm-carto.xml edinburgh.png`
