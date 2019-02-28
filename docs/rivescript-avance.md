# Utilisation avancée de RiveScript

## Des déclencheurs plus puissants (Les Jokers)

Pour l'instant on n'a vu que des déclencheurs qui ne marchaient que quand l'utilisataur écrivait exactement le même message.

Mais pour pouvoir être capable de répondre à un maximum de messages, il va falloir trouver un moyen d'écrire des déclencheurs plus souples.

C'est là qu'interviennent les Jokers.

### L'étoile `*`

Essayons ce bout de code :

```
+ je m'appelle *
- Oh ! C'est un très joli prénom !
```

Si je teste ce code je verrai que le robot répondra "Oh ! C'est un très joli prénom !" quelque soit mon prénom. Que j'écrive "Je m'appelle Sofiane", "Je m'appelle Lola" ou encore "Je m'appelle voiture de course"

En fait, le symbole `*` veut dire "n'importe quelle suite de lettres"

#### Autres exemples d'utilisation de `*`

```
+ * est très beau
- Je ne le trouve pas si beau que ça.
```

```
+ jai * ans
- Moi je suis beaucoup plus jeune que ça !
```

```
+ * rouge *
- Le rouge c'est ma couleur préféré !
```

#### Le déclencheur *fourre-tout*

Jusqu'à maintenant, quand on disait au robot une phrase à laquelle il ne savait pas répondre, il y avait une erreur (`ERR: No Reply Matched`).

L'étoile peut nous permette de créer un déclencheur qui se déclenche à chaque fois que le robot n'a rien à dire :

```
+ *
- Je ne sais pas trop quoi dire...
- Parlons d'autre chose !
```

#### Récupérer le contenu de l'étoile

Nous avons vu que l'étoile voulait dire "n'importe quelle suite de lettres". On peut récupérer la suite de lettres qui a déclenché une étoile et s'en servir dans la réponse. Par exemple:

```
+ je m'appelle *
- Tu es la première personne que je rencontre qui s'appelle <star>
```

Ça donnera la discussion :
"Je m'appelle Kévin"
"Tu es la première personne que je rencontre qui s'appelle Kévin"
