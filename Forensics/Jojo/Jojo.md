# Overview
<b> Points:</b> 110
<br>
<b>Category:</b> Forensics

# Description
Be a fast insvistigator and find what Jojo is hiding, as she has a favorite number
<br>
Flag Format: <b>IAU_CYS{}<b/>


# Challenge File
[Jojo.zip](./Jojo.zip)

# Solution
When extracted the Zipped file we’ll have multiple files:
<br>
![image15](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/1d94ba92-beeb-49b4-9896-5b7813afe2e2)

A tweet.jpg
<br>
![image16](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/68578b3d-df4d-436e-9d93-8be2e4eaa9cb)

exam leakage.jpg
<br>
![image17](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/7d988ed2-64c1-4236-9fbd-8ced59e9ba5a)

Hmmm.txt
<br>
![image18](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/f5277f10-d4ad-4c74-a0a6-a31190952a82)

Termination of Enrollment Announcement.docx
<br>
We will see a lot of hints, as we have a twitter account link
<br>
![image20](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/467c5022-2795-4a06-b153-2ad638d017fc)
<br>
![image22](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/1521ea07-145e-4df8-93b6-859e7c740d33)

After going through tweets, we will see encoded base64 message 
<br>
![image23](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/74b50660-a1b8-4e87-a6eb-eef2ef57c22b)

After decoded it, we will see part of the flag as isn’t complete if we insert it there
<br>
![image24](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/d3a5381d-d554-4557-9054-db5b926413d6)

This tweet is a big hint as if you go through files, tweets you will notice number ‘5.5’ is repeating 
<br>
![image26](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/eaf6de3e-8c3a-4386-bf7e-acea52131d14)
<br>
![image25](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/1fff2bff-16bb-4830-bd25-de4bd231b15d)


# Flag
IAU_CYS{IhateJAU5.5}
