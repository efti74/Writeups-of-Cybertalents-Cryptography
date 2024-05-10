# Up Cybertalents Problem

__Problem Link:__ [Up](https://cybertalents.com/challenges/cryptography/up)
---

__Description:__ Every time you go up you will gain one ballon

ejxc{T0nY0J_BsUMS4} 

### My Approach:

1. First of all it cannot be solved by any online tool.
2. Read the description very carefully. It says `everytime you go up` means everytime I have to add 1 to the previous value then add with the character.
3. In the below python script you will see the code.
4. Remove the curly braces `{}`
5. After getting the flag remain the same number in the cipher text. That means there are 3 numbers 0, 0, 4. Put this same after getting the plain text.

```python
cipher = "ejxcT0nY0JBsUMS4" # i just remove the {} braces and underscore.
plain = ''
j = 1 # set the increment value with 1
for i in cipher:
    a = ord(i) + j # everytime increment the alphabet with the increment variable
    if i.isupper():
        if a > 90: # if the upper character cross the ascii value 90
            a = 64 + a-90 # then repeat from the first character
    else:
        if a > 122: # if the lower character cross the ascii value 122
            a = 96 + a-122 # then repeat from the first character
    j += 1 # always increase the increment variable
    plain += chr(a) 

print(plain)

# after running the program you get the output like this
# outupt: flagY6uG9TMeHAHD
# just put the curly brace as the position in cipher also replace the number with the cipher text number 6 replace with 0, 9 replace with 0 and the last character D replace with 4
# also don't forget to put the underscore in the plain text also like cipher text
```

### flag : flag{Y0uG0T_MeHAH4}
_Note:_ Don't copy it try yourself.