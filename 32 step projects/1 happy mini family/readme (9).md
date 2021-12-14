# The 'Happy Family' mini-project keeps striking!

The idea of the project is to describe the structure of a family while taking into account that every human has relatives and the family members can change over time.

# Working with I/O streams. Reading and writing to files
## The task

Improve the project: add the ability to work with the file system.

#### Technical requirements:
- Add to the application the ability to save data locally to your computer.
- Add the ability to load previously saved data (new item in the main menu instead of generating test data).
- To download data in the `FamilyService` and `FamilyDao` classes, add `loadData` method which accepts the `List<Family> families` and downloads it to our database.
-For each action, add an item to the main menu.

The list of families with all data should be saved/downloaded.

#### Not a necessary task of advanced complexity:
- Create a separate service (class) for logging, which will have 2 methods: `info()` (log information message) and `error()` (log error). Both methods accept the message for logging, but give a different format: 01/01/2019 15:35 [DEBUG]/[ERROR] `message`. 
- Add a call to the `logger.info()` method in all methods `CollectionFamilyDao`  with an info message such as `receiving a family list`, `adding a new family`, `deleting a family`, etc. 
- При обработке исключений логируйте их с помощью метода `logger.error()`.
- When processing exceptions, log them using the `application.log`.
- Make sure that the recording is always done at the end of the file from a new line.  

#### Literature:
- [File handling in Java using FileWriter and FileReader](https://www.geeksforgeeks.org/file-handling-java-using-filewriter-filereader/)
- [Reading strings from a file](https://www.geeksforgeeks.org/different-ways-reading-text-file-java/)
- [Add text to end of file](https://stackoverflow.com/questions/1625234/how-to-append-text-to-an-existing-file-in-java)

