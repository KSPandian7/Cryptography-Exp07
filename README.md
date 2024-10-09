# ADVANCED-ENCRYPTION-STANDARD-DES-ALGORITHM

## Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

## ALGORITHM:
step 1 :AES is based on a design principle known as a substitution–permutation.<br>
step 2 :AES does not use a Feistel network like DES, it uses variant of Rijndael.<br>
step 3 :It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.<br>
step 4 :AES operates on a 4 × 4 column-major order array of bytes, termed the state<br>

## PROGRAM:

```c
#include <stdio.h>
#include <string.h>


  void xor_encrypt_decrypt(char *input, char *key) {
int input_len = strlen(input);
int key_len = strlen(key);

for (int i = 0; i < input_len; i++) {
    input[i] = input[i] ^ key[i % key_len]; 
}
}

int main() {
char txt[] = "KULASEKARAPANDIAN K";
char key[] = "secretkey"; 

printf("Plain Text: %s\n", txt);

xor_encrypt_decrypt(txt, key);
printf("Encrypted Text: %s\n", txt);

xor_encrypt_decrypt(txt, key);
printf("Decrypted Text: %s\n", txt);

return 0;
}
```

## OUTPUT:
![Screenshot 2024-10-09 161531](https://github.com/user-attachments/assets/e062d872-7df5-48f1-8218-393a77dbb931)

## RESULT:
Hence,to use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption is done successfully.
