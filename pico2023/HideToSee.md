## Details:
Challenge name: HideToSee

Category: Cryptography

Description:
How about some hide and seek heh?
Look at this image [here](https://artifacts.picoctf.net/c/235/atbash.jpg).

## Solve:

Opening the file, we can see that it is a picture of the Atbash cipher:

![atbash](https://github.com/uuu2q/ctf-writeups/assets/134032122/c9ef5e24-2f6f-4f36-8738-7688f136652f)



I then put the image through [Aperi'Solve](https://www.aperisolve.com/). 
Looking through the summary, I noticed that the Steghide section has an `encrypted.txt` file, which likely contains the flag:

<img width="1065" alt="Steghide" src="https://github.com/uuu2q/ctf-writeups/assets/134032122/c6078822-44d8-4c30-a846-0737b988870f">



Downloading and opening the Steghide file, we get `encrypted.txt`, which says: "krxlXGU{zgyzhs_xizxp_92533667}".

Since the source file references the Atbash cipher, I tried using an [Atbash cipher decoder](https://www.dcode.fr/atbash-cipher) and got the flag:

picoCTF{atbash_crack_92533667}

