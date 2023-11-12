# Overview
<b> Points:</b> 100
<br>
<b>Category:</b> Forensics

# Description
I received this secret message, but I can't figure out the secret. As they say "don`t follow your shadow"


# Challenge File
[Color_Palette.png](./Color_Palette.png)

# Solution
When we open the file, we can see multiple different shades of blue.
<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/b33288cd-6218-450b-95eb-5da08a65a730" width="500"></kbd>
<br> <br>

Then, when we pick the color shades for each circle, we notice that each of them has a different RGB value (we focus on the blue one).
<figure markdown>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/15e70fff-c69b-4f0b-adcd-a396ed8aaaa7" width="490"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/74deb06c-a169-4f36-ab03-cad9afa275b0" width="490"></kbd>

</figure>
<br> <br><br>

After we picked all the blue values, we came up with this text:
```
73 65 85 95 67 89 83 123 102 49 110 100 95 109 51 125
```
<br><br>
After that, we go to CyberChef: https://cyberchef.org/
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/63045893-30bf-4e10-908f-fde6fc183a9b" width="1000"></kbd>
and that's the flag :).

# Flag
IAU_CYS{f1nd_m3}
