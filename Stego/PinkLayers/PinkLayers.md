# Overview
<b> Points:</b> 80
<br>
<b>Category:</b> Stego

# Description
I love the color pink. Here are my favorite 8 layers of pink.


# Challenge File
[Pink_Layers.png](./Pink_Layers.png)

# Solution
When opening the file, we can see an image with 8 layers of pink.
<br><br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/0c424cf7-74a3-4a37-893c-7bcb03bd5b24" width="500"></kbd>

When we look at the picture and read the description carefully, we notice a hint, which is <b>8 layers</b>.<br>
and as we know any image made of 8 layers.

<br><br>
Go to the <b>StegOnline</b>: https://stegonline.georgeom.net/upload
<br>
and browse the bit plane of the image:
<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/2cb72798-0cb3-4d8f-b85a-8b3577c7260c" width="845"></kbd>

<br><br>
We can notice in <b>Red 1</b> and <b>Blue 0</b> there are pixel glitches, which is an indication of hidden data.

<figure markdown>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/7a3cbd04-9539-4868-bab2-7984e81ff63f" width="400"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/fc2c18d7-9f50-4a81-9277-97c831b33a90" width="425"></kbd>
  
</figure>

<br><br>
Then we go to <b>Extract Files/Data</b>: <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/15cdd70e-7097-4d6b-a99f-6a30143809c5" width="845"></kbd>
<br>
<br>
Select the Red 1 and Blue 0:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/633e8862-f21b-4d63-8d98-93da4dddc1c1" width="845"></kbd>

<br><br>
Then download the extracted data:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/7bd1231d-bf09-4f06-903b-ab7701b5ea13" width="845"></kbd>

And here is the flag ;).<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/09662e72-995d-4f8a-9608-073ad580118f" width="500"></kbd>


# Flag
IAU_CYS{1s_w4s_t00_3asy}

