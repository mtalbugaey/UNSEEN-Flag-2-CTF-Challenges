# Overview
<b> Points:</b> 80
<br>
<b>Category:</b> Forensics

# Description
Live is full of ups and downs!
<br>
but you need to know where to stop and where to continue

# Hint
Base 2

# Challenge File
[A.wav](./A.wav)
<br>
[ups_and_downs.mp4](./ups_and_downs.mp4)

# Solution
We have two files, one is an audio file, and the other is a video. 
<br>
After investigating the audio file, it has nothing!
<br>
But the video file looks like this:

![image12](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/664c88b8-502d-4863-b55b-668b574ae56e)

When thinking of the name and description "Ups and Downs" and the video has go a picture of audio waves, maybe they mean ONE ==> Ups and ZERO ==> Downs!

So, let’s try by replacing the short line by zero and the tall line by one
<br>
01111011 01000001 01101100 01110111 01100001 01111001 01110011 01000000 01100010 01100101 00100100 01010101 01010000 01111101 00001010
<br>
Then convert them from binary to text.
<br>
And trrraaa! We got the flag.
![image13](https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/d708e78b-9290-49a7-8590-275f7dd100ed)


# Flag
IAU_CYS{Always@be$UP}
