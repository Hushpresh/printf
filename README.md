Write a function that produces output according to a format.
Prototype: int _printf(const char *format, ...);
Returns: the number of characters printed (excluding the null byte used to end output to strings). Write output to stdout, the standard output streamformat is a character string. The format string is composed of zero or more directives. See man 3 printf for more detail. 
You need to handle the following conversion specifiers: c and s %
Handle the following custom conversion specifiers: b: the unsigned int argument is converted to binaryHandle the following conversion specifiers: d and i
Handle the following conversion specifiers: u, o, x and X
Use a local buffer of 1024 chars in order to call write as little as possible.
Handle the following custom conversion specifier: S : prints the string.
Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: \x, followed by the ASCII code value in hexadecimal (upper case - always 2 characters)
Handle the following conversion specifier: p.
Handle the following flag characters for non-custom conversion specifiers: +, space and #
Handle the following length modifiers for non-custom conversion specifiers: l and h, Conversion specifiers to handle: d, i, u, o, x, X
Handle the field width for non-custom conversion specifiers.
Handle the precision for non-custom conversion specifiers.
Handle the 0 flag character for non-custom conversion specifiers.
Handle the - flag character for non-custom conversion specifiers.
Handle the following custom conversion specifier: R: prints the rot13'ed string
All the above options work well together.
