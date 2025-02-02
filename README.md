# Drix Programming Language

## Introduction
Drix est un langage de programmation simple, puissant et intuitif, conçu pour être utilisé dans le noyau Darix. Il privilégie la lisibilité, l'efficacité et la facilité d'utilisation tout en se distinguant des langages existants. Drix permet d'écrire des programmes tant au niveau système qu'utilisateur et s'intègre de manière transparente avec le noyau Darix.

## Principes Clés
- **Simplicité** : Drix doit être facile à apprendre et à utiliser, y compris pour les débutants.
- **Puissance** : Drix prend en charge un large éventail de fonctionnalités pour écrire des programmes robustes.
- **Lisibilité** : La syntaxe doit être claire et intuitive.
- **Unicité** : La syntaxe de Drix ne doit pas ressembler aux langages existants.

## Format des Fichiers
- **Extension** : Les fichiers écrits en Drix doivent utiliser l'extension `.drix`.
- **Encodage** : L'encodage UTF-8 est utilisé pour prendre en charge des symboles spécifiques.

## Exemple de Code
```drix
start (
    set x -> 10
    set y -> 20
    set result -> x + y
    use-output result
)
```

## Syntaxe de Base
### Mots-Clés
- `start` : Définit le début d'un programme.
- `set` : Assigne une valeur à une variable.
- `loop` : Définit une boucle itérative.
- `use-output` : Affiche une valeur à l'utilisateur.
- `use-input` : Demande à l'utilisateur d'entrer une valeur.

### Délimiteurs
- Les blocs de code sont entourés par `(` et `)`.

### Variables
- Les variables sont dynamiquement typées.
- L'affectation se fait avec l'opérateur `->`.
- La concatenation des variables se fait avec `[` et `]`

## Fonctionnalités du Langage
### 1. Variables
#### Déclaration et Assignation
```drix
start (
   set x -> 10
   set name -> "Drix"
)
```

#### Utilisation
```drix
use-output x
```

### 2. Boucles
#### Itération Fixe
```drix
loop 3 (
    use-output "Ce message sera affiché trois fois"
)
```

### 3. Entrée/Sortie
#### Affichage
```drix
use-output "Bonjour, tout le monde !"
```

#### Entrée utilisateur
```drix
use-input "Entrez votre nom :" -> name
use-output "Bienvenue [name]"
```

### 4. Opérations Mathématiques
#### Opérateurs Supportés
- Addition : `+`
- Soustraction : `-`
- Multiplication : `*`
- Division : `/`

#### Exemple
```drix
set result -> 10 + 5
use-output result

```

## Interprétation du Code
### Processus d'Exécution
1. Chargement du fichier `.drix` en mémoire.
2. Analyse syntaxique et transformation en tokens.
3. Exécution des instructions associées aux tokens.

## Exemples de Programmes
### 1. Affichage "Hello, World!"
```drix
start (
    use-output "Hello, World!"
)
```

### 2. Calcul de Factoriel
```drix
start (
    set n -> 5
    set result -> 1
    loop n (
        set result -> result * n
        set n -> n - 1
    )
    use-output "Factoriel : [result]"
)
```

### 3. Interaction avec l'Utilisateur
```drix
start (
    use-input "Quel est votre nom ?" -> name
    use-output "Bonjour, [name] !"
)
```

## Conclusion
Drix est un projet initié récemment avec l'objectif de fournir un langage simple et efficace. Cette documentation doit permettre une prise en main rapide et complète du langage.

### Les structures conditionnelles, les boucles infinies et de nombreuses ameliorations sont à venir!
