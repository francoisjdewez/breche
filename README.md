# BRÈCHE

Un jeu de construction et de siège en 3D, jouable directement dans le navigateur.
Bâtis un château pour protéger ton coffre, puis fais tomber celui des autres à la catapulte.

**[Jouer sur itch.io](https://phantomex2.itch.io/breche)**

## Le jeu

- **Atelier** : empile des pièces en pierre ou en bois autour du coffre, puis scelle ton château.
- **Campagne** : assiège 7 forteresses, de plus en plus difficiles, avec un nombre de tirs limité.
- **Partage** : ton château est enregistré dans un lien, qu'un ami peut ouvrir pour l'assiéger.

La physique est simulée : un château mal construit s'écroule vraiment.

## Commandes

| Action | Souris ou doigt | Clavier |
|---|---|---|
| Poser une pièce | Clic ou appui sur le terrain | |
| Tirer | Maintenir, tirer vers le bas, relâcher | |
| Tourner le château | Boutons à l'écran | Flèches gauche et droite |

## Technique

- **Three.js** pour la 3D
- **Rapier** pour la physique
- **lz-string** pour compresser le château dans le lien de partage
- JavaScript sans étape de compilation : tout le jeu tient dans `index.html`

## Lancer le jeu sur son ordinateur

Le jeu doit passer par un petit serveur web : un double-clic sur `index.html` ne suffit pas.
Il faut aussi une connexion internet, car les bibliothèques sont chargées depuis un CDN.

Dans PowerShell, depuis ce dossier :

```powershell
python -m http.server 8000
```

Puis ouvrir <http://localhost:8000> dans le navigateur.

## Droits

Code publié pour être consulté. Tous droits réservés.
