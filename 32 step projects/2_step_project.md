# Step Project Booking
## The task

#### Create a Java console app for booking plane tickets

#### The description

Create a console app that provides an interface for searching and booking plane tickets in an infinite loop (before the user chooses the `exit` command).

#### Teamwork

In this project, all students are divided into groups of three.There is a list of tasks to be done for each team member. The rest of the tasks can be assigned by the team members themselves. Team members can decide for themselves who will perform the  #1, #2 and #3 tasks.

#### The app's main menu

The main menu which the user sees upon opening the app should have the following features:
1. **Online-board**. Shows information about all flights from Kiev in the next 24 hours. The main menu will be displayed again afterwards.

2. **Show the flight info**. The user is prompted to enter the flight id. Then the following window depicts all the information about this particular flight: the date, time, destination point and the amount of free seats. The main menu will be displayed again afterwards.

3. **Search and book a flight**. The user is prompted to enter the following information: destination, date, number of people (how many tickets to buy). After that, the program must search for flights that meet the specified conditions (there must be enough seats for all passengers). All found flights should be displayed on the screen. After that, the user can choose one of the found flights by specifying its serial number or return to the main menu (selecting item 0). If the user decides to book a flight, he will need to enter the names and surnames of all passengers.

4. **Cancel the booking**. The user is prompted to enter the booking id. If such a booking has been found, it will be cancelled. The main menu is then displayed again. The user can cancel any booking.

5. **My flights**. The user is prompted to enter his full name. A list of all bookings made by the user or in which the user is a passenger is then displayed.

6. **Exit**. Shuts down the application

#### Technical requirements:
- The application must have a standard three-layer structure - for each entity it must have Controller, Service and DAO classes.
- Unit tests must be written for each controller, service and DAO classses.
- To work with the console (main menu), a separate class must be created, which will access the necessary controllers to get information. Controllers can access services, services from DAO. There should be no direct access to services or DAO from the console class.
- The rest of the entities/classes should also be broken down into corresponding packages.
- You should use the features of Java 8 wherever possible.
- In case of impossible actions of the user (for example, if he selects of a non-existent menu item), throw your own exception class. Intercept it in the application above to make the program continue its work.
- The "database" of the application should be stored in a text/binary file next to the application. When launching the application, the data from the files should be written to the the collections in the DAO classes.
- The application should have a large automatically generated flight database, which should be copied to a file and read by the application at startup.
- It is enough to make all the flights from Kiev, they will differ only in the destination.
- When exiting the application, all the changes must be written to the save file. When restarting the application, the collections in DAO must be re-initialized with data from the save file.

#### The task for student №1
- Create a class to work with the console

#### The task for student №2
- Create a controller, a service and DAO for the flights

#### The task for student №3
- Create a controller, a service and DAO for the bookings

#### Organization of the workflow:
- The code of the team members must be in the same repository.
- You will need to set up GitLab so that the `master` branch would be protected and nobody could commit to it. You can read about how to do such thing [here](https://help.github.com/en/enterprise/2.16/admin/developer-workflow/configuring-protected-branches-and-required-status-checks).
- You need to create a new branch each time you make changes in the project and then Pull Request, based on its changes. You can find more details about the process [here](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).
- You will learn to commit Code review of the code which was written by your colleagues. The project must be set up in such a manner, so that every Pull Request is able to be merged into master after it gets Approve from other team members. You can find the description of setting up the repository [here](https://yangsu.github.io/pull-request-tutorial/ ).

#### Non-obligatory task, advanced level:
- Create a separate class for logging, write down all the actions of the use in a log file.
- Before showing the main menu authorize the user - he must enter his login and password. If such a user exists the main menu is displayed and вся работа происходит от имени этого пользователя. For example section **My bookings** displays information about all the bookings of the current user. A new section is added to main menu **End session**, it makes a logout, so that login and password of an other user can be entered.
- Add flight not only from Kiev but also between other cities. Finding connecting flights with connections not longer than 12 hours.
#### Good luck!
