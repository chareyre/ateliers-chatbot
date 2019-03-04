# Les règles de contribution

### Préparer le code

Avant de partager votre code il y a deux dernières choses à faire :

1 - Tester
2 - Commenter

#### Tester : chercher les bugs

Lancer le code et voir si tout se passe comme prévu.

#### Commenter : Décrire le rôle du code

Pour que les personnes qui liront votre code puissent se faire une idée de ce à quoi il sert, il est bon d'ajouter un petit commentaire pour le leur expliquer. En RiveScript, les commentaires commencent par `//`. Vous pouvez par exemple écrire :

```
// Ce code permet de répondre à des salutations basiques.
```

Les commentaires ne changent rien au code, quand l'ordinateur "lit" (on dit aussi "exécute") le code et qu'il arrive à une ligne qui commence par '//', il comprends que c'est juste une ligne écrite pour les humains, du coup il ne la lit pas et passe à la ligne suivante. 

### Des conventions :

Pour que ce soit plus simple on va tous écrire les commentaires de la même manière :

```
// [Sujet]
// [Version] ([date])
// [Nom du groupe], [nom des élèves], [classe et collège]

// [Description du code]

[Le code]
```

Par exemple :

```
// Salutation
// v1 (4 mars 2019)
// Nokill, Fabien Bertrand et Léon

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

Nous allons rassembler tous les liens de vos codes sur un "pad" :

Chacun copie ce lien et le colle sur le pad à une nouvelle ligne
```
- [Sujet] [version] : [lien]
```

Par exemple

```
- Salutation v1 : https://play.rivescript.com/s/Tgm9H81Ovi
```