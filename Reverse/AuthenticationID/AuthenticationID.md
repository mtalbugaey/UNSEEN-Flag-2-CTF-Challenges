# Overview
<b> Points:</b> 80
<br>
<b>Category:</b> Reverse

# Description
I forgot my authentication ID. Can you help me find it out? This ID is needed to run this application.


# Challenge File
[Authentication_ID.exe](./Authentication_ID.exe)

# Solution
When we open the executable file, it keeps asking for the authentication ID.
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/fa8eeb1c-c2e6-4d92-b8b3-eaac1c437000" width="700"></kbd>

<br><br>
Since we didn't know the ID, we go to IDA to performe the static anaylsis.<br>
And here's the view of main function:<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/a6bd872e-7c33-4c0b-b8f1-220c5bae6de8" width="700"></kbd>

<br><br>
We notice there is a call for the "print" function. <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/3e932c9b-3d2f-4d32-b62e-8edb9ed78ada" width="700"></kbd>
<br><br>

When we go to the "print" function, we see another call for the "print2" function. <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/9129b938-d1ba-4506-9cc7-22159a9c1b30" width="700"></kbd>
<br><br>

When we go to the "print2" function, we see multiple calls and print. <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/4881df33-efc0-4aca-8259-68d5e3e1100e" width="700"></kbd>
<br><br>

We decided to go to the "print5" function. <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/ee12ca0d-57d4-4fa0-986f-85eec117f15c" width="700"></kbd>
<br><br>

Since the passed parameter is 55h, it is greater than 54h, so we will go to the left block. <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/ce02ea93-0480-4385-9d66-0b572eec8e7f" width="700"></kbd>
<br><br>

After that, we go to the value, and we copy it. <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/cdd8da43-6a32-456a-985d-7c2b239b2334" width="700"></kbd>
<br><br>


Then, we go to CyberChef: https://cyberchef.org/ <br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/3df5fa6c-70e0-4860-9731-cbe493df1a81" width="700"></kbd>
<br>
And we find it :).

# Flag
IAU_CYS{R3v3r5e_3ngineer_3his}
