# Uttilisation avancée de RiveScript

## Des déclancheurs plus puissants (Les Jokers)

Pour l'instant on avait des déclancheurs qui ne marchaient que quand l'utilisataur écrivait exactement le même message.

Mais pour pouvoir être capable de répondre à un maximum de message, il va falloir trouver un moyer d'écrire des déclancheurs plus souples.

C'est là qu'interviennent les Jokers.

### L'étoile `*`

Essayons ce bout de code :

```
+ je mappelle *
- Oh ! C'est un très joli prénom !
```

Si je test ce code je verrai que le robot répondra "Oh ! C'est un très joli prénom !" quelque soit mon prénom. Que j'écrive "Je m'appelle Sofiane", "Je m'appelle Lola" ou encore "Je m'appelle voiture de course"

Enfait, le symbole `*` veut dire "n'importe quoi"

#### Autres exemples 

```
+ * est très beau
- Je ne le trouve pas si beau que ça
```

```
+ jai * ans
- Moi je suis beaucoup plus jeune que ça !
```

```
+ * rouge *
- Le rouge c'est ma couleur préféré !
```

#### Le déclancheur *fourre-tout*

Jusqu'à maintenant, quand on disait au robot une phrase à laquelle il ne savait pas répondre, il y avait une erreur (`ERR: No Reply Matched`).

L'étoile peut nous permette de crééer un déclancheur qui se déclanche à chaque fois que le robot n'a rien à dire :

```
+ *
- Je ne sais pas trop quoi dire...
- Parlons d'autre chose !
```

#### Récupérer le contenu de l'étoile

```
+ je mappelle *
- Tu es la première personne que je rencontre qui s'appelle <star>
```

Ça donnera la discussion : "Je m'appelle Kévin", "Tu es la première personne que je rencontre qui s'appelle Kévin"