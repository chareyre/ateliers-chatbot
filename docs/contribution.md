# Les règles de contribution

### Préparer le code

Avant de partager votre code il y a quelques étapes importantes à respecter :

-1 - Commenter (mettre le bon numéro de version dans les commentaires)
-2 - Mettre en page
-3 - Tester de fond en comble
-4 - Supprimer les tableaux dont on s'est servi pour tester




#### Commenter : Décrire le rôle du code

Pour que les personnes qui liront votre code puissent se faire une idée de ce à quoi il sert, il est bon d'ajouter un petit commentaire pour le leur expliquer. En RiveScript, les commentaires commencent par `//`. Vous pouvez par exemple écrire :

```
// Ce code permet de répondre à des salutations basiques.
```

Les commentaires ne changent rien au code, quand l'ordinateur "lit" (on dit aussi "exécute") le code et qu'il arrive à une ligne qui commence par '//', il comprends que c'est juste une ligne écrite pour les humains, du coup il ne la lit pas et passe à la ligne suivante. 

#### Mettre en page
On saute une ligne entre chaque bloc de question réponse.
Si le code est long, on fait plusieurs parties avec un commentaire qui sert de titre de la partie et 3 sauts de ligne entre chaque partie.

#### Tester : chercher les bugs

Lancer le code et voir si tout se passe comme prévu.

### Mon code ressemble donc à ceci :

```
// Salutations
//V3
//Nom du groupe et des élèves
// Ce code permet de répondre à des salutations basiques.

//Quand on salue
+ salut robot
- Salut humain !

+ bonjour robot
- Bonjour humain !



//Quand on demande comment ça va 
+ ça va
- Oui je vais super bien !
- Bof...
- Bien et toi ?

+ ça va pas
- Non pas trop
- Non, j'ai la grippe.
```

#### Enfin

J'appuie sur `Share` et j'obtiens un lien que je peux copier dans le pad.

![](img/cde2.png)

