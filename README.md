## Ateliers chatbot

Ce dépot contient un modèle pour organiser le travail et le rendu des ateliers chatbots.

Il contient deux dossiers :

- `docs/` : [la documentation](docs) pour pendant le déroulement de l'atelier
- `www/` : [les pages web](www) qui permettent de faire tourner le chatbot créé pendant l'atelier.

### Usage

Faire un fork de ce dépot et modifier directement les fichiers source :

#### charger les fichiers dans le bot
- Mettre tous les fichiers `.rive` dans le dossier `brain/`
- Lister ces fichiers dans `riveList.js` :
    ```
    const riveList = [
        'brain/fichier1.rive',
        'brain/fichier2.rive',
        'brain/fichier3.rive'
    ];
    ```
- Compléter `index.html` et `about.html` avec les bonnes informations. (Nom du bot, etc.)


### Ressources

- Aire de jeu : https://play.rivescript.com/
- Doc officielle : https://www.rivescript.com/
- Pad : https://etherpad.wikimedia.org/
- Doc Nokill : https://github.com/LeonLenclos/ateliers-chatbot
