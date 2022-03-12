### Explanation of stafck frames and frame pointer

- Function has local memory associate with to incomming params, local vars and temporary vars. This region of memory => **STACK FRAME**, allocated on process's stack

- **Frame pointer** (`ebp` for intel x86 and `rbp` for 64-bit arch) contains base address of the function frame   =>  Does not change throughout the function
- Code to access local vars within function generated in term of **offsets** to frame pointer
- **Stack pointer** (`ebp` for intel x86 and `rsp` for 64-bit arch): values are pushed(preparation to call another function)/popped off the stack => Chnage during exec function
