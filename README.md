🔐 Advanced AES-256 File Encryption Tool 🗂️
📖 Overview

This is a user-friendly GUI application built with Python and Tkinter that allows you to encrypt and decrypt files using AES-256 encryption in GCM mode. It uses secure password-based key derivation (PBKDF2 with SHA256) and random salts and nonces for strong cryptographic protection.
⚙️ Features

    🔑 Password-based encryption & decryption (AES-256 GCM)

    🧂 Uses PBKDF2HMAC with SHA256 for key derivation and a unique salt per file

    🔒 Authenticated encryption mode (GCM) providing confidentiality and integrity

    🖼️ Simple and intuitive Tkinter GUI for easy file selection and password entry

    📂 Supports encrypting any file type

    💾 Save encrypted files with .enc extension and decrypted files with .dec

🛠️ How It Works

    You enter a password to generate a cryptographic key using PBKDF2 with a random salt.

    The selected file is encrypted using AES-256 in GCM mode with a random nonce.

    The encrypted output file stores salt + nonce + authentication tag + ciphertext.

    For decryption, the key is derived from the password and salt, then the ciphertext is decrypted and verified with the tag.

💻 Usage

    Run the program:

    python encryption_tool.py

    Enter a strong password in the Password field.

    Click Browse to select the file you want to encrypt or decrypt.

    Click Encrypt to encrypt the file and save the .enc output.

    Click Decrypt to decrypt a previously encrypted .enc file and save the original content.

📦 Requirements

    Python 3.x

    cryptography package

    tkinter (usually included with Python)

Install the required package with:

pip install cryptography

⚠️ Important Notes

    🔐 Choose a strong, memorable password to ensure file security.

    ❗ Losing the password means the file cannot be decrypted.

    🛑 Use this tool responsibly and only encrypt files you own or have permission to secure.

    🧩 Encrypted files contain all necessary metadata (salt, nonce, tag) for decryption.

👩‍💻 Author

Mansi Gharat
