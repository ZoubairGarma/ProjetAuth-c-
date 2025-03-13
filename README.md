# ProjetAuth-c- 
Key Features
Hashing & Salting

Uses OpenSSL's SHA-256 for password hashing.
Generates a random 16-character salt to strengthen security.
User Class

Stores username, hashed_password, and salt.
Converts user data to/from a string format for file storage.
UserRepository Class

Manages user records in a CSV file (users.csv).
Saves users and retrieves them based on the username.
AuthService Class

Validates usernames (no commas) and passwords (must be strong: min 8 chars, upper/lowercase, digit, special character).
Prevents duplicate usernames.
Handles registration (hashing & storing credentials).
Handles login (verifies hashed password against stored hash).
Main Program

Provides a simple menu-based interface (Register, Login, Exit).
Prompts the user for credentials and interacts with AuthService.

PS:this code  has been tested , it is fully functional . If there are any issues, check if openSSL is installed and recompile the project 
PS:OpenSSL must be installed. 
