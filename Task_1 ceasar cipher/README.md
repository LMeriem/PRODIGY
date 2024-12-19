# Caesar Cipher

A Python program to encrypt and decrypt text using the Caesar Cipher algorithm. The program allows users to input a message and a shift value to perform encryption and decryption.

## Features
- Encrypt text by shifting characters by a given value.
- Decrypt text using the same shift value.
- Supports both uppercase and lowercase letters.
- Keeps non-alphabetical characters unchanged.

## Requirements
- Python 3.x

## Installation
1. Clone the repository or download the script:
   ```bash
   git clone https://github.com/your-repo-name/caesar-cipher.git
   cd caesar-cipher
   ```

2. Ensure Python 3 is installed on your system.

## Usage
Run the script in your terminal:

```bash
python caesar_cipher.py
```

Follow the prompts:
1. Choose a mode (`encrypt` or `decrypt`).
2. Enter the text you want to process.
3. Input the shift value (integer).

### Example
**Encryption:**
```
Caesar Cipher Program
Choose mode ('encrypt' or 'decrypt'): encrypt
Enter the text: Hello World
Enter the shift value (integer): 3

Result (encrypted text): Khoor Zruog
```

**Decryption:**
```
Caesar Cipher Program
Choose mode ('encrypt' or 'decrypt'): decrypt
Enter the text: Khoor Zruog
Enter the shift value (integer): 3

Result (decrypted text): Hello World
```

## How It Works
The Caesar Cipher shifts each alphabetical character in the input text by a fixed number of positions based on the ASCII table. Non-alphabetical characters are not modified.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contributing
Feel free to submit issues or pull requests for improvements or bug fixes.

