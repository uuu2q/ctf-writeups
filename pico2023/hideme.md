## Details:
Challenge name: hideme

Category: Forensics, steganography

Decription:
Every file gets a flag.
The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/258/flag.png).

## Solve:

I first put the image through [Aperi'Solve](https://www.aperisolve.com/). 
Looking at the Binwalk section, I noticed that there were some extra files in the `flag.png` provided by the challenge; in particular, `secret/flag.png` likely contains the flag.

<img width="1053" alt="Screen Shot 2023-08-02 at 09 38 06" src="https://github.com/uuu2q/ctf-writeups/assets/134032122/f1a9a555-91b0-4f8b-b069-b91fe80dac85">


After downloading the Binwalk files, we navigate to `secret/flag.png` and find an image, which displays the flag:

<img width="943" alt="Screen Shot 2023-08-02 at 09 43 28" src="https://github.com/uuu2q/ctf-writeups/assets/134032122/0984375a-b39c-4b0c-926a-29c9d964bf1f">

