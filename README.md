## <samp>Les questions Java dans un entretien technique </samp>

- 1 . C'est quoi une classe Java? C’est une template définissant un type de données. Elle est utilisée pour créer des objets.

- 2 . Qu’est-ce qu’un objet? C’est un élément d’une classe (instance)

- 3 . Qu’es-ce qu’une méthode? C’est l’action qu’un objet peut faire.

- 4 . Heap vs Stack
  *  Heap: Lorsqu'un objet est créé, il est toujours créé dans Heap et a un accès global.
  *  Stack: Lorsqu'une fonction est appelée, un bloc est réservé en haut de Stack pour stocker ses variables locales. aussi on trouve les références aux objets stockés dans Heap qui sont utilisés par cette méthode.

- 5 . La différence entre JDK, JVM et JRE:
  *  JDK : Java Devlopment Kit. C’est l’ensemble des packages et programmes qu’on utilise pour écrire nos propres programmes.
  *  JRE : Java Runtime Environment . C’est la couche logicielle fournissant les packages et les ressources nécessaires pour qu’un programme java puisse s'exécuter.
  *  JVM : Java Virtuel Machine. C’est l’environnement dans lequel le code Java (Byte Code) s’exécute.

- 6 . Oracle JDK Vs OpenJDK
  * OpenJDK est une implémentation gratuite et open source de Java SE Platform Edition.
  * Oracle JDK nécessite une licence commerciale.

- 7 . Est-ce que Java utilise les pointeurs? Non, Java importe une couche de sécurité en utilisant les références à la place des pointeurs. Donc pas de pointeurs.

- 8 . les modificateurs d’accès en java: Ce sont les mots clés utilisés pour spécifier l’accès et la porté des objets,
  *  public : les classes, attributs, les méthodes peuvent être utilisés par n’importe quel objet.
  *  protected : Seules les classes du même packages ou des sous-classes qui peuvent utiliser les objets, attributs, méthodes avec ce modificateur.
  *  private: c’est le modificateur le plus restreint, les objets, attributs, méthodes, variables ne peuvent être utilisées que dans la classes où ils sont déclarés.
  *  « nothing » : pas de modificateur ou le modificateur par défaut, la visibilité est restreinte dans le même package.

- 9 . Quelle est la différence entre inner class et subclass?
  *  inner class : ou classe interne, est une classe définie (déclarée) à l’intérieur d’une classe.
  *  subclass : sous classe, est une classe fille d’une classe mère.

- 10 . Qu’est-ce qu’un constructeur? quels sont ses type?
Un constructeur est un bloc de code utilisé pour initialiser un objet. On distingue deux types de constructeur : constructeur par défaut, et constructeur paramètré.

- 11 . Overloading Vs Overriding?
  * Overloading : décrit le fait que deux méthodes (ou plus) peuvent avoir le même nom mais pas les mêmes parametres.
  * Overriding : décrit le fait que deux méthodes (ou plus) peuvent avoir le même nom et les mêmes parametres avec une relation mère-fille entre elles.

- 12 . Quelle est la différence entre equals() et ==?

== | equals() 
--- | --- 
Est un opérateur | Est une méthode
Pour la comparaison des primitives et des objets (leurs réferneces) |  Pour la comparaison de contenu des objets

- 13 . Qu'est-ce qu'un objet immuable ? 
Tu ne peux pas modifier les objets d'une classe immuable une fois qu'ils sont créés. En d'autres termes, une fois que tu les crées, tu ne peux pas les modifier.

- 14 . Qu’est ce qu’un thread?
Thread est une classe permettant d’exécuter un programme. En Java, chaque programme a au moins un thread en cours d’exécution (main). 

- 15 . C’est quoi le Garbage Collector?
C’est un mécanisme défini dans la JVM pour faire le ménage. Si un objet n’est plus utilisé, il sera automatiquement détruit pour libérer les ressources.

- 16 . Qu’est-ce qu’une exception?
C’est un problème qui se produit lors de l’exécution d’un programme, et qui nécessite un traitement spéciale pour le bon fonctionnement de l’application. Ceci peut être réalisé, soit par:
  *  l’envoi de l’exception à un niveau supérieur (throws) 
  *  ou par la capture et le traitement au niveau local (try/catch)

- 17 . C’est quoi une classe abstraite? 
Une abstract class est une classe qui permet de définir une classe sans que cette dernière soit instanciable. Pour l’exploiter il faut absolument passer par l’héritage. C’est une technique qui renforce la programmation orientée-objet POO.

- 18 . C’est quoi une interface?
C’est une classe abstraite, qui permet de regrouper un certain nombre de définition des méthodes sans qu’elle soit instanciée. Pour l’exploiter il faut l’implémenter

- 19 . Quelle est la différence entre une classe abstraite et une interface ?

Classe abstraite	 | Interface
--- | --- 
Les constructeurs sont autorisés	| Une interface ne peut pas avoir de constructeur.
Les méthodes static sont autorisées	| Les méthodes static ne sont pas autorisées
Une classe ne peut avoir qu'un seul parent abstrait | Une classe peut implémenter plusieurs interfaces
Une classe Java abstraite peut avoir des membres de classe private et protected | Les membres d'une interface Java sont public par défaut

- 20 . Peut-on exécuter un programme sans la méthode main ?
la réponse est : oui, c'est possible. Par exemple, nous pouvons le faire à l'aide d'un bloc static.   static{...code}

- 21 . Quelle est la différence entre les classes String, StringBuilder et StringBuffer en Java ?

String | StringBuilder | StringBuffer
--- | --- | ---
String est une classe immuable. | Mutable | Mutable
... | non synchronisée  (not thread safe) | synchronisée  (thread safe)

- 22 . Quelles sont les étapes pour établir une connexion à une base de données?
  *  Enregistrer le driver
  *  Créer la connexion
  *  Créer le statement
  *  Exécuter la requête
  *  Récupérer les résultats ou l’état de l’exécution
  *  Fermer la connexion
