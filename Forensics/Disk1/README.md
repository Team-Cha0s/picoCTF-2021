>Use srch_strings from the sleuthkit and some terminal-fu to find a flag in this disk image: dds1-alpine.flag.img.gz

To solve this all I had to do was grep for "pico" using the command below

>cat dds1-alpine.flag.img|strings|grep pico

The command above was able to search for any strings containg "pico" within that file ```dds1-alpine.flag.img``` doing so this is what I got in return:

>ffffffff81399ccf t pirq_pico_get
ffffffff81399cee t pirq_pico_set
ffffffff820adb46 t pico_router_probe
  SAY picoCTF{f0r3ns1c4t0r_n30phyt3_ad5c96c0}

Moreover the flag was the in the last line:  ```picoCTF{f0r3ns1c4t0r_n30phyt3_ad5c96c0}```
