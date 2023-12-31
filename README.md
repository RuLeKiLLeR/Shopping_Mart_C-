# Shopping_Mart
This C++ code defines a simple command-line based supermarket management system. Here's a brief description of the code:

Class Definition (shopping):

It defines a class named shopping that encapsulates the functionality of the supermarket system.
Private data members include product code (pcode), price (price), discount (dis), and product name (pname).
Public member functions include:
menu(): Displays the main menu and handles choices for Administrator, Buyer, or Exit.
administrator(): Displays the administrator menu with options like adding, modifying, deleting products, or going back to the main menu.
buyer(): Displays the buyer menu with options like buying a product or going back to the main menu.
add(): Adds a new product to the system by taking input for product details and writing to a file (database.txt).
edit(): Modifies a product's details based on the product code by reading from and writing to a file.
rem(): Deletes a product based on the product code by reading from and writing to a file.
list(): Displays the list of products with their details.
receipt(): Generates a receipt for the buyer, calculates the total amount with discounts, and displays the details of purchased items.
Main Function:

It creates an instance of the shopping class (s) and calls its menu() function to start the supermarket management system.
File Handling:

The program uses file handling to store and retrieve product information in a file named database.txt.
It reads and writes product details from/to this file for tasks like adding, modifying, and deleting products.
Looping Structure:

The program uses labeled goto statements for looping (which is generally discouraged but used here for simplicity). The labels (m:) are placed at the beginning of the loops, and the program can jump to these labels based on user choices.
Security Check:

There is a basic login check for the Administrator, with a hardcoded email (robby@gmail.com) and password (robby@123).
Note: The code has some issues, such as incorrect file handling in the rem() function (remove("databaes.txt") should be remove("database.txt")). Also, the use of goto statements is generally discouraged due to potential readability and maintainability issues.
