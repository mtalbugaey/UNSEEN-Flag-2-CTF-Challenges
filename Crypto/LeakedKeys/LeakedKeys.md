# Overview
<b> Points:</b> 90
<br>
<b>Category:</b> Crypto

# Description
oops!! I believe some of the RSA keys were leaked.


# Challenge File
[Leaked_Keys.py](./Leaked_Keys.py)

# Solution
When opening the Python file, we can see three keys were leaked (P, N, and e).
<br>
<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/60a125e0-2b98-439b-bb37-a541acf89a2a" width="1000"></kbd>
<br><br>
We can take advantage of these keys to calculate the other keys needed by using any online RSA calculater.
<br>
I'm using this website: <b>https://www.tausquared.net/pages/ctf/rsa.html</b>.
<br><br>
<br><br>
Enter the values for p and N to calculate q
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/a0c3f9f8-e70f-43a6-aa81-f0a71460f3ff" width="1000" ></kbd>

<br><br>
After the q calculation:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/5e88ccd7-88f1-4fee-accf-de239486a0d0" width="1000" ></kbd>

<br><br>
Now we enter the N value to calculate phiN:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/aa5ee647-ce83-4322-97ba-5bec6e720eac" width="1000" ></kbd>


<br><br>
To calculate d, we can use the same website or use the exiting function (invers) in the Python file:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/60c8c889-5271-4e19-9d11-6fdb4902b23d" width="1000" ></kbd>
<br><br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/6fcd16fc-b3d4-40cf-ad3a-730663b014cd" width="1000" ></kbd>

After we put the calculated values of q, phiN, and d in the Python file, we run it:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/b4d34b32-a77b-4204-821c-5a35a9ed9c17" width="1000" ></kbd>
<br><br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/14541771-0760-4fb5-918a-7f2cb08fb0b1" width="1000" ></kbd>

# Flag
IAU_CYS{RS4_n0t_34zy_101}


