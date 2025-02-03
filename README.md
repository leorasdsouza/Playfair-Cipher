# Playfair-Cipher

## Overview
This program implements the **Playfair Cipher**, a cryptographic algorithm that encrypts and decrypts text in pairs of letters. It is a more complex and secure encryption method compared to classical ciphers. The program provides both **encryption** and **decryption** functionalities.

## Open in Google Colab
Click the button below to run the program directly in **Google Colab**:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/leorasdsouza/Playfair-Cipher/blob/main/PlayfairCipher.ipynb)

## Features
- Encrypts text using a user-specified key.
- Decrypts the encrypted text to retrieve the original message.
- Automatically replaces 'J' with 'I' during encryption and decryption (as per the Playfair cipher standard).
- Handles plaintext with odd lengths by adding an 'X' at the end.

## How It Works
1. The **key** provided by the user is used to generate a 5x5 matrix for encryption and decryption.
2. The input text is converted into uppercase, and spaces are removed.
3. If the text has an odd number of characters, an 'X' is added to the end to make the length even.
4. The program processes the text in pairs of characters:
   - If the characters are in the same row, they are replaced by the character to the right (wraps around).
   - If the characters are in the same column, they are replaced by the character below (wraps around).
   - If the characters are in different rows and columns, they form a rectangle and swap the corners.
5. For decryption, the same rules apply but characters are shifted to the left or above instead of right or below.

## Usage Instructions

### Running the Program
1. **Run in Google Colab** by clicking the **"Open in Colab"** button above.
2. Alternatively, download the script and run it locally in:
   - Python (3.x) environment
   - Jupyter Notebook
   - VS Code / PyCharm
3. Enter the required inputs when prompted:
   - A **key** for the Playfair cipher.
   - A **plaintext message** to encrypt.
4. The program will output:
   - The **encrypted message**.
   - The **decrypted message** for verification.

### Sample Output
![image](https://github.com/user-attachments/assets/94b2b251-f57d-439a-b9bc-eede2e94497b)
![image](https://github.com/user-attachments/assets/9c384b0a-9f42-4ac1-bc8d-0e3306cd1ebc)


