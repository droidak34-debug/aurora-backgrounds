# Arrière-plans d'Aurora Player

Photos d'aurores boréales affichées sur l'accueil d'Aurora Player (mode « Aurores boréales », réglage par défaut) :
elles défilent au hasard toutes les 10 s, avec le nom du lieu juste au-dessus de la barre de l'accueil.
L'appli en contient 3 (01 à 03) et télécharge les autres d'ici, une seule fois.

- `tv/tv_NN.jpg` : version paysage (1920×1072) — Android TV, Samsung, LG, VIDAA
- `tel/tel_NN.jpg` : version portrait (1072×1920) — téléphones (et mode téléphone)
- `manifest.json` : liste des photos par version ; `title` est le lieu affiché

Ajouter une photo : mettre `tv_NN.jpg` dans `tv/` et `tel_NN.jpg` dans `tel/` (1920 px de grand côté, JPEG
qualité 80 environ), puis une ligne dans chacune des deux listes de `manifest.json` (`bytes` = taille du fichier : une photo remplacée sous
le même nom est retéléchargée quand sa taille change). Retirer une ligne de la liste
efface la photo sur les appareils (sauf 01 à 03, fournies avec l'appli). Les applis relisent la liste à chaque lancement.

Photos : © brams (photos personnelles et images créées par IA). Réservées à Aurora Player.
