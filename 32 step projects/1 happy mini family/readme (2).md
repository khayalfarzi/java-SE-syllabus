# The "Happy Family" Mini-Project strikes again! (again)

The idea of the project is to describe the structure of a family while taking into account that every human has relatives and the family members can change over time.

# Object's life cycle. Garbage colector
## The task:

Redefine the `finalize()` method. 

Improve the project: 
 - implement animal species and timetables for extracurricular activities through the `enum` listings (use the views as you see fit, e.g. `CAT`, `DOG`, etc.)
 - implement unit-tests for every custom project method that can be covered with tests

#### Technical requirements:
- Redefine the`finalize()` method in the `Family`, `Human`, `Pet` classes so that they would output a message about the removal of an object before the garbage collector deletes them,
- Create the right amount of loops in the Main class of the `Human` object so that the garbage collector would start deleting old objects (from 10 thousand untill 10 million, depending on the amount of free ram)
- Create the `enum` `Species` with a list of animal types; add the enumeration at your liking; refactor the `Pet` class - the animal type will changed from the `String` type to a `Species` type
- Create `enum` `DayOfWeek` with a list of the days of the week (all 7 days); when you fill in the `Human` schedule (in the `main` method), use the `name()` enumeration method, which returns the string representation of the current enumeration.
- Add the following methods, while keeping in mind that you may have both a positive and a negative scenario of the execution:
- `toString` - check if the methods return a specific string for a specific object:
  - `deleteChild(Human child)` - do 2 checks: 
    - check if the child is actually being removed from the `children` array (if you pass an object that is equivalent to at least one element of the array);
    - check if the `children` array remains unchanged (if you pass an object that is not equivalent to any array element)
  - `deleteChild(int index)` - do 2 checks: 
    - check that the child is actually being removed from the `children` array and the method returns the correct value;
    - check that the `children` array remains unchanged (if you pass an index outside the index range) and the method returns the correct value;
  - `addChild` - check that the  `children` array increases by one element and that this element is the passed object with all the necessary references;
  - `countFamily` - check if the method returns the correct number of family members
- Cover the further project changes with tests.


#### Non-obligatory task with advanced complexity:
- `enum` `Species` must include a constructor in which you can specify the amount of parameters for a pet.
  - can the animal fly (`canFly`, boolean)
  - how many legs does the enimal have (`numberOfLegs`, number)
  - does the animal have fur (`hasFur`, boolean)
- Add the info above to the `toString()` method of the `Pet` class.
- Make tests for `equals()` и `hashcode()`:  `equals()` should return `true/false`, handle all cases according to the `equals` contract; 

#### Literature:
- [Finalize()](https://www.baeldung.com/java-finalize)
- [enum](https://www.w3schools.com/java/java_enums.asp)
- [Java Enum Tutorial with examples](https://beginnersbook.com/2014/09/java-enum-examples/)
- [Unit testing using JUnit](https://www.vogella.com/tutorials/JUnit/article.html)
- [Настройка JUnit с помощью IntelliJ IDEA](https://stackoverflow.com/questions/19330832/setting-up-junit-with-intellij-idea)
