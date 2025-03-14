# Block & Stream Cipher

This project implements two types of encryption algorithms: **Block Cipher** and **Stream Cipher**. It allows users to encrypt or decrypt files using a provided key.

## Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Example Commands](#example-commands)
- [Contributing](#contributing)
- [Contact](#contact)

## About the Project
This project provides an encryption/decryption system using:
- **Block Cipher**: Encrypts data in fixed-size blocks with padding.
- **Stream Cipher**: Encrypts data byte-by-byte using XOR operations.

Users can specify which cipher type to use and whether they want to **encrypt (E)** or **decrypt (D)** files.

## Features
Supports **Block Cipher** (fixed-size encryption)
Supports **Stream Cipher** (continuous encryption)
Implements **padding and XOR operations**
Performs **file-based encryption and decryption**
Validates input files and key files

## Technologies Used
- **Java** - Core implementation
- **Makefile** - Simplifies compilation and execution
- **File I/O** - Reads and writes encrypted/decrypted files

## Installation

### **1. Clone the Repository**
```sh
 git clone https://github.com/AedynSimon/cipher-encryption.git
 cd cipher-encryption
```

### **2. Compile the Java Files**
```sh
 make
```

## Usage

The program takes **five command-line arguments**:
```sh
 java Cipher <cipher_type> <input_file> <output_file> <key_file> <mode>
```
Where:
- `<cipher_type>`: `B` for **Block Cipher**, `S` for **Stream Cipher**
- `<input_file>`: Path to the file to be encrypted/decrypted
- `<output_file>`: Path to save the encrypted/decrypted file
- `<key_file>`: Path to the encryption key file
- `<mode>`: `E` for **Encryption**, `D` for **Decryption**

## Example Commands

### **Block Cipher Encryption:**
```sh
 java Cipher B plaintext.txt encrypted.txt keyfile.txt E
```

### **Block Cipher Decryption:**
```sh
 java Cipher B encrypted.txt decrypted.txt keyfile.txt D
```

### **Stream Cipher Encryption:**
```sh
 java Cipher S plaintext.txt encrypted.txt keyfile.txt E
```

### **Stream Cipher Decryption:**
```sh
 java Cipher S encrypted.txt decrypted.txt keyfile.txt D
```

## Contributing

Contributions are welcome! Feel free to fork the repository, submit pull requests, or report issues.

## Contact
Email: [aedynsimon@gmail.com](mailto:aedynsimon@gmail.com)
GitHub: [github.com/AedynSimon](https://github.com/AedynSimon)
