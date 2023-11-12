# Overview
<b> Points:</b> 120
<br>
<b>Category:</b> Forensics

# Description
What about a stepbrothers hate each others? one of them want to destory the other Focuse on the numbers


# Challenge File
[Manipulation.zip](./Manipulation.zip)

# Solution
We have this email image
<br>
Two clues: Eva Rivera, Ahmed Reda
<br>
![image27](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/517ea3b8-254e-458c-ab22-371fd07c7d62)

Go to excel and search for Eva name 
<br>
![image28](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/f5f89de5-9649-4331-99ec-30c06baee7af)

Notice the dates. She only stayed for two days:
<br>
![image29](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/b6d07d6d-616a-4434-aa7f-8e0a060194f2)

As Ahmed Reda is the brother, so we will search for the father name ‘Reda’ to find the other brother
<br>
Notice the salary cell!! Too much salary is it?
<br>
![image30](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/0e7d2850-e5ec-48aa-806f-209a77baa22b)

Think more and see if there are any hidden sheets
<br>
![image31](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/e4fce395-cf3f-4ffa-8cbf-dc1f837778a2)

Pingo! We have one
<br>
Observe that Bader Reda row number is 83 ->  so we go to the same row -> the salary cell, oh! Encoded 
<br>
![image32](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/9b27c329-bd55-4728-aded-b888747b0e02)

That’s it! The flag with Base 32 :0 
<br>
![image33](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/de6ee4ad-4c01-470d-8cbe-61e86c9815ff)

# Flag
IAU_CYS{manpluatingCell}

