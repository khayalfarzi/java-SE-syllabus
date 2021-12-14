# The 'Happy Family' mini-project keeps striking!

The idea of the project is to describe the structure of a family while taking into account that every human has relatives and the family members can change over time.

# Layer DAO
## The task

Improve the project: 
 - create the DAO layer
 - create `FamilyController` classes and `FamilyService` for wokr with objects like `Family`.

#### Techincal requirements:
- Create interface to access class data  `Family` - `FamilyDao` with next methods:
  - `getAllFamilies` - returns an indexed list of all families    (`List`).
  - `getFamilyByIndex` (accepts the family index from general list) - returns the family by the specified index. In case you have requested an element with a non-existent index, return     `null`.
  - `deleteFamily` (accepts the index) - deletes family with a specified index, if such an index exists; returns `true` if the removal took place, `false` - if not.
  - `deleteFamily` (takes on the `Family` type) - deletes a family if one exists on the list; returns `true` if the removal took place, `false` - if not.
  - `saveFamily` (accepts the `Family` type) - updates an existing family in Database if if that one already exists, saves at the end of the list - if not.
- Create `CollectionFamilyDao` class: class have to include `List<Family>`, where all the families will be kept (it's gonna be our database) and implement the `FamilyDao` interface.
- Create `FamilyService` class, which should contain the `FamilyDao` field to access stored data.
- `FamilyService` class must implement the methods (if in `FamilyDao` there are not enough methods for the implementation - add them and implement them in `CollectionFamilyDao`):
  - `getAllFamilies` - to get a list of all the families. 
  - `displayAllFamilies` - to put all the families on the screen (in the indexed list) with all the family members.
  - `getFamiliesBiggerThan` - to find family with number of people **more** than (takes the number of people and returns all families where the number of people is greater than specified); displays the information on the screen.
  - `getFamiliesLessThan` - to find family with number of people **less** than (takes the number of people and returns all families where the number of people is less than specified); выводит информацию на экран.
  - `countFamiliesWithMemberNumber` - to calculate the number of families with the number of people equal to the number of transfered people.
  - `createNewFamily` - create a new family ( takes two parameters of Human type) - create a new family, saves in database.
  - `deleteFamilyByIndex` - to delete a family by its index in the list - deletes the family fron database.
  - `bornChild` - to give a birth to a child's family (takes `Family` and two `String` types: masculine and feminine) - a new child is born in the given family taking into account the parents' data, the information about the family is updated in the database; the method returns the renewed family. If the child is born a boy, it is given a male name, if the girl is female.
  - `adoptChild` - to adopt child (takes two types: `Family`, `Human`)- the child is kept in the given family, the information about the family is updated in the database; the method returns the renewed family.
  - `deleteAllChildrenOlderThen` - to delete all children older than (takes int) - in all families, children over the specified age are removed and the information is updated in the database.
  - `count` - returns the number of families in the database.
  - `getFamilyById` - takes the family  index, returns `Family` as specified index.
  - `getPets` - takes the family index, returns the list of pets that live in the family.
  - `addPet` - takes family index and `Pet` parameter - adds a new pet to the family, updates the data in the database.
- Create `FamilyController` class, which should contain `FamilyService` field to access the application' business logic methods.
- `FamilyController` class must contain the same methods as those in the `FamilyService`.
- In the Main class call up all the methods from `FamilyController`, to demonstrate their perfomance.
- Cover all methods from `FamilyService` unit tests.

#### Literature:
- [Data acess object (DAO) in Java](https://www.baeldung.com/java-dao-pattern)
- [Service Layer](https://softwareengineering.stackexchange.com/questions/220909/service-layer-vs-dao-why-both)
- [DAO levels and Service](https://dzone.com/articles/unit-testing-dao-service-and-controller-in-spring)
- [Service layer pattern](https://en.wikipedia.org/wiki/Service_layer_pattern)
