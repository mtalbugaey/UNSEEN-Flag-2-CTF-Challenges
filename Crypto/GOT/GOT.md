# Overview
<b> Points:</b> 70
<br>
<b>Category:</b> Crypto

# Description
Is it good to try many times?


# Challenge File
[GOT.zip](./GOT.zip)

# Solution
When extracted the Zipped file we’ll have three files:
<br>
![image1](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/daa1d19b-30c1-4e4e-82d7-8db1fd47cb53)

First image ‘1’ it has Vinegar photo, seems as a hint 
<br>
![image2](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/1266300c-d93b-4032-a59f-05704a809773)

Second image ‘2’ has a key photo, also null inside so seems as a hint.
<br>
![image3](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/2c01cf24-4edc-417e-bf9c-ca7778bc94c4)

When we open third image ‘Stark’s’ 
<br>
![image4](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/ba9868ac-50ff-4232-bda1-0fb74902f3ab)

You can put it in HxD or any Hex Editor but for simplicity we will change the extinction to .txt
<br>
![image5](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/cc35967b-b49a-42f1-8374-b24975669dc9)

When we reach end of file, notice there is encoded message
<br>
![image7](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/aca9e887-f631-4014-963f-8eeaf27c3565)

Decoded first with Base58 
<br>
![image6](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/f5ed6163-5bc5-4cb0-bc15-6d285ede541f)

Then decoded with Base64
<br>
![image8](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/9de7b1a2-e8cf-4f30-8b03-50e9b44e5e1a)

For seek for the two hints, we will take the Vigenère Cipher-> The password is ‘key’.
<br>
The flag Decoded  
<br>
![image9](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/82e22c0c-a02f-471d-a4b1-62bd6eb6aed3)


# Flag
IAU_CYS{JON+TYRION<3}


