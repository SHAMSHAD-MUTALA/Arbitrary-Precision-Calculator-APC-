# 🧮 Arbitrary Precision Calculator (APC)

**Arbitrary Precision Calculator (APC)** is a powerful command-line calculator implemented in C that performs arithmetic operations (addition, subtraction, multiplication, division) on arbitrarily large integers using doubly linked lists.

## 📁 Project Structure

```
APC/
├── header.h              # Header file containing function declarations and macros
├── calculator.c          # Main calculator program
├── calculator.o          # Object file for the main calculator
├── add_func.c            # Source code for addition function
├── add_func.o            # Object file for addition function
├── sub_func.c            # Source code for subtraction function
├── sub_func.o            # Object file for subtraction function
├── mul_func.c            # Source code for multiplication function
├── mul_func.o            # Object file for multiplication function
├── div_func.c            # Source code for division function
├── div_func.o            # Object file for division function
├── inserting_func.c      # Source code for helper functions (e.g., inserting numbers)
├── inserting_func.o      # Object file for helper functions
├── makefile              # Makefile for building the project
└── result.exe            # Compiled executable (output)
```

## 🚀 Features

- ✨ Support for large number arithmetic beyond native data types
- ➕ Addition, ➖ Subtraction, ✖️ Multiplication, ➗ Division
- 🔄 Linked list-based implementation for flexible number storage
- 🧩 Modular design with clear separation of logic
- 🧼 Dynamic memory management with cleanup functions

## 🛠️ Build Instructions

### 🧾 Prerequisites

- GCC compiler
- `make` utility

### 🔧 To Build

```bash
cd APC/
make
```

This will compile all object files and generate the executable `result.exe`.

## 📌 Usage

```bash
./result.exe <number1> <operator> <number2>
```

### Example

```bash
./result.exe 987654321987654321 + 123456789123456789
Result is 1111111111111111110
```

### Supported Operators

| Operator | Description  |
|----------|--------------|
| `+`      | Addition      |
| `-`      | Subtraction   |
| `*`      | Multiplication|
| `/`      | Division      |

## 📦 Implementation Details

- Input numbers are stored as doubly linked lists (`struct node`).
- Each digit is stored in a separate node to allow operations on very large numbers.
- Custom functions handle parsing, processing, and printing results.
- Memory is carefully managed using `malloc()` and `free()`.

## 🧹 Clean Build Files

To remove object files and executable:

```bash
make clean
```

## 🤝 Contributing

1. Fork this repository
2. Create a new branch (`git checkout -b feature/feature-name`)
3. Commit your changes (`git commit -m "Add feature"`)
4. Push to the branch (`git push origin feature-name`)
5. Open a Pull Request

