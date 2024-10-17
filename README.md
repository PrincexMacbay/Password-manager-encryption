# Password-manager-encryption
Password Manager with Encryption: This project is a simple yet effective password manager designed to securely store and retrieve user passwords through encryption. Using the cryptography library's Fernet symmetric encryption, this application ensures that sensitive information remains confidential and protected from unauthorized access.

Features
Secure Password Storage: The application encrypts passwords before saving them to a text file, rendering them unreadable to anyone who does not possess the encryption key and master password.

Easy Retrieval: Users can easily access stored passwords by providing the correct master password, which decrypts the passwords for viewing.

User-Friendly Interface: The program features a straightforward command-line interface, making it easy for users to add new passwords or view existing ones without technical expertise.

How It Works
Key Generation: A unique encryption key is generated using the Fernet algorithm and saved to a file named key.key. This key is essential for both encryption and decryption of passwords.

Password Encryption: When a user adds a password, it is encrypted using the generated key and the user's master password. The encrypted password is then stored in a text file (passwords.txt) along with the associated account name.

Password Decryption: When users wish to view their passwords, the program retrieves the encrypted passwords from the text file and decrypts them using the master password.

Installation
To get started, clone the repository and install the required library:

bash
Copy code
git clone https://github.com/PrincexMacbay/Password-manager-encryption.git
cd password-manager
pip install cryptography
Before running the program, generate the encryption key by uncommenting the write_key() function in the code.

Usage
Run the program and enter your master password when prompted. Choose to either add a new password or view existing ones. Note that the application stores passwords in an encrypted format, ensuring their security.

Contributing
Contributions are welcome! Feel free to fork the repository and submit pull requests to improve the functionality or fix any bugs.

License
This project is licensed under the MIT License.
