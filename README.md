🔐 PyCryptX — Secure Text & File Encryption Toolkit

PyCryptX is a Python-based cryptography project designed to demonstrate how modern encryption can be used to protect text and files.

The project uses AES-256-GCM for authenticated encryption and PBKDF2-HMAC-SHA256 to securely derive an encryption key from a user-provided password.

✨ Features

- 🔒 Encrypt and decrypt text
- 📁 Encrypt and decrypt files
- 🔑 Password-based key derivation
- 🛡️ AES-256-GCM authenticated encryption
- 🧂 Random salt generation
- 🔢 Random nonce generation
- ✅ Data integrity and authentication verification
- 🔐 Hidden password input
- ⚠️ Error handling and validation
- 💻 Simple command-line interface

🛠️ Technologies Used

- Python 3
- Cryptography
- AES-256-GCM
- PBKDF2-HMAC-SHA256
- SHA-256
- Base64
- File handling

🚀 Installation

Clone the repository:

git clone https://github.com/YourUsername/PyCryptX.git
cd PyCryptX

Install the required package:

pip install -r requirements.txt

▶️ Usage

Run the program:

python pycryptx.py

The application provides options for:

1. Encrypt text
2. Decrypt text
3. Encrypt file
4. Decrypt file
5. About / security details
6. Exit

🔒 Example

Encrypt Text

Enter text: Hello from PyCryptX!
Password: ********

The program generates an encrypted text payload.

Encrypt a File

Input file path: sample_files/notes.txt
Password: ********

The encrypted file will be created as:

notes.txt.pcrypt

The original file remains unchanged.

🧠 How It Works

PyCryptX first generates a random salt and uses PBKDF2-HMAC-SHA256 to derive a 256-bit key from the user's password.

The data is then encrypted using AES-256-GCM.

The encrypted data contains the required salt and nonce along with the ciphertext and authentication information.

Conceptually:

Password
    ↓
PBKDF2-HMAC-SHA256
    ↓
256-bit Encryption Key
    ↓
AES-256-GCM
    ↓
Encrypted Data

🛡️ Security

AES-GCM provides both:

- Confidentiality — protects the contents of the data.
- Integrity/authentication — detects unauthorized modification.

PyCryptX does not store the user's password.

If the password is incorrect or encrypted data has been modified, decryption fails.

«Never upload passwords, API keys, private keys, or real sensitive data to GitHub.»

📚 What I Learned

Through this project, I learned about:

- Symmetric-key cryptography
- AES encryption
- Authenticated encryption
- Password-based key derivation
- PBKDF2
- SHA-256
- Salt and nonce
- Binary data processing
- File encryption
- Secure password handling
- Python exception handling
- Command-line application development

🔮 Future Improvements

- Graphical User Interface using Tkinter
- Password strength checker
- Secure password generator
- Multiple-file encryption
- Encrypted ZIP archives
- Key-file support
- Unit testing
- Automated security testing

⚠️ Disclaimer

PyCryptX is an educational and portfolio project created to demonstrate Python programming and fundamental cryptography concepts.

It should not be considered a replacement for professionally audited security software or enterprise key-management systems.

👨‍💻 Author

Subhadip

Python Developer | Cryptography | Cybersecurity Fundamentals
