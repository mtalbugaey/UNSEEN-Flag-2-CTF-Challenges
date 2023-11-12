# Overview
<b> Points:</b> 30
<br>
<b>Category:</b> Network

# Description
I always get empty results!! what is happening?


# Challenge File
[Empty_Result.pcap](./Empty_Result.pcap)

# Solution
When openning the pcap file, we can see there is multiaple HTTP POST requests. <br>
we can use the following filter:
```
http.request.method == "POST"
```
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/4f1495a6-f4f4-4f36-9ef4-5e6d292cf6f1" width="1000"></kbd>

And when we inspect these records, we can find these searches:
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/b27fecb0-704d-41a5-a37a-597093418672" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/7128bddf-5e5c-4ac7-ae23-f516a1a04eb7" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/9af44a2e-ae90-430c-8e30-3687677268e6" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/b6573ed4-cbd1-491d-883b-bd225d00ad60" width="1000"></kbd>
<kbd><img src="https://github.com/mtalbugaey/UNSEEN-Flag-2-CTF-Writeups/assets/126514202/780f63c5-b1be-42ec-ab7f-fef384411a93" width="1000"></kbd>

<br><br>
Then we combine these words to get the flag ;).

# Flag
IAU_CYS{Http_n0t_s4f3}


