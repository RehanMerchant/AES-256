# Simplified AES Block Cipher Simulator
Simplified AES Block Cipher Simulator
A command-line C program that simulates the fundamental transformations of the Advanced Encryption Standard (AES). It processes a single 128-bit block of data (16 characters) and visualizes the state matrix in memory during the encryption process.

### Disclaimer
This is an educational toy cipher, not a secure or complete implementation of AES-256. It deliberately omits MixColumns, Key Expansion, and multiple encryption rounds to simplify the demonstration of basic state matrix operations. Do not use this for actual data security.

## Features
- Interactive CLI: Simple menu-driven interface to encrypt, decrypt, and view state status.
- Core Transformations: Implements standard AES SubBytes, ShiftRows, and AddRoundKey functions (along with their inverse operations).
- State Matrix Visualization: Prints the 4x4 data matrix in hexadecimal format after encryption.
- In-Memory Processing: Holds the encrypted cipher state in RAM until decrypted or overwritten.

## Compilation

You will need a standard C compiler (like gcc) to build the executable. Run the following command in your terminal:

```
gcc -o aes_simulator main.c
```

## Execution
Run the compiled executable:
```
./aes_simulator

```


## Usage Guide
When you launch the program, you will be presented with a menu showing the current status of the memory ([EMPTY] or [LOCKED DATA IN RAM]).

1) Encrypt & Store Message: * Prompts you for a plaintext message (up to 16 characters).
   - Prompts you for a secret key (also up to 16 characters).
   - Applies the cipher transformations and displays the resulting hexadecimal state matrix.
  
2) Decrypt & Clear Memory: * Requires the exact secret key used during encryption.
   - Reverses the operations (AddRoundKey, InvShiftRows, InvSubBytes).
   - Prints the recovered plaintext and clears the memory matrix.

3) Exit: Terminates the program. Any data left in memory is lost.


## Team
- Aditi Mohapatra
- Avinash Sahani
- Poorbasha Kar
- Sk Md Rehan

Guided By- Mr. Vijay Kumar Meena










