## Details:
### Challenge name:
rotation

### Category:
Cryptography

### Description:
You will find the flag after decrypting this file<br> Download the encrypted flag [here](https://artifacts.picoctf.net/c/386/encrypted.txt).

### Solve:
Opening the source file, `encrypted.txt`, we get this: `xqkwKBN{z0bib1wv_l3kzgxb3l_4k71n5j0}`.

Upon first glance, I thought it was Caesar cipher, especially since the start, `xqkwKBN`, has two occurances of the letter 'k', which probably represents 'c' in picoCTF.

Putting the ciphertext into a [Caesar cipher decoder](https://www.dcode.fr/caesar-cipher), we get the flag: `picoCTF{r0tat1on_d3crypt3d_4c71f5b0}`.
