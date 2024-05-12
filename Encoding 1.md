# Encoding 1 Cybertalents Problem

__Problem Link:__ [Encoding 1](https://cybertalents.com/challenges/cryptography/encoding-1)
---

__Description:__ Decode this message: ZmxhZ3tiYXNlNjRfaXNfbjB0X3MzY3VyZX0=

### My Approach:

1. When I see that in the cipher, there is a equal(=) sign at the end of the sentnce.
2. Then definitely sure that it is a base64 cipher
3. Use the command in the `kali` terminal _echo "ZmxhZ3tiYXNlNjRfaXNfbjB0X3MzY3VyZX0=" | base64 -d_
4. Or, use the online [decoder](https://www.base64decode.org/) system and post the cipher.

### flag : ~~flag{base64_is_n0t_s3cure}~~
_Note:_ Don't copy it try yourself.