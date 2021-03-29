## Information

This problem requires you to view the metadata of the file. When you do this you will see a base 64 encoded string as the license value. If you decode this you get the flag 

```bash
$ wget https://mercury.picoctf.net/static/d1375e383810d8d957c04eef9e345732/cat.jpg
$ exiftool cat.jpg
License: cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9
```

I used this website to decode the base 64: https://www.base64decode.org/

### Flag
`picoCTF{the_m3tadata_1s_modified}`
