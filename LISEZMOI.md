# La Grande Chasse

Jeu de chasse en 3D qui tourne dans le navigateur. Tout tient dans `index.html` (three.js r128 est intégré dans le fichier) : aucune installation, aucune dépendance, pas de serveur à faire tourner.

## Contenu

- `index.html` : le jeu complet
- `CNAME` : sous-domaine `lgc.gamzu.fr`
- `.nojekyll` : demande à GitHub Pages de servir les fichiers tels quels
- `capture.jpg` : capture d’écran pour la tuile de la page d’accueil de gamzu.fr

## Déployer sur GitHub Pages

1. Crée un dépôt (par exemple `la-grande-chasse`) et pousse-y le contenu de ce dossier, à la racine.
2. Dans le dépôt : Settings > Pages > Source « Deploy from a branch », branche `main`, dossier `/ (root)`.
3. Chez ton registrar, ajoute un enregistrement DNS `CNAME` : `lgc` vers `<ton-compte>.github.io`.
4. Une fois le DNS propagé, coche « Enforce HTTPS » dans Settings > Pages.

## À savoir

- La partie est sauvegardée dans le navigateur du joueur (localStorage), propre à chaque domaine : une partie commencée ailleurs ne suit pas.
- Seules les polices viennent de Google Fonts ; sans internet, le jeu marche avec des polices de secours.
- Classement partagé de gamzu.fr (`https://gamzu.fr/scores.js`) : le total d’argent gagné est envoyé à chaque vente au comptoir, si le joueur a choisi un pseudo. Le top 10 s’affiche sur l’écran titre et en pause.
- Le jeu se joue au clavier et à la souris, sur ordinateur.
