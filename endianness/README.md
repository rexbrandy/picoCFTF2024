##### Author
Nana Ama Atombo-Sackey

### Description
Know of little and big endian?

# Solution
In this challenge we are given the source code for a script that generates a random 5 character string and askes us to provide the big endian and little endian representations of this string.

```
> nc titan.picoctf.net 58276                                    
Welcome to the Endian CTF!
You need to find both the little endian and big endian representations of a word.
If you get both correct, you will receive the flag.
Word: hzxxv
```

To complete this challenge we need to convert the word `hzxxv` to hexadecimal `687A787876`

`687A787876` is the big endian representation of this string. `h`(hex `68`) is the most significant byte and `v`(hex `76`) being the least significant. `7678787A68` is the litle endian representation of this string. 

```
Enter the Little Endian representation: 7678787A68
Correct Little Endian representation!
Enter the Big Endian representation: 687A787876 
Correct Big Endian representation!
Congratulations! You found both endian representations correctly!
Your Flag is: picoCTF{3ndi4n_sw4p_su33ess_817b7cfe}
```