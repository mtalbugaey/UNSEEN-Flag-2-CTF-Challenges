# Overview
<b> Points:</b> 50
<br>
<b>Category:</b> Network

# Description
The life is step by step. Take it slow, and remember who is taking care of the names behind the address.
<br>
Flag Format: <b>IAU_CYS{}</b>

# Challenge File
[Names_Addresses.pcap](./Names_Addresses.pcap)

# Solution
When we go to Statistics, then Protocol Hierarchy:<br>
We can notice the use of DNS.
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/34223466-9ca2-47db-903d-4b382a558443" width="1000"></kbd>
<br><br>
So we apply it as a filter:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/d55bb3ab-51ef-4c53-8f2e-46a9f60c4186" width="1000"></kbd>
<br><br>
<br> We can notice there are multiple unusual and wired website names:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/147d7db2-178d-481a-a6dd-d92fb301791c" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/36de02f2-fc9a-47cd-8d30-782e2ab8890e" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/2a51687e-f572-49f6-8f7c-b7eef8f9e5e9" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/dae8cfb2-94b6-4708-9ba0-e36e815a732e" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/6c5efe91-94a8-45ae-9485-152800c6d79a" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/5af1e408-ec3d-440c-a579-4ba4ed9ac12c" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/7c2ca6ef-0e38-4740-8f7b-67ec47097194" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/f69fde8d-2b1b-4c59-b982-d749970d3f63" width="1000"></kbd>

<br>
Then, when we took these names, we came up with text similar to the hex value.
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/015a2e26-8b4f-45c8-85d0-ef2066662a18" width="1000"></kbd>

<br><br>
Then we go to the CyberChef: https://cyberchef.org/<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/09eb8c51-c858-42a0-8ba2-4d7b03f6afd6" width="1000"></kbd>
<br> and here's the flag.

# Flag
IAU_CYS{usm4rt}

