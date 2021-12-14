# "A happy family" Mini-Project 

Assignment: describe the structure of a family, take into account that each member has blood relatives and the composition of the family tends to fluctuate.
Before you get to the "Collections" topic - all the homeworks must be done using arrays (**DO NOT** use  `List`, `Set`, `Map` interfaces, unless the assignment says you to.

# Objects
## Task

Create and describe these classes:  (`Pet`), (`Human`). Create constructors for the classes you have written. Create the `Main` class and the examples of the described classes in it. 

#### Technical requirements: 
- Describe the Pet with the following fields:
  - (`species`)
  - (`nickname`)
  - (`age`)
  - (`trickLevel`) (a whole number from 1 to 100)
  - (`habits`) (array of strings)
- Describe and implement the following methods for Pet:
  - (`eat`) (method displays a message 'I am eating')
  - (`respond`) (method displays a message 'Hello, owner. I am - [the name of the pet]. I miss you!')
  - (`foul`) (method displays a message 'I need to cover it up')
- Describe Human with the following fields:
  - (`name`)
  - (`surname`)
  - date of birth (`year`), number
  - IQ level (`iq`) (a whole number from 1 to 100))
  - (`pet`) (object type Pet)
  - (`mother`) (object type Human)
  - (`father`) (object type Human)
  - Schedule of non-working activities (`schedule`) (2d array: [day of the week] x [type of the activity])
- Describe and implement the following methods for Human:
  - (`greetPet`)("Hello, [the name of the pet]")
  - (`describePet`): (display the information about your pet: "I have a [species], he is [age] years old, he is [very sly]>50/[almost not sly]<50". 
- Redefine the  `toString()` method for bot classes;
  - The Pet class must display the following message: `dog{nickname='Rock', age=5, trickLevel=75, habits=[eat, drink, sleep]}`, where `dog` = species;
  - The Human class must display the following message: `Human{name='Michael', surname='Karleone', year=1977, iq=90, mother=Jane Karleone, father=Vito Karleone, pet=dog{nickname='Rock', age=5, trickLevel=75, habits=[eat, drink, sleep]}}`
- In class `Pet` create constructors:
  - constructor which describes the pet's species an nickname 
  - constructor which describes all the fields for the pet
  - empty constructor 
- In class`Human` create constructors:
  - constructor which describes the name, surname and the date of birth
  - constructor which describes the name, surname, date of birth, father and mother
  - constructor which describes all the fields 
  - empty constructor 
- In the Main class create several families, so that every class uses all the available constructors. Display data about every person.
- In the Main class: create a mother, father, child and his pet. Specify all the needed links (for child to his parents and to the pet), in order to form a full family. Call all available methods for the child (including  `toString()` method) and his pet.


#### Non-obligatory task with advanced complexity:
Describe and implement the  (`feedPet`) method in the Human class, which accepts a logical boolean type as a parameter ("isn't it time for feeding "). If it is time - the owner feeds the pet, if not - the trick level is compared to a pseudorandom number of 0-100 using `java.util.Random` and the owner feeds the pet if the trick level is greater than the generated number. The method should display the following result: (`Hm... I will feed Jack's [animal name]/`/`I think Jack is not hungry.`) and return a boolean value (`true/false`) - whether the feeding happened or not.

#### Литература:
- [Classes and objects](https://www.geeksforgeeks.org/classes-objects-java/)
- [Constructors](https://www.w3schools.com/java/java_constructors.asp)
- [Initializers](https://www.dummies.com/programming/java/what-is-an-initializer-in-java/)
