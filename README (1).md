# 📚 ft_printf  

`ft_printf` is a custom C library that replicates the functionality of the standard `printf` function in C. It supports a wide range of format specifiers and is optimized to handle various types of data efficiently. This project is an essential tool for any C developer looking to work with formatted output.

## 🛠 Features  

`ft_printf` implements the following format specifiers:

- **`%c`**: Prints a single character.
- **`%s`**: Prints a string (as defined by the common C convention).
- **`%p`**: Prints a `void *` pointer argument in hexadecimal format.
- **`%d`**: Prints a signed decimal (base 10) number.
- **`%i`**: Prints an integer in base 10.
- **`%u`**: Prints an unsigned decimal (base 10) number.
- **`%x`**: Prints a number in lowercase hexadecimal (base 16) format.
- **`%X`**: Prints a number in uppercase hexadecimal (base 16) format.
- **`%%`**: Prints a percent sign (`%`).

### Core Functions  
- **Formatted Output**: Implements a custom `printf` function for formatted printing.  
- **Character Printing**: Functions to print characters, strings, and numbers in different formats.  
- **Memory Management**: Efficient memory handling using custom utility functions for buffer manipulation.  

### Advanced Modules  
- **Parser**: Parses the format string to identify the types and formatting for output.  
- **Print Integer and Pointer**: Specialized functions to handle printing unsigned integers (`ft_put_uint`), pointers (`ft_putptr`), and more.  

## 🚀 Installation  

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/ft_printf.git
   cd ft_printf
2. Compile the library using the Makefile:
    ```bash
    make
This will generate the libftprintf.a file, which can be linked to your projects.

## 📂 Directory Structure
    .
    ├── Makefile                # Build and cleaning rules
    ├── ft_printf.h             # Header file with function declarations
    ├── src/                    # Source files for the main logic
    │   ├── ft_parser.c         # Parses the format string for printf
    │   ├── ft_printf.c         # Main implementation of the printf function
    │   ├── ft_put_uint.c       # Prints unsigned integers
    │   └── ft_putptr.c         # Prints pointers
    └── utils/                  # Utility functions for printing
        ├── ft_putchar.c        # Prints a single character
        ├── ft_putnbr_base.c    # Prints integers in a specific base
        ├── ft_putstr.c         # Prints a string
        └── ft_strlen.c         # Returns the length of a string

## 🧩 Usage
To use the library in your project, include ft_printf.h in your source code and link the compiled libftprintf.a during compilation:

    gcc -Wall -Wextra -Werror main.c -L. -lftprintf -o my_program
