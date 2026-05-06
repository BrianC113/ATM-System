ATM BANKING SIMULATOR
=====================

Author: Brian Munashe Chinhamora  
Language: Java  
Framework: JavaFX  
Architecture: Model–View–Controller (MVC)

--------------------------------------------------

PROJECT OVERVIEW
----------------
This project is a Java-based ATM Banking Simulator developed using the 
Model–View–Controller (MVC) architectural pattern and a JavaFX graphical user interface.

The system simulates basic ATM functionality, allowing users to create accounts, 
log in securely, and perform banking operations such as deposits, withdrawals, 
balance checks, and transfers.

The application separates responsibilities into three main components:
- Model (Bank & BankAccount classes)
- View (JavaFX GUI)
- Controller (handles user input and interaction with the UIModel)

--------------------------------------------------

FEATURES
--------
- Account creation with validation
- Secure login system with limited attempts
- Deposit and withdrawal functionality
- Balance checking
- Money transfer between accounts
- Password change functionality
- Support for decimal (currency) transactions
- Input validation and error handling
- Multiple account types (e.g. Savings, Student, Prime)

--------------------------------------------------

ACCOUNT TYPES
-------------
- Standard Account: Basic banking functionality
- Savings Account: Designed for saving money (can include interest)
- Student Account: Withdrawal limit per transaction
- Prime Account: Allows overdraft (negative balance within limits)

--------------------------------------------------

SYSTEM DESIGN (MVC)
-------------------
Model:
Handles all business logic including account management, transactions, and validation.

View:
Implements the JavaFX graphical interface, displaying input/output to the user.

Controller:
Receives user actions (button clicks) and sends commands to the UIModel.

UIModel:
Acts as the central logic controller between the View and the Bank system, 
managing application state and user interactions.

--------------------------------------------------

HOW TO RUN
----------
1. Ensure Java (JDK 8 or later) is installed.
2. Ensure JavaFX is properly configured in your environment.
3. Compile all Java files.
4. Run the Main class to launch the application.

--------------------------------------------------

USAGE
-----
1. Enter an account number and press "Ent" to log in.
2. Enter password and press "Ent".
3. Choose a transaction:
   - Dep: Deposit
   - W/D: Withdraw
   - Bal: Check balance
   - Trf: Transfer money
   - Pwd: Change password
   - New: Create new account
   - Fin: Logout

--------------------------------------------------

TESTING
-------
The system has been tested for:
- Successful transactions
- Invalid inputs (e.g. zero/negative amounts)
- Transfers to invalid or same accounts
- Insufficient balance handling
- Login failures and retry limits

--------------------------------------------------

KNOWN LIMITATIONS
-----------------
- Data is not persisted (accounts reset on restart)
- Fixed maximum number of accounts
- No advanced security (e.g. encryption)
- Limited UI styling

--------------------------------------------------

FUTURE IMPROVEMENTS
-------------------
- Database integration for persistent storage
- Enhanced security (encryption, hashing passwords)
- Improved UI/UX design
- Transaction history tracking
- Interest calculation for savings accounts

--------------------------------------------------

END OF FILE
