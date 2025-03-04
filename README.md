ATM System Project
Overview:

The ATM System Project is a console-based C++ application designed to simulate basic banking functionalities, including client account management, login, balance inquiry, money withdrawal, and transfer operations. This project demonstrates structured programming techniques and includes proper error handling and validation for user inputs.

Features
Client Account Management

Create new client accounts with a unique username, PIN, and initial balance.
Prevent duplicate usernames.
Login System

Validate client credentials with username and PIN.
Allow a maximum of 3 login attempts before locking the account.
Account Operations

Balance Inquiry: View the current balance of the logged-in client.
Money Withdrawal:
Withdraw amounts in multiples of 50.
Limit withdrawals to $2000 per transaction.
Ensure sufficient balance before withdrawal.
Money Transfer:
Transfer funds to other registered clients.
Limit transfers to $10,000 per transaction and 3 transfers per day.
Error Handling

Input validation for PINs, balances, and usernames.
Proper messaging for invalid operations or inputs.
Code Structure
The project is organized around the following core functions:

New_Client()

Adds a new client to the system.
Ensures unique usernames and valid PINs.
login()

Validates client credentials.
Locks account after 3 failed attempts.
displayMenu()

Displays the main operations menu after successful login.
balanceCheck()

Displays the balance of the logged-in client.
withdraw()

Allows the client to withdraw money within the allowed limits.
Money_Transfer()

Facilitates fund transfer between accounts with proper validations.
main()

Entry point for the program.
Handles the high-level flow of the system, including activation, login, and navigation.
Limitations
Supports up to 10 clients due to fixed array sizes.
User data is stored in memory and does not persist after the program ends.
PINs are stored in plain text for simplicity.
