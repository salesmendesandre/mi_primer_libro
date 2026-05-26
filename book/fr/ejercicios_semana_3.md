# Exercices Semaine 3 : Programmation III

CONTENU : Classes Wrapper et premiers exercices de POO

## Exercices obligatoires :

1. Vous devez créer une classe `Person.java` avec les attributs nom, taille et poids, ainsi que leurs getters et setters correspondants. Dans la méthode principale, vous devez instancier 3 objets de cette classe et compléter leurs informations en les demandant à l'utilisateur via la console pour chaque objet. Enfin, vous devez afficher dans la console qui est le plus grand et qui pèse le plus. Vous devez toujours utiliser les getters et setters pour obtenir et définir les informations.

2. Améliorez l'exercice 1 pour qu'il existe un constructeur sans paramètres qui initialise les valeurs de nom, taille et poids à des valeurs par défaut que vous jugez appropriées.

3. Améliorez l'exercice 1 pour que la classe `Person` propose une méthode calculant l'IMC de la personne à travers les valeurs actuelles des attributs de l'objet (son état). Il faut envisager la possibilité que les valeurs n'aient pas été initialisées avec des valeurs valides.

4. Analysez le flux d'exécution du programme en plaçant des points d'arrêt dans le constructeur et dans les différentes parties du code de l'exercice 1. Définissez des valeurs aux attributs directement lors de leur déclaration et vérifiez ce qui s'exécute en premier : le constructeur ou la déclaration de l'attribut.

## Exercices d'extension :

5. En utilisant les méthodes `parseXXX` des classes wrapper, construisez une classe dotée de méthodes adéquates pour lire tous les types de données numériques (`int`, `float`, `double`) sous forme de chaînes de caractères. Si l'utilisateur n'insère pas de valeur valide, demandez à nouveau.

6. Modifiez l'exercice 1 pour que la classe `Person.java` se trouve dans un package appelé `model` au lieu du même package que la classe `App.java`. Qu'avez-vous dû changer pour l'utiliser dans `App.java` ?

7. Quelle est la différence entre le constructeur par défaut d'une classe en Java et un constructeur sans paramètres ?

8. Pourquoi utiliser des getters et des setters au lieu d'accéder directement aux attributs via le point ? Encapsulation. Est-ce une question de sécurité ou de conception ?

9. Quelle est la différence entre définir un attribut comme `public`, `private` ou sans modificateur de visibilité ? Dans quel cas est-il possible d'y accéder via le point (.) avec une référence d'objet ?

10. À quoi sert le mot-clé `this` ? Et le mot-clé `new` ?

11. Il est possible de définir des classes qui ont à leur tour des attributs d'autres classes (appelé Composition). Vous devez maintenant modifier l'exercice 1 pour que la classe `Person` ait un attribut de type `DNI` (une autre classe que vous devrez créer) qui aura comme attributs numéro et lettre. Au constructeur de la classe `Person`, vous devrez passer en paramètre un numéro de DNI et un objet de type `DNI` sera créé, générant la lettre correspondante à partir de l'algorithme. Consultez l'opérateur `%` en Java.

12. Créez une classe appelée `Rectangulo.java` avec les attributs longueur et largeur, chacun avec une valeur par défaut de 1. Elle doit avoir des méthodes pour calculer le périmètre et l'aire du rectangle, ainsi que des getters et setters. Les setters doivent vérifier que la longueur et la largeur sont des nombres à virgule flottante supérieurs à 0.0 et inférieurs à 20.0. Écrivez un programme pour tester la classe `Rectangulo`.

13. Créez un nouveau projet avec la classe `Person.java`. Réalisez les instructions suivantes et répondez aux questions posées.

```java
public static void main(String[] args) {
    // Création d'un objet de la classe Person
    Person paco = new Person("Paco", 22, 177.3f, 82.3f);

    // Nous copions la référence de l'objet précédent vers une autre référence
    Person refPaco2 = paco;

    // Nous utilisons la deuxième référence pour définir une valeur
    refPaco2.setAgeYears(77);

    // Résultat ?
    System.out.printf("L'âge de %s est:%d%n", paco.getName(), paco.getAgeYears());

    // Quel est l'âge affiché ?
    // Combien d'objets y a-t-il en mémoire ? Combien de références ? Vérifiez le débogueur
}
```
