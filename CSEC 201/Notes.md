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
Pointers are variables that store memory addresses
All pointers should be initialized to `NULL` regardless of datatype
- If you don't, it might get whatever data is in the memory address allocated for the variable, even if it isn't assigned yet
Pointer size is based on system architecture (4 bytes for 32-bit system)
"Referencing" - use the address of a variable using `&` to get the address of a variable (ex: `scanf("%d", &x)`, `printf("%p", &x)`)
"Dereferencing" - use an address of a variable to fetch the data using `*` (ex:`printf("%d", *&x)`)
- `*` negates `&`
### Arrays
Arrays are created at compile time and cannot use runtime data for sizing
`<DataType> <name>[size]`
`[]` are operators for finding the address of an element from the base index of the array
- Done by multiplying the size of the data type by the index
	- int x\[3];
	- x\[0] = 1a2b3c2f + (4 * 0) = 1a2b3c2f
	- x\[1] = 1a2b3c2f + (4 * 1) = 1a2b3c33
	- x\[2] = 1a2b3c2f + (4 * 2) = 1a2b3c37
### Functions
Function names are identifiers, just like variable names
If you try to use a function before it is defined, it won't be recognized - very common error: <u>Unresolved External Symbol</u>
Good practice is to split code into a lot of different files based on what they do
A function's stack frame is how much RAM is allocated to it
- Its size might fluctuate over the course of execution
- Includes local variables, parameters, calculations, <u>control information</u> (return to where the function was called from), etc.
- Organized from high to low addresses (high used earlier than low)
- RAM is reallocated after the function finishes
