# libft

`libft` is a foundational project in the 42 Network curriculum that involves creating a custom C library. This library replicates and extends some of the most commonly used standard C library functions, as well as includes additional utilities for string manipulation, memory handling, and linked list management.

---

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Installation](#installation)
- [Implementation Details](#implementation-details)
- [Learning Outcomes](#learning-outcomes)
- [Credits](#credits)

---

## Introduction
The `libft` project aims to:
- Reinforce understanding of essential C programming concepts.
- Build reusable and modular code.
- Serve as a foundation for future projects like `ft_printf` and `get_next_line`.

This library is coded from scratch, adhering to the 42 Network's rigorous coding standards.

---

## Features

### Core Functions:
`libft` implements many standard C library functions, including:

| Category            | Functions                                     |
|---------------------|----------------------------------------------|
| **String Handling** | `ft_strlen`, `ft_strcpy`, `ft_strdup`, `ft_strjoin` |
| **Memory Handling** | `ft_memset`, `ft_memcpy`, `ft_memmove`, `ft_calloc` |
| **Character Checks**| `ft_isalpha`, `ft_isdigit`, `ft_tolower`, `ft_toupper` |

### Bonus Features:
If the bonus part is implemented, `libft` also includes functions to manipulate linked lists:

| Function              | Description                                  |
|-----------------------|----------------------------------------------|
| `ft_lstnew`           | Creates a new list node                     |
| `ft_lstadd_front`     | Adds a node at the beginning of the list    |
| `ft_lstiter`          | Iterates over the list and applies a function |
| `ft_lstmap`           | Maps a function to each node and returns a new list |

---

## Usage

Include `libft.h` in your project and link the compiled library.

### Example:
```c
#include "libft.h"

int main(void)
{
    char *str = ft_strdup("Hello, libft!");
    ft_putstr_fd(str, 1);
    free(str);
    return 0;
}
```

### Output:
```
Hello, libft!
```

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/libft.git
   cd libft
   ```

2. Compile the library:
   ```bash
   make
   ```

3. Include `libft.h` and link the library when compiling your project:
   ```bash
   gcc -o main main.c libft.a
   ```

---

## Implementation Details

### Key Concepts:
- **String Manipulation:**
  Functions to copy, concatenate, and manipulate strings efficiently.

- **Memory Management:**
  Utilities for handling memory allocation and copying.

- **Linked Lists:**
  Optional functions to manage singly linked lists for dynamic data storage.

---

## Learning Outcomes

Through this project, I:
- Strengthened my understanding of low-level C programming.
- Learned to write modular and reusable code.
- Gained experience with memory management and debugging.

---

## Credits

Project completed as part of the 42 Network curriculum.

---

