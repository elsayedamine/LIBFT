# 📚 Libft — Custom C Library

## 📖 Overview

**Libft** is my foundational C library project from the 42 curriculum. It recreates and extends many standard C library functions, while also adding custom utility functions to streamline C programming in future projects.

The library serves as a reusable toolkit of safe, efficient, and well-tested functions — from string manipulation and memory management to linked list handling and I/O utilities.

---

## ⚙️ Core Library Features (Base)

The base folder implements all the mandatory Libft functions, including:

- Character checks and conversions (`ft_isalpha`, `ft_isdigit`, `ft_tolower`, etc.)  
- String operations (`ft_strlen`, `ft_strchr`, `ft_strdup`, `ft_strncmp`, `ft_strtrim`, etc.)  
- Memory manipulation (`ft_memset`, `ft_memcpy`, `ft_memmove`, etc.)  
- Conversion and output (`ft_atoi`, `ft_itoa`, `ft_putchar_fd`, `ft_putstr_fd`, etc.)  
- Linked list standard operations (`ft_lstnew`, `ft_lstadd_front`, `ft_lstlast`, `ft_lstsize`, etc.)  

All functions were built from scratch following the 42 norms and tested thoroughly.

---

## 🚀 Additional Custom Features

Beyond the base Libft requirements, I implemented a suite of custom utilities to improve productivity and cover common programming needs:

- **Advanced linked list utilities** like `ft_lstdup`, `ft_lstpop`, `ft_lstinsert`, `ft_lstndup`, `ft_lstgetnode`, `ft_lst2str`, `ft_list2arr` and more  
- **String and array helpers** such as `ft_strchr_index`, `ft_stristr`, `ft_strextract`, `ft_strinsert`, `ft_strndup`, `ft_arr2str`, `ft_arrdup`, `ft_arrlen`  
- **Memory management helpers** like `ft_malloc`, `ft_free`, and `int_free` for safer dynamic allocations  
- **I/O and printf enhancements** housed in the `2.printfd/` folder, including `ft_printf` and support for printing numbers and pointers to file descriptors  
- **Get Next Line** implementation for reading lines from file descriptors efficiently  
- **Whitespace handling** with functions like `ft_isspace` and `ft_iswhitespace`  
- Utility functions for swapping values (`ft_swap`), counting characters (`ft_count_char`), and inserting characters into strings (`ft_insert_char`)  
- Extensive list management (`lst_addback`, `lst_addfront`, `lst_clear`, `lst_new`, `lst_last`, `lst_size`) with robust, reusable code

---

## 🧰 Project Structure
```
libft/
├── 1.base/ # Base Libft mandatory functions
├── 2.printfd/ # Custom printf and fd output utilities
├── 3.get_next_line/ # Get Next Line implementation
├── new/ # Custom added functions and helpers
└── README.md # This documentation
```

---

## 🧪 Testing & Usage

- All functions adhere strictly to 42 coding norms  
- Extensively tested with unit tests and integrated into subsequent 42 projects  
- Designed to be modular and easy to include in any C project by linking `libft.a`  
- Usage example:

```c
#include "libft.h"

int main(void)
{
    char *s = ft_strdup("Hello, Libft!");
    if (!s)
        return (1);
    ft_putendl_fd(s, 1);
    free(s);
    return (0);
}
```

---

## 💡 What I Learned
Implementing low-level C functions from scratch deepened my understanding of pointers, memory management, and string operations

Designing reusable and modular code that complies with strict coding standards

Handling edge cases and writing robust error checking

Expanding standard libraries with practical utilities to simplify future projects

Mastering linked list manipulations and file descriptor operations

## ✍️ Author
Amine Elsayed
- 42 Network Student | Systems programming enthusiast
  
> _“Writing your own library is the first step toward mastering C.”_
