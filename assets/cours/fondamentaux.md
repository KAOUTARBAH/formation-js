# Les fondamentaux : Variables, Opérateurs et Types

En javascript, comme tout les langages de programmation, il éxiste 3 notions fondamentales : Types, Opérateurs et variables

## Les Types

Un « type », c'est comme une grosse famille contenant certaines données. Parmis ces familles et éxiste 2 branches :

### les types primitifs

Voici les différentes primitif :

1. `number` (représente n'importe quelle nombre)
2. `boolean` (représente une données vrai ou fausse)
3. `string` (représente n'importe quel texte)
4. `undefined` (représente une valeur non définie)
5. `null` (représente une valeur définie, mais qui ne contient rien)

### Les types complexe

1. `array` (ce sont des tableaux)
2. `objets` (ce sont des groupement de données)
3. `function` (ce sont des boites de codes réutilisable)

## Les numbers

Représente l'intégralité des nombres immaginable :

```js
125 // Nombre 125
125.36
65.8 - 85 - 85.63
```

> **Pour faire un nombre à virgule il faut utiliser "."**

> **Pour faire un nombre négatif il est obligatoire de « coller » le signe moins au nombre**

Il éxiste 2 `number` un peu particulier :

1. L'infinie : `Infinite` (`-Inifinite`)
2. Un opération qui échoue : `NaN` (`Not A Number`), c'est le nombre retourné lorsque l'on fait une division par `0`.

### Les oopérateurs sur les nombres :

On peut réaliser des opérations sur les nombres :

```js
52 + 12 // Addition
12 - 5 // soustraction
12 * 2 // Mutliplication
53 / 2 // Division
53 % 3 // Reste d'une division euclidienne
10 ** 2 // Puissance
10++ // Incrémentation avec retour initiale (Ajoute 1 à 10, 10 + 1)
++10 // Incrémentation avex retour finale (Ajoute 1 à 10)
10-- // Décrémentation avec retour initiale (Enléve 1 à 10, 10 - 1)
--10 // Décrementation avec retour finale (Enléve 1 à 10)
```

## Les booleans

Les « booleans », sont inventé par un mathématicien Anglais : « James Bool ». C'est une algébre basé sur 2 valeurs : Le vrai et le faux. C'est les fondations de l'informatique !

En informatique, certaines données peuvent « vrai » ou « fausse » :

```js
true // vrai (1)
false // faux (0)
```

### Les opérateurs logique

Les opérateur logique nous permette de « combiner » des valeurs vrai ou fausse :

```js
true && false // ET (false)
true && true // ET (vrai)
false && true // ET (false)

true || false // OU (vrai)
true || true // OU (vrai)
false || true // OU (vrai)
false || false // OU (faux)

!true // NON VRAI (false)
!false // NON FAUX (vrai)
```

> **Le non (`!`) doit être collé au boolean pour fonctionner !**

### Les opérateurs de comparaisons

Les opérateurs de comparaisons permettent de comparéer des données entre elle :

```js
10 > 12 // Supérieur (false)
10 < 12 // Inférieur (true)
10 >= 10 // Supérieur ou égale (true)
10 <= 12 // Inférieur ou égale (true)
10 == 10 // Égale à (true)
10 === 10 // Identique à (true)
10 != 10 // N"est pas égale (false)
10 !== 10 // N'est pas identique à (false)
```

## Les strings

Les string (chaînes de caractères) sont un type de données permettant de représenter du texte. Pour représenter du texte, il faut utiliser les caractères suivants :

- `""` les guillemets double
- `''` les guillemets simple
- `` Les backtick (alt gr - 7)

### Exemple

```js
'Coucou les amis'
"J'ai 19 ans"`Je suis aussi du texte`
```

> Attention, les guillemets (double ou simple) ne fonctionne que sur 1 seule ligne !

```js
"coucou
les
amis" // Erreur impossible de faire plusieurs ligne !
```

```js
;`Coucou
les
amis` // Fonctionne très bien !
```

### Egalité vs Identité

Attention, nous avons vue 2 opérateurs de comparaison : l'égalité (`==`) et l'identité (`===`) :

```js
10 == '10' // true (égalité)
10 === '10' // false (identité, égalité + même type)
```

### Les opérateurs sur les string

Il est possible « d'assembler » plusieurs texte ensemble, de les réunir. On appel ce phénoméne : `concaténation`

```js
'Coucou' + ' les amis' // 'Coucou les amis'
'Coucou' + 'les amis' // "Coucoules amis"
'Coucou' + ' ' + 'les amis' // 'Coucou les amis'
```

## Le `null` et `undefined`

Le `null` et `undefined` sont généralement utilisé par javascript pour symboliser des valeur vide ou non définie. On les utilises très rarement, cependant nous verrons que nous pouvons souvent les rencontrer.

Elles s'écrivent comme le nom l'indique :

```js
null // null
undefined // undefined
```

### La coerscion

Il éxiste un petit opérateur : `?` permettant de choisir la valeur non null ou undefined d'un couple :

```js
null ? "coucou" // "coucou"
undefined ? "salut" // "salut"
"coucou" ? null // "coucou"
"salut" ? undefined // "salut"
```
