# Libft

This project was completed as part of the curriculum at École 42. The goal of the project is to create a library of useful functions that can be used in future projects.

## Installation

To use the libft library, follow these steps:

1. Clone the repository to your local machine.
2. Open a terminal window and navigate to the root directory of the project.
3. Run the command `make` to compile the library.
4. Include the header file `libft.h` in your project.
5. Link the library during compilation using the `-L` and `-l` flags.

```bash
gcc -o my_program my_program.c -L/path/to/libft -lft
```
## Usage
The libft library provides a wide range of functions that can be used for string manipulation, memory management, character checks, linked lists, and more. The functions are prefixed with the ft_ abbreviation.

To use a specific function, include the corresponding header file and call the function in your code. Here's a new example that demonstrates the use of different functions:
```c
#include "libft.h"

int main(void) {
    char src[] = "Hello,";
    char dest[20];
    
    ft_strcpy(dest, src);
    printf("Copied string: \"%s\"\n", dest);
    
    char str[] = "Hello, world!";
    int length = ft_strlen(str);
    printf("Length of string: %d\n", length);

    int is_alpha = ft_isalpha('A');
    printf("Is 'A' alphabetic? %d\n", is_alpha);
    
    int is_digit = ft_isdigit('9');
    printf("Is '9' a digit? %d\n", is_digit);
    
    return 0;
}
```
In this example, the program demonstrates the use of different functions. It copies a string using ft_strcpy, calculates the length of a string using ft_strlen, and checks if a character is alphabetic using ft_isalpha and if a character is a digit using ft_isdigit. The results are then printed to the console.

Make sure to compile your program with the libft library, as mentioned in the installation instructions.

## Documentation
For detailed documentation on all available functions in the libft library, refer to the libft.h header file. Each function is documented with its parameters, return value, and a brief description of its purpose.

## Credits
This project was completed by Thibault GIRAUDON (tgiraudo) as part of the curriculum at École 42.
