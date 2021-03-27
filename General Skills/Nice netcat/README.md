## Nice netcat...

This problem requires you run the command provided and convert the decimal code into ASCII

```python
# Import Libraries
from pwn import *
import re

# Connect to server
p = remote("mercury.picoctf.net", 7449)

# Get and format output
output = p.recv()
output = output.decode('utf-8')
output = output.replace("\n", "")

# Convert output to ASCII
output = ''.join(chr(int(x)) for x in output.split())

# Print Flag
print(output)
```

### Flag
`picoCTF{g00d_k1tty!_n1c3_k1tty!_f2d7cafa}`
