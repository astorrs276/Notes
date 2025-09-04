### Bitwise Data
Unsigned chars hold a single byte of data (0 to 255)
Best to think of it as a series of 8 bits ordered left to right (01000001 rather than the int 65 or the char 'A')
Logical operations - AND, OR, XOR, shifts, etc.
### Pointers
Variables get space allocated in order of declaration
After allocation, address is needed to access - name doesn't exist after compilation
Within a variable
- Lowest address is the first byte of the variable
- Highest address is the last byte
- Byte with the lowest address contains the least significant information
Data is written from the low address to the high address
A pointer is NOT a memory address, it is a variable that can store a memory address
Most commonly used for run-time allocation of memory - don't have to be used for this
Needed to share memory addresses between between functions