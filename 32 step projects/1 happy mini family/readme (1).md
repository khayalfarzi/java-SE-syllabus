# The "Happy Family" Mini-Project strikes again!

The idea of the project is to describe the structure of a family while taking into account that every human has relatives and the family members can change over time.

# Getters/setters
## The task:

Improve the project:
- Make all the fields private
- Create and describe a Family class. Let's say that a family can be created by 2 people who do not fall apart and can give birth to/adopt their children. Children can grow up and leave the family, creating their own.

- Redefine `equals()` and `hashCode()` methods in all project classes.
- Add the method `deleteChild(Human child)` to the `Family` class, while taking the availability of these methods into account.

#### Technical requirements:
- Declare all the fields of existing classes as private. Add getters and setters, refactor the existing methods to reflect the changes.
- Add the following fields of the `Family`: class
  - mother - `mother` (type `Human`)
  - father - `father` (type `Human`)
  - children - `children` (array `Human`)
  - pet - `pet` (type `Pet`)
- Add getters and setters, redefine `toString` so that it would show all the info about all the family members
- Make a constructor in the `Family`
  - The only condition for creating a new family is the presence of two parents, with the parents being referred to the current new family and the family being created with an empty array of children.
- Refactor the `Human` class, while taking the `Family` structure into account:
  - Remove all information duplicated in the Family class from Human (Human should only keep the information that describes itself)
  - add the `family` (type `Family`) field (now it stores all the information about the family data of a person)
  - add necessary getters, setters, constructors; remove irrelevant constructors and methods; make refactoring of the  ` to welcome the favourite `, ` to describe the favourite `, ` to feed ` methods
  - refactor the `toString()` method. It should output info in the following format:
  `Human{name='Name', surname='Surname', year=1, iq=1, schedule=[[day, task], [day_2, task_2]]}`
  - Add the following methods in `Family`:
  - add a child - `addChild` (accepts the `Human` type and adds it to the children array; adds a link to the current family to the child)
  - delete a child -  `deleteChild` (accepts and array index and deltes the following element; returns a boolean value - was the element deleted or not)
  - get the amount of family members - `countFamily` (the parents in the family never change. If the parents do change - it's a different family)
  - redefine the `toString()` method
  - Decide which fields to use for comparison in the `equals()` method (for example, animal habits may change).
  
Methods should not only add/remove items to the `Human` array, but also make the necessary modifications (to the added/removed item to set/remove the link to the current family). When deleting an item, there should be no empty spaces in the array - a new array should be created.  

#### Advanced complexity. Not necessary to implement:
- Add a  `deleteChild`(`deleteChild`) method to `Family` (accepts the Human type and deletes the corresponding element). The method should be written taking  `equals()` and `hashCode()` into account

   **Hint**: In order to remove the correct element from the Human array, you need to make comparisons by fields that identify the person (think about which fields are suitable for this purpose).
   
- Add a static and a non-static initialisation block 
  - The static block should display the information that a new class is being loaded (specify the class name).
  - The non-static block should display information that a new object is created (specify the object type).


#### Литература:
- [Encapsulation. Getters/setters](https://www.geeksforgeeks.org/encapsulation-in-java/)
- [Method Overloading(https://beginnersbook.com/2013/05/method-overloading/)
- [Overriding equals() and hashcode()](https://www.mkyong.com/java/java-how-to-overrides-equals-and-hashcode/)
- [Comparing Java objects with equals() and hashcode()](https://www.javaworld.com/article/3305792/learn-java/java-challengers-4-comparing-java-objects-with-equals-and-hashcode.html)
- [Java Best Practices: equals() and hashCode()](https://www.intigua.com/blog/good-and-bad-equals-and-hashcode)
- [Java static constructor](https://softwareengineering.stackexchange.com/questions/228242/working-with-static-constructor-in-java)
- [Static and non-static initialization blocks](https://www.quora.com/What-is-difference-between-non-static-block-and-instance-initialize-block)
