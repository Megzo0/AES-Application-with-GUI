🛡️ AES-128 Encryption/Decryption – Java Implementation + GUI

Simple educational AES-128 encryption/decryption tool written fully in pure Java (no external libraries).
The project includes:

✔ Full AES-128 implementation (SubBytes, ShiftRows, MixColumns, KeyExpansion, AddRoundKey)

✔ Encryption + Decryption working on 16-byte blocks

✔ PKCS#7 / Custom padding (#)

✔ Full round-by-round tracing (Verbose Mode)

✔ Swing GUI to test plaintexts, keys, padding, and view HEX + raw ciphertext output

✔ Designed for Security Labs / Cryptography Assignments

This project is meant for learning, analysis, and demonstrating AES internal transformations.

📌 Features
🔐 AES-128 Core

Manual implementation of:

S-Box

Inverse S-Box

ShiftRows / Inverse ShiftRows

MixColumns / Inverse MixColumns

KeyExpansion (11 round keys)

AddRoundKey

🖥️ GUI (Swing)

Input plaintext

Input 32-hex character key (128-bit)

Select padding:

PKCS#7

Pad with #

Encrypt & Decrypt buttons

Optional Verbose Mode (shows full round states)

Output:

Cipher (HEX)

Cipher (raw chars)

Decrypted text

🛠️ How to Compile & Run
Using Terminal / CMD
javac AES_GUI.java
java AES_GUI


Make sure you have Java 8+ installed.

🧪 Usage
🔹 Encrypting

Enter plaintext

Enter 32-hex key (example: 00112233445566778899AABBCCDDEEFF)

Select padding

(Optional) Check Verbose to show all rounds

Click Encrypt

Output will show:

Cipher HEX

Cipher raw characters

Logs for debugging / learning

🔹 Decrypting

Paste cipher-hex into the plaintext field

Enter the same 32-hex key

Select the same padding used for encryption

Click Decrypt

The decrypted plaintext will appear at the bottom.

📂 Project Structure
.
├── AES_GUI.java     # Main file (GUI + AES implementation)
├── README.md        # This file

🧩 Padding Modes
▶ PKCS#7

Standard padding:

If plaintext is 4 bytes → adds 12 bytes of value 0x0C.

▶ Pad with '#'

Simple demo padding (used in many labs):

Appends # until reaching 16 bytes.

👀 Verbose Mode

Shows AES internal transformations:

After SubBytes

After ShiftRows

After MixColumns

After every round

Final ciphertext block

Great for labs, debugging, and understanding AES internals.

⚠️ Disclaimer

This project is for educational & lab use only.
Do NOT use this implementation in production systems.
Not hardened against timing attacks, padding oracles, or side-channel leaks.

⭐ Author

Developed by Ahmed Hussein Saad
4th-year Computer Science student – interested in Security, SOC analysis, and Crypto Engineering.

🤝 Contributions

PRs and suggestions are welcome.

🔥 If you like this repo

Leave a ⭐ on GitHub — helps a lot!
