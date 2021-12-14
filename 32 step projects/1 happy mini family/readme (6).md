# The 'Happy Family' mini-project keeps striking!

The idea of the project is to describe the structure of a family while taking into account that every human has relatives and the family members can change over time.

# Working with date and time
## The task

Improve the project: Do a refactoring `Human` class in such a way that he can work with date and time.

#### Technical requirements:
- Replace `year` field with `birthDate` field that keeps the meaning Unix Millis Timestamp (`long` type).
- Add in `Human` class `describeAge()` method,which returns a line indicating the exact number of years, months and days of human life;
- Create a constructor for adopted children describing the name, surname, date of birth and IQ. The date of birth is transmitted as a string in the format `20/03/2016`
- Do a method refactoring `toString()` that it should indicate the date of birth in a format other than the year of birth `20/03/2016`

#### Literature:
- [Date and time](https://www.w3schools.com/java/java_date.asp)
