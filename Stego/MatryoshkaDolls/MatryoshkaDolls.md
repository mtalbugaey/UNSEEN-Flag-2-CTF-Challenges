# Overview
<b> Points:</b> 30 
<br>
<b>Category:</b>  Stego
# Description
Matryoshka dolls are interesting ;)

# Challenge File
[Matryoshka_dolls.jpg](./Matryoshka_dolls.jpg)

# Solution
When opening the file, we can see 3 dolls:<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/a062cb09-1fd3-485d-9723-660d2e59028d" width="500"></kbd>
<br><br>
The Matryoshka dolls are a set of dolls of decreasing size placed one inside another.<br>
We will use the <b>Stegseek</b> to extract other dolls, by using this command:<br>
```
stegseek Matryoshka_dolls.jpg 
```

After that, this image was extracted:<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/21330e62-739f-4285-bc0a-865805d6ba55" width="500"></kbd>
<br><br>
We keep continue:
```
stegseek Matryoshka_dolls.jpg.out
```

Then this image was extracted:<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/0d533101-8a21-4339-9d0e-6c58eb62cbaa" width="500"></kbd>
<br><br>

We keep continue:
```
stegseek Matryoshka_dolls.jpg.out.out
```
<br><br>
Then this text file was extracted, which is the flag :).<br>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/86da4f3c-8482-45d9-9bae-36b930549460" width="500"></kbd>



# Flag
IAU_CYS{H1dd3n_St3go}

