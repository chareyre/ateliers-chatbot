# Quelques exercices sur les bases de RiveScript

## C'est quoi RiveScript ?

RiveScript est un **langage de programmation** qui sert à programmer des **chatbots**.

## Le RiveScript Playground

Pour commencer à utiliser RiveScript, une bonne solution est d'aller sur l'*aire de jeu RiveScript* : [play.rivescript.com](http://play.rivescript.com).

Une fois sur cette page, supprimez tout le contenu de la zone jaune et cochez la case `UTF-8 Mode` située en bas à gauche.

Pour la suite on écrira notre code dans la partie de gauche (jaune), et on appuiera sur `Run` pour le tester dans la partie droite.

## Premiers pas

Écrivons notre premier code RiveScript !


```
+ salut robot
- Salut humain !
```

Écrivez ce code dans la partie jaune du *RiveScript Playground*, puis appuyez sur `Run`.

Maintenant écrivez "Salut robot." et appuyez sur `Send`. Le robot vous répond !

![](img/cde1.png)


### Explication du code

Dans un code RiveScript, chaque ligne est une commande. Pour savoir de quelle type de commande il s'agît il suffit de regarder le symbole en début de ligne (dans cet exemple on voit les symboles `+` et `-`).

#### Commande de déclencheur `+`
La commande `+` sert à définir un **déclencheur**. Un déclencheur est une ligne de texte qui sert à reconnaître le message de l'utilisateur.

#### Commande de réponse `-`
La commande `-` sert à définir les réponses au déclencheur.

### Important !

**Un déclencheur doit toujours être écrit en minuscule et sans ponctuation !**

Les apostrophes `'` et les tirets `-` ne posent pas de problèmes, mais si vous mettez une majuscule ou encore un point dans un déclencheur, cela va créer une erreur qui vous empêchera de tester le code. 
Par contre on peut mettre des majuscules et des signes de ponctuation dans les commandes de réponse.

```
+ Tu as l'air d'aller bien.
- Bof...
```

Revenez dans la partie jaune en cliquant sur `Stop Running`, puis essyez de cliquer sur `Run`. Une erreur apparaît alors.
Essayez de corriger la ligne qui commence par + de manière à ce que la commande de déclencheur ne contienne plus de majuscule ni de signe de ponctuation. Essayez de nouveau d'appuyer sur `Run`, normalement il ne devrait plus y avoir de message d'erreur.

### Plusieurs réponse pour un même déclancheur

Un même déclencheur peut avoir plusieurs réponses possible, il suffit de mettre plusieurs *commandes de réponse*.

Par exemple, complétez le code précédent en rajoutant deux réponses comme suit:
```
+ tu as l'air d'aller bien
- Bof...
- Bien et toi ?
- Oui je vais super bien !
```
Puis essayez de tester le code en appuyant sur `Run` puis en lui demandant plusieurs fois d'affilé "ça va ?"

Quand il y a plusieurs réponses possibles à un même déclencheur, le robot choisira une réponse au hasard parmis elles.

### Partager le code

Avant de partager votre code il y a deux petites dernières choses à faire :

#### Indiquer la version de RiveScript utilisée

Nous utilisons la version 2.0 de RiveScript, le RiveScript Playground est au courant mais il faut l'indiquer pour d'autres programmes qui ne le sauraient pas.

Entrez cette ligne tout en haut de votre code, à la première ligne :
```
! version = 2.0
```

#### Décrire le rôle du code

Pour que les personnes qui liront votre code puissent se faire une idée de ce à quoi il sert, il est bon d'ajouter un petit commentaire pour le leur expliquer. En RiveScript, les commentaires commencent par `//`. Vous pouvez par exemple écrire :

```
// Ce code permet de répondre à des salutations basiques.

```
Les commentaires ne changent rien au code, quand l'ordinateur "lit" (on dit aussi "exécute") le code et qu'il arrive à une ligne qui commence par '//', il comprends que c'est juste une ligne écrite pour les humains, du coup il ne la lit pas et passe à la ligne suivante. 

#### Mon code ressemble donc à ceci :

```
! version = 2.0
// Ce code permet de répondre à des salutations basiques.

+ salut robot
- Salut humain !

+ ça va
- Oui je vais super bien !
- Bof...
- Bien et toi ?
```

#### Enfin

J'appuie sur `Share` et j'obtiens un lien que je peux partager à qui je veux.

![](img/cde2.png)

### La suite...

RiveScript est un language puissant qui permet de faire beaucoup plus de choses que ce qu'on a vu là. Essayez déjà d'exploiter un maximum ce que vous avez appris ici, puis passez à la suite : [Uttilisation avancée de RiveScript](rivescript-avance.html)
