# Overview
<b> Points:</b> 170
<br>
<b>Category:</b> Stego

# Description
Help the blind person to find his glasses. he cant see without them!

# Hint
We need to learn the blinds language so we can communicate with them 

# Challenge File
[Blind.jpg](./Blind.jpg)

# Solution
In this challenge we can see a jpg file, since it is in strgonography category we will try to steganalysis it using <b>stegseek</b> or <b>steghide</b> 
![image14](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/e2fc3f69-9af2-482d-85d1-e5eaec1ac279)

But none of them will work unless you find the passphrase!
![image15](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/c8828096-118d-4277-af02-07d162186b9f)

If we investigate the source file, we will see some data at the end of the code!
![image16](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/56051b36-5e19-408f-934f-724a85242599)

If you think it is a normal base2 code, you are wrong! You will not find any useful data when you convert it.
<br>
So, let's think of the picture and the name of the challenge?
<br>
It says blind… it is possible that they mean Blind Language? 
<br>
Yess it is!
<br>
Go to any website that translates from Braille to text. 
<br>
Here is one: https://abcbraille.com/braille

![image17](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/4ea15092-4cba-47a6-9502-b599c8b3509f)

As you can see, every character in Braille represented by of 6 dots
![image18](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/1cb24f48-b8c0-4c5a-b122-b6e887f98f6f)

This is how the data looks like in Braille.
<br>
Now let's convert them!

![image19](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/78a0d10f-e238-4a56-994c-8d977140c20f)

Here you got the passphrase! 
<br>
Now we go back to Kali to enter the passphrase.
![image20](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/45fe2042-328c-44ed-8f9b-a22592f4b32e)

![image21](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/7e5f94d5-d09d-43b9-beb9-a9462916568e)

Re-enter the password. 
<br>
![image22](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/d74eb126-b77c-4909-9aaf-1cfe317a1dff)
<br>
And here it is!!

# Flag
IAU_CYS{6_Out_of_6}
