>Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: this

By the name of the file and description I thought that there could be files embedded within this file so from my previous experience I know that there is a 'matryoshka' command which can be used with -M.

So I typed 
```bash
binwalk -e -M dolls.jpg
```
 in the terminal and navigated till I found something intresting and I did, I found a flag.txt in the directory:
```
C:\Users\MAIN\Downloads\_dolls.jpg.extracted\base_images\_2_c.jpg.extracted\base_images\_3_c.jpg.extracted\base_images\_4_c.jpg.extracted
```
which contained the flag.txt.

>picoCTF{e3f378fe6c1ea7f6bc5ac2c3d6801c1f}
