Download Link: https://assignmentchef.com/product/solved-programming-assignment-3-a-date-class
<br>
Uses: Classes, Constructors, Methods, Enumerations

For your third assignment, you are to write a Java class that implements dates. A date is simply a month, a day, and a year. Externally (that is, to the user of the class) the month should represented as 0 for January, 1 for February, and so on. Internally, the class should use an enumeration for the months. The day is a one or two-digit integer. The year is a four-digit integer. (No Y2K bug for us!) The class should have the following:

A three-parameter constructor that takes three parameters, all ints: the month, the day, and the year,

and constructs a date with that information. Hint: Use a switch statement to convert the external representation of the month (an int) to the internal representation of the month (the enum). If youknow about arrays, you could use an array to do the conversion instead.

A two-parameter constructor that takes two ints and constructs a date using those ints as the month and the day. The year is taken to be the current year. Hint: To find the current year (which may change

as you use your program), you can use the line:  int year = Calendar. get Instance() . get(Ca1endar . YEAR);  which requires import java. util. Calendar;

A one-parameter constructor that takes one int and creates a date with that int as the day. The year and

the month are taken to be the current year and month. Hint: Use the Calendar object to find the month.

A zero-place constructor that creates a date corresponding to the current date. Hint: Use the Calendar

object to find the day.

Accessor methods, public int getMonth(), public int getDay(), and public int  get Year ( ) , that return the month, the day, and the year, respectively. Hint: use the ordinal () method on the enumeration literals to return the integer corresponding to the literal.

A method, public int compareT0(Date d), that returns a negative number if this (the object that compare To is called upon) is less that Date d, zero if they are equal, and a positive number if this  is greater than Date d. Hint: Compare the years first, then months (if the years are equal), and then the days (if the year and months are equal.)

A method, public String to string(), that returns a String with the date inhuman-readable form, e.g. “January 1, 2017”. Hint: You can use the month directly, or use a switch statement to convert the enum to a nice String

A main program that tests all of your methods. The testing should be thorough