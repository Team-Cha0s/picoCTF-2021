>What could go wrong if we let Word documents run programs? (aka "in-the-clear"). Download file.

This chall gives us a word document with macros embedded into it, to solve it I decided to open up the macro embedded into the file, the way to do this is to open up microsoft words and open up the macros feature and through there you come accross the coded macro below:

```py
 Sub runpython()

Dim Ret_Val
Args = """" '"""
Ret_Val = Shell("python -c 'print(\"cGljb0NURnttNGNyMHNfcl9kNG5nM3IwdXN9\")'" & " " & Args, vbNormalFocus)
If Ret_Val = 0 Then
   MsgBox "Couldn't run python script!", vbOKOnly
End If
```

At first glance I did not notice anything, but after a bit more analysis I thought that the string given is a bit promising so I tried it with a bunch of different decoders and it turned out to be base-64. So after decoding I recieve the flag below:

>picoCTF{m4cr0s_r_d4ng3r0us}