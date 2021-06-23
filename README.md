# DesignPattern

## Loi DEMETER
Lorsqu'on crée des classes on ne fait pas toujours attention aux dépendances
- une classe peut utilize d' autre classe, par agrégation, soit par passage de params par méthodes
- une classe A utilise une classe B
- une méthode de B utilise une classe C ==> La classe A va donc utiliser la classe C

 Loi DEMETER : chaque classe doit avoir une connaissance limitée des autres classes
 --- une clqsse ne doit parler qu' à ses amis
 En pratique: une méthode d'une classe peut invoker les methodes:
 - de l'objet
 - les arguments de la methode
 - des objets crées dans la methode
 - des propriétes ou des champs de l'objet

## Tell, Don't Ask
- Dite et ne demande pas le status de votre objet
- 

## Les principes SOLID 
S: Single of Responsability

O: Open/Close

L: Liskov Substitution

I: Interface

D: Dependency Injection

Ce sont de bonnes pratiques à appliquer dans le conception des objets

Quote: " N' importe qui peut ecrire un code q'une machine. Un bon dev c' est quelqu'un qui ecrit un code qu' un etre humain peut comprendre"

**Intérêt**: permette d' ameliorer la cohésion, de dimunier le couplage et de favoriser l' encapsulation d' un programmme objet.

**Cohésion**: un modules (classe ou ensemble de classe) est dit cohesif s'il ne fait qu'une seule et unique tâche précise.

**Open/close**: une classe doit rester ouverte à l' extension mais fermer à la modification.

**LISKOV SUBSTITUTION** : les sous-types doivent être subtituable à leur type de base

Dans un code, remplacer un objet parent


Solution: les classes enfants doivent garder l' implementation de la classe parent.

**Interface Segregation**
**Dependancy injection** Typer avec les interfaces
- Cas 1  injection par constructeur ---> un objet de type UserService est creée dans un état stable, la dépendance est inectée et initialisée
- Cas 2  injection par paramètre de la méthode

Avantage: à chaque appel de la méthode on a la possibilité de changer de dependance
Contrainte: dépendance à fournir à chaque appel de la methode

- Cas 3 injection par setter (approche très rare, à utiliser si vous êtes contraints)
Avantage: possilité de changer de dépendance
Contrainte: on doit s' assurer que la dépendance a été injectée



# Design Pattern (DAO, Repo,...)
Solution classique à des probèmes de conceptions objet récurrents.

**GOF: Gang of Four** -- 4 auteurs qui ont écrit un livre qui détail les differents patterns

- Pattern de création: singleton, Builder, Factory, Prototype
- Pattern Behavior: Proxy, observer, Adapter, State, Memento, Chain of Responsability
- Pattern de structure: Mediator, Visitor, Iterator, Strategy, Command

## Singleton:
**Problème** : garantir l' existance d'une et unique instance d'une 
Eg: une sociéteé ne peut avoir qu' un seul et unique Directeur 

Garantir l' existance d' un instance de cette classe

Pas d' accès au constructeur --> une var static pour avoir l'instance unique --> verouiller la ressource











