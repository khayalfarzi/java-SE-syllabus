# The 'Happy Family' mini-project keeps striking!

The idea of the project is to describe the structure of a family while taking into account that every human has relatives and the family members can change over time.

# OOP in Java, OOP guidelines
## The task

Improve the project using OOP

#### Techincal requirements:
- Make  `Pet` an abstract class .
- Implement inheritance from the `Pet` class:
  - create the `Fish`, `DomesticCat`, `Dog`, `RoboCat` (a cat robot) classes
  - not all animals can do the same thing. Everybody eats the same way, everyone describes themselves differently, but not everybody does all the nasty things (a fish, for example, does not know about them at all). Therefore, leave the implementation of the `eat`  method in the abstract class, make the `respond` method abstract and implement `foul` into the interfaces of those hereditary classes, which can do that.
- Add the corresponding enumerations in `Species`, also add the  `UNKNOWN` enumeration (for the animals, which kind is not known); make it so that at the initialisation of variables the corresponding kind was assigned to it automatically and in case of an unknown type - the type would be set to `UNKNOWN`.
- Now the `Species` field is set at the object's initialization. Remove it from the `Pet` constructor.
- Make sure all subclasses have superclass designers.
- Implement inheritance from the `Human` class:
  - create class inheritors of the `Human` class: `Man`, `Woman`; prohibit the inheritance of these classes.
  - redefine the `Human`  `greetPet` method for each subclass (the text can be selected at your discretion).
  - Describe each subclass's unique method of choice (e.g. `makeup` for women and `repairCar` for men).

#### Non-obligatory task with advanced complexity:
- Create the `HumanCreator` interface and specify a `bornChild()` method, which creates a new instance of the `Human` class (child).
- Implement the `HumanCreator` interface in one of the existing project classes. The implementation should return a new object `Man` or `Woman` with references to the current family, father's name, random name (you need to create a list of names in advance), and average IQ (from father and mother). The sex of the child is defined casually with the 50%/50% probability.

#### Literature:
- [Inheritance, polymorphism, encapsulation](https://www.quora.com/What-is-the-difference-between-inheritance-encapsulation-and-polymorphism)
- [Abstract classes](https://idratherbewriting.com/java-abstract-methods/)
- [Java 8 interfaces](https://beginnersbook.com/2017/10/java-8-interface-changes-default-method-and-static-method/)
