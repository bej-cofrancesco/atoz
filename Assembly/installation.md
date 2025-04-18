# Assembly Installation Guide

## Required Software

- **Assembler**: Depends on target architecture
  - **x86/x64**: NASM, MASM, GAS (GNU Assembler)
  - **ARM**: GNU Assembler (as), ARMASM
  - **RISC-V**: GNU Assembler (as)
- **Linker**: Usually included with development tools (ld on Unix systems)
- **Debugger**: GDB or architecture-specific debugger

## File Extensions

- `.asm`, `.s` - Assembly source files
- `.o`, `.obj` - Object files
- `.lst` - Listing files (with source and machine code)
- `.inc` - Include files with macros or constants
- `.exe`, `.out`, `.elf` - Executable output formats

## Package Management

```bash
# No standard package management for Assembly
# Typically manually include libraries or import system calls

# Example for building with NASM on Linux (x86_64)
nasm -f elf64 -o file.o file.asm
ld -o program file.o

# Example for building with NASM on Windows (x64)
nasm -f win64 -o file.obj file.asm
link file.obj /subsystem:console /entry:main

# Example for building with GAS (GNU Assembler)
as -o file.o file.s
ld -o program file.o
```

## Running Assembly Programs

```bash
# Run compiled executable on Linux
./program

# Run compiled executable on Windows
program.exe

# Debug with GDB
gdb ./program

# Run with arguments
./program arg1 arg2
```

## Common Libraries

- **Assembly typically doesn't use libraries in the traditional sense**
- **System libraries**: Called through system calls
- **C standard library**: Can be linked against for some functionality
- **BIOS/UEFI routines**: For low-level hardware access
- **CPU-specific instruction sets**: SSE, AVX, NEON, etc.
