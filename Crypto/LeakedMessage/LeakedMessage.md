# Overview
<b> Points:</b> 120
<br>
<b>Category:</b> Crypto

# Description
I finally obtained the encrypted message with its private key. but unfortunately, I can't break the encryption scheme. Should I continue or what?

# Challenge File
[Top_Secret](./Top_Secret)
<br>
[UNSEEN2_private.pem](./UNSEEN2_private.pem)

# Solution
When we show the content of the first file <b>Top_Secret</b>, we will find that it is encrypted.
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/75d99d36-f98c-46ea-9d9b-265cbae941a8" width="1000"></kbd>

Then, when we open the <b>UNSEEN2_private.pem</b> we know the RSA was used as an encryption algorithm.
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/b6bf7f73-5c72-4e3b-8a74-759818d66087" width="1000"></kbd>

<br><br>

So, we used this command to decrypt the <b>Top_Secret</b> file by using the file key <b>UNSEEN2_private.pem</b>.
```
openssl rsautl -decrypt -in Top_Secret -out DecTop_Secret -inkey UNSEEN2_private.pem
```

<br>
Then, this is the <b>decryption</b> of the <b>Top_Secret</b> file, it looks like a binary value.
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/f4093365-f702-4792-8c7a-8e9d18d49fc4" width="1000"></kbd>
<br><br><br>

So, we go to the CyberChef: https://cyberchef.org/
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/f2fc1372-a97d-4e11-82c9-bbd134309832" width="1000"></kbd>
We can notice the last line was not decrypted, but when we read the text carefully, we find a hit saying "continue <b>or</b> what"<br>

So from the word <b>"or"</b>, we will use the OR operation.
<br> and we will put the last line as a key.
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/b6a58742-ffae-409e-a9ac-b07f939e132f" width="1000"></kbd>

And yesss!! That's  the flag ;).

# Flag
IAU_CYS{v1rsu}

