# Data-validation-Employee
# Index
## 1. [Introduction](#Introduction)
## 2. [Flow Chart](#Flow-Chart)
## 3. [Algorithms](#Algorithms)



>* [Main Function](#Main-Function)
>* [Asking Employee Details](#Reading-Employee-Details)
>* [Asking Salary Details](#Reading-Salary-Details)
>* [Validate Employee Details](#Validate-Personal-Details)
>>* [Validate Name](#Validate-Name)
>* [Validate Salary Details](#Validate-Salary-Details)
>* [Validate Date](#Validate-Date)


# __Introduction__
This document Explains you about the __Data Validation on Employee Details__ using structures. 
And the usage of Structures within structures and Dynamic Memory Allocation and  Pointers of structure variables. 

# Algorithms
### Main-Function
* Created structure for Employee details in this Structure we have Structure members for __First name__, __Last name__ and __Date of Birth__.
* Created another structure for Storing Salary details in Structure members for __Initial salary__, __Percentage Increment__ and __Date of Joining__.
* In this Main Function we Call the functions to __Create__ and __Print__ the empolyee details.
* In _Create_ function we create the structure varaibles to take salary and employee details from user.
* _Create_ function calls Two more function __Get Employee details__ and __Get Salary details__ to take these details from user.
* __Get Employee details__ function gets personal details from user. 
* __Get Salary details__ function  gets salary details from user.
### Get-Employee-Details
* In this function we take input from user for Employee details - _Frist name_, _Last name_ and _Date of Birth_.
* After finish taking inputs from the user, this function starts __Validate Employee details__ operation.
### Validate-Employee-Details
* In this section we use two more function to validate the Employee details.
* __Validate Name__ and __Validate Date__ funtions are two function used to validate Employee details of a person.
#### Validate-Name
* In this function the user given _first name_ and _last name_ are taken as inputs in this function.
* The name is taken in the form of string.
* Now the string is Cheked Character by Character to check the respective character is in the range of alphabets ASCII values.
* While checking if one character is out of Alphabetic ASCII range it return __-1__, produce error message to intimate the user and asks user to "Enter the Name correctely ".
* If the full string is in Alphabetic ASCII range then it exit from the function with return __0__
### Validate-Salary-Details
* In this section we use three more functions to Validate salary details.
*__Validate salary__, __Validate percentage__ and __Validate date__ are the functions to validate salary details.
* In __Validate salary__ we create another character array variable to take the salaray as string and check each character in the string, if the character is in AlphaNumeric ASCII range are not, if it is not in the specifed range then it returns __-1__ and produce error message and asks user to enter the salary again and again till the user gave the correct salary as INPUT.
* In __Validate Percentage__ we create here also another character array variable to store the percentage in the string form, after finishin up taking input from user, It checks the string size is two bytes or not and after that checks each character is in AlphaNumeric ASCII Range or not, If the it is not in Specifed Ranges then it returns __-1__ , produces error message and asks user to enter the percrntage correctly.
* After finishing the salary and percentage Validations it calls __Validate Date__ function.
### Validate-Date
* In this Section Checking User Entered __Valid-Date__ or __not__.
* In this function we checking date Entered from User as three strings in same line to read and check the every character in the date, month and year are in correct size. 
After checking date, month and year It checks individually the each and ever byte in date format are in the range of  ASCII range
And also checks the date, month and Year format of date  in between (1 to 31), month (1 to 12) and year>999
If all the conditions are satisified then it return -1 and produces error message and asks user to enter the date correctly again and again till the user will enter the correct date, month and Year


