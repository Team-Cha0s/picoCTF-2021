## Tab, Tab, Attack

This problem requires you to unzip the file, and 'cd' into all the directories until you find a file. You then need to search the file for the flag.

```bash
$ wget https://mercury.picoctf.net/static/72712e82413e78cc8aa8d553ffea42b0/Addadshashanammu.zip
$ unzip Addadshashanammu.zip 
$ cd Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku
$ strings fang-of-haynekhtnamet | grep 'pico'
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_6f332f10}
```

### Flag
`picoCTF{l3v3l_up!_t4k3_4_r35t!_6f332f10}`

