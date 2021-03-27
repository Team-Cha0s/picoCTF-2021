## Magikarp Ground Mission

This problem requires you ssh into the server, then navigate through the directories to piece together the flag

```bash
$ ssh ctf-player@venus.picoctf.net -p 53750
ctf-player@venus.picoctf.nets password: ee388b88
$ cat 1of3.flag.txt
picoCTF{xxsh_
$ cd ../../../
$ cat 2of3.flag.txt
0ut_0f_\/\/4t3r_
$ cd home/ctf-player/
$ cat 3of3.flag.txt
3ca613a1}
```

### Flag
`picoCTF{xxsh_0ut_0f_\/\/4t3r_3ca613a1}`

