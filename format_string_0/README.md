# format_string_0

### Author: Cheng Zhang

### Description
Can you use your knowledge of format strings to make the customers happy?

### Solution

After connecting to the server we are prompted with the following

```
> nc mimas.picoctf.net 56191
Welcome to our newly-opened burger place Pico 'n Patty! Can you help the picky customers find their favorite burger?
Here comes the first customer Patrick who wants a giant bite.
Please choose from the following burgers: Breakf@st_Burger, Gr%114d_Cheese, Bac0n_D3luxe
Enter your recommendation:
```

Here the only string that has a format specifier is `Gr%114d_Cheese`

next we see

```
Good job! Patrick is happy! Now can you serve the second customer?
Sponge Bob wants something outrageous that would break the shop (better be served quick before the shop owner kicks you out!)
Please choose from the following burgers: Pe%to_Portobello, $outhwest_Burger, Cla%sic_Che%s%steak
Enter your recommendation:
```

Here the only string that has a format specifier is `Cla%sic_Che%s%steak`

inputting that returns us the flag

`picoCTF{7h3_cu570m3r_15_n3v3r_SEGFAULT_74f6c0e7}`