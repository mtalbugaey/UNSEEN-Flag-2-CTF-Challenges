# Overview
<b> Points:</b> 60
<br>
<b>Category:</b> Stego

# Description
My other half is missing, try to find us

# Challenge Files
[Foreground.png](./Foreground.png)
<br>
[Background.png](./Background.png)

# Solution
Download and open the PNG files 

<figure markdown>
  
![image1](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/122155e6-8d79-4a20-8b0a-91f2e875a6e5)
![image2](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/cc44b085-cd6b-4acc-b425-cdcda61ae58e)
</figure>

We notice that the text is not clear, and it seems that the piece of text in each picture completes the flag.
<br>
Let’s try the Stegsolve tool in Kali.

![image3](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/31cf49b3-afcf-4678-98d6-9d7453cbbdbc)

Use this command to open the tool. 
<br>
Notice: it requires preinstallation 
![image4](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/88f93329-980c-4a66-bb8b-a4a133e758a0)
This is how the window tool look like 
<br>
Open the "Background" PNG file
![image5](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/fdecc2a6-555d-4d40-94ac-cedc2fd25301)
We can change the colors using the arrows at the button 
<br>
It looks much clearer now!

![image6](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/f60797d0-8b71-4760-8236-39b6558a24a5)

Let's add the "Foreground" PNG file from analysis tab, then Image Combiner

![image7](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/242dfae0-f4c0-4b75-87fb-b0e34b908993)

Now we can see the flag!

# Flag
IAU_CYS{oki*doki}
