## Details:
### Challenge name: 
money-ware

### Category/tags: 
General Skills, osint

### Description:
Flag format: picoCTF{Malwarename}<br>
The first letter of the malware name should be capitalized and the rest lowercase.<br>
Your friend just got hacked and has been asked to pay some bitcoins to 1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX. He doesn’t seem to understand what is going on and asks you for advice. Can you identify what malware he’s being a victim of?

## Solve:

When I first tried to solve this, I tried searching for online bitcoin address lookups, but none of the results had information about the malware.

I then tried searching "bitcoin malware 1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX" on Google, and that's when I found information about a certain bitcoin malware attack called "NotPetya."

<img width="716" alt="Screen Shot 1" src="https://github.com/uuu2q/ctf-writeups/assets/134032122/39ac7601-358d-45e3-9be4-90d593147093">

When I tried inputting the flag, `picoCTF{Notpetya}`, it did not work, so I scrolled a little more until I saw its other name, Petya:

<img width="742" alt="Screen Shot 2" src="https://github.com/uuu2q/ctf-writeups/assets/134032122/817fc04a-7c43-4635-886b-11c75d4d9c44">

`picoCTF{Petya}` worked.
