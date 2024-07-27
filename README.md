# Customized-Database-Management-System_Marvellous
Java programming

## Customized Database Management System (DBMS) Documentation

### Overview

The Customized Virtual Database Management System (CDBMS) is a simple, console-based application implemented in Java for managing employee records. It allows users to perform various operations such as inserting new records, displaying records, deleting records, and performing aggregate operations on employee salaries. The system uses a linked list data structure to store employee data in memory.

### Classes

#### `Employee`
This class represents an employee in the database.

**Attributes:**
- `int EID`: Employee ID (auto-incremented)
- `String Ename`: Employee name
- `String EAddress`: Employee address
- `int ESalary`: Employee salary
- `static int Counter`: Static counter to generate unique Employee IDs

**Methods:**
- `Employee(String B, String C, int D)`: Constructor to initialize an employee object
- `void DisplayInfo()`: Method to display employee information

#### `CDBMS`
This class provides methods to manage the employee database.

**Attributes:**
- `LinkedList<Employee> lobj`: Linked list to store employee objects

**Methods:**
- `CDBMS()`: Constructor to initialize the DBMS
- `protected void finalize()`: Destructor to deallocate resources
- `void InsertIntoTable(String name, String Address, int Salary)`: Method to insert a new employee record
- `void SelectStar()`: Method to display all employee records
- `void SelectSpecific(int ID)`: Method to display records with a specific Employee ID
- `void SelectSpecific(String Name)`: Method to display records with a specific Employee name
- `void DeleteFrom(int ID)`: Method to delete records with a specific Employee ID
- `void DeleteFrom(String Name)`: Method to delete records with a specific Employee name
- `void AggregateSum()`: Method to display the sum of all employee salaries
- `void AggregateMax()`: Method to display the maximum salary among employees
- `void AggregateMin()`: Method to display the minimum salary among employees
- `void AggregateAvg()`: Method to display the average salary of employees
- `void AggregateCount()`: Method to display the count of employee records

### Main Program (`program665`)
The main program provides a console-based menu for interacting with the DBMS.

**Attributes:**
- `Scanner sobj`: Scanner object for reading user input
- `CDBMS mobj`: Instance of the CDBMS class
- Various variables for storing user input (e.g., `int iOption`, `int Salary`, `int EID`, `String Name`, `String Address`)

**Menu Options:**
1. Insert new record into the table
2. Display all records
3. Display all records having a specific EID
4. Display all records having a specific Name
5. Delete the record based on EID
6. Delete the record based on Employee name
7. Display the sum of all salaries
8. Display the average of all salaries
9. Display the minimum salary
10. Display the maximum salary
11. Display the count of records
12. Display Help
13. Display About
14. Terminate the DBMS

### Usage

1. **Insert a New Record**: Enter the employee's name, address, and salary. The system automatically generates a unique Employee ID.
2. **Display All Records**: Lists all employee records.
3. **Display Records by EID**: Enter the specific Employee ID to view the record.
4. **Display Records by Name**: Enter the employee's name to view the record(s).
5. **Delete Record by EID**: Enter the specific Employee ID to delete the record.
6. **Delete Record by Name**: Enter the employee's name to delete the record(s).
7. **Display Sum of Salaries**: Displays the total sum of all employee salaries.
8. **Display Average Salary**: Calculates and displays the average salary of employees.
9. **Display Minimum Salary**: Shows the minimum salary among employees.
10. **Display Maximum Salary**: Shows the maximum salary among employees.
11. **Display Count of Records**: Displays the number of employee records.
12. **Display Help**: Provides information about the DBMS project.
13. **Display About**: Shows information about the project developer.
14. **Terminate the DBMS**: Ends the program and deallocates resources.

### Notes
- This DBMS is implemented entirely in primary storage (memory), so all data will be lost upon program termination.

### Example Usage
Run the main program, follow the menu options, and input the required data as prompted to manage employee records effectively.
