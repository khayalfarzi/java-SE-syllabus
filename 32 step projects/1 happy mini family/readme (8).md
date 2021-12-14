# The 'Happy Family' mini-project keeps striking!

The idea of the project is to describe the structure of a family while taking into account that every human has relatives and the family members can change over time.

# Creating a console application
## The task

Improve the project: 
 - Create a console application, which in an infinite loop ( untill entering the command `exit`) allows you to display and edit family information.
 - add the exception processing.

#### Technical requirements:
- In `Family` class create `prettyFormat()` method which returns a string, describing the family in a legible format (the format can be invented or taken from the example). **Each field should start with a new line**:  
```    
family: 
	mother: {name='Kate', surname='Bibo', birthDate='03/03/1991', iq=95, schedule={FRIDAY=fitness, MONDAY=fitness}},
	father: {name='Karl', surname='Bibo', birthDate='10/12/1990', iq=90, schedule={FRIDAY=library, MONDAY=library}},
	children: 
		boy: {name='Donna', surname='Bibo', birthDate='23/10/2018', iq=92, schedule=null}
		girl: {name='Sun', surname='Bibo', birthDate='23/10/2018', iq=92, schedule=null}
		boy: {name='Kurt', surname='Kobein', birthDate='05/05/2003', iq=85, schedule={FRIDAY=music}}
	pets: [{species=DOG, nickname='Jack', age=3, trickLevel=35, habits=[sleep]}, {species=CAT, nickname='Oscar', age=5, trickLevel=81, habits=[eat, play]}]
```
(To get such a format it is necessary to implement `prettyFormat` method in all three classes: `Family`, `Human`, `Pet`)
- Do a `FamilyService` refactoring in that way when a single family or list is displayed on the screen, the information is displayed in a convenient format, using `prettyFormat()` method.
- Display a list of available commands each time the user is expected to enter data.
- The application has the following hierarchical command structure:
```
- 1. Fill with test data (create several families and save them in the database)
- 2. Display the entire list of families (displays a list of all families with indexation starting with 1)
- 3. Display a list of families where the number of people is greater than the specified number
  - request a number one you interested in
- 4. Display a list of families where the number of people is less than the specified number
  - request a number one you interested in
- 5. Calculate the number of families where the number of members is
  - request a number one you interested in
- 6. Create a new family
  - request for the mother's name
  - request mother's last name
  - request mother's birth year
  - request mother's month of birth
  - request mother's birthday
  - request mother's iq
  
  - request for the father's name
  - request father's last name
  - request father's birth year
  - request father's month of birth
  - request father's birthday
  - request father's iq
- 7. Delete a family by its index in the general list
  - request identifier (ID)
- 8. Edit a family by its index in the general list
  - 1. Give birth to a baby
    - request family identifier (ID)
    - request the necessary data (what name to give the boy, what name to girl)
  - 2. Adopt a child
    - request family identifier (ID)
    - request Required data (full name, year of birth, intelligence)
  - 3. Return to main menu  
- 9. Remove all children over the age of majority (all families remove children over the age of majority - let us assume they have grown up)
  - request interested age
```
- The user selects the menu item of interest by its serial number.
- Handle all possible exceptions related to incorrect data entry by the user.
- Create your own exception `FamilyOverflowException`, inherited from `RuntimeException`. Drop it if the family size is larger than [any desired number] of people and the family is trying to give birth to/adopt a child. Process it in the controller.

#### Literature:
- [Exception handling](https://www.journaldev.com/1696/exception-handling-in-java)
- [Creating a custom exception](https://www.baeldung.com/java-new-custom-exception)
