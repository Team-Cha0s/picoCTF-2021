## Static ain't always noise

This problem requires you run the bash script with the 'static' file, then search through the outputted file for the flag

```bash
$ wget https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/static
$ wget https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/ltdis.sh
$ chmod +x ltdis.sh
$ cat static.ltdis.strings.txt | grep 'pico'
1020 picoCTF{d15a5m_t34s3r_f5aeda17}
```

### Flag
`picoCTF{d15a5m_t34s3r_f5aeda17}`
