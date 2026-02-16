# get_next_line

## 📚 Project Overview
**get_next_line** is a C function that reads a line from a file descriptor, returning it as a string each time it is called. The goal of this project is to improve understanding of file I/O, dynamic memory allocation, and buffer management in C.

---

## 📌 Requirements
- Must be written in C.  
- Reads from a file descriptor one line at a time, including the newline character (`\n`) if it exists.  
- Returns `NULL` when there is nothing more to read or in case of an error.  
- Proper handling of memory to avoid leaks.  
- Uses a buffer size defined by `BUFFER_SIZE` during compilation.  

---

## ⚙️ Features
- Reads from any valid file descriptor (files, standard input, etc.).  
- Handles lines of arbitrary length.  
- Returns a newly allocated string each call; the caller is responsible for freeing it.  
- Supports multiple calls in sequence to read a file line by line.  

---

## 🛠 Installation
1. Clone the repository:
```bash
git clone eng-juliet/get_next_line
cd get_next_line
```

2. Build the library using the Makefile:
```bash
make
```

3. Optional cleanup:
```bash
make clean   # Removes object files
make fclean  # Removes object files and libft.a
```
4. Link the library in your C programs:
```bash
gcc your_program.c -L. -lft
```

## 📝 Author
**Juliet Haddadin** – 2024
