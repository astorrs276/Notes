### Format Specifiers
**Common**
`%d`/`%i` - integer (2 or 4 bytes)
`%ld` - long integer (4 bytes)
`%f` - float (4 bytes)
`%lf` - double (8 bytes)
`%c` - character (1 byte)
`%s` - string (character array)
`%p` - memory address (for printing)

**Less Common**
`%u` - unsigned integer (2 or 4 bytes)
`%hhu` - unsigned character (1 byte)
`%hd` - short integer (2 bytes)
`%lld` - long long integer (8 bytes)
`%Lf` - long double (12 bytes)
### Other
`&` (as unary operator) - "memory address that the variable begins at" (ex: `&x`)
`&` (as binary operator) - bitwise AND (ex: `x & y`)
`|` - bitwise OR
`^` - bitwise XOR
`~` - bitwise complement
`<<` - shift left (pad right with 0s)
`>>` - shift right (pad left with 0s)
