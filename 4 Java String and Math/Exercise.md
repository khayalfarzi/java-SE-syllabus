# The task is

Write a program called "numbers", which makes a random number and offers the player to guess it.

#### Technical requirements:

- With the help of `java.util.Random` the program makes a random number in a range [0-100] and invites the player
  through a console to enter the name which is saved in the variable `name`.
- Before the beginning, show up given text on screen: `Let the game begin!`.
- The whole process of the game is processed in an infinite cycle.
- The player is invited to enter the number in the console, after which the program compares the hidden number with the
  fact that the user has entered.
- If the entered number is less than a random number which the program has generated, you should to display the
  text: `Your number is too small. Please, try again.`. If the entered number is more than the number which the program
  has generated, you should display the text: `Your number is too big. Please, try again.`.
- If the entered number is equal to the number which the program has generated, it is necessary to display the text on
  the screen: `Congratulations, {name}!`.