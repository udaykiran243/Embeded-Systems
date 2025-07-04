# Compilation Stages
Compilation stages are the steps of implementing the compilation of the program where the program creates a executable file. The compilation of a C program involves a series of stages, transforming human-readable source code into an executable file. These stages are:
- **Preprocessing Stage**
- **Compilation Stage**
- **Assembler Stage**
- **linker Stage**

## Preprocessing Stage
- This is the first stage where the preprocessor handles directives indicated by # (e.g., #include, #define, #ifdef). Comments are removed.
- Macros defined with #define are expanded and replaced with their corresponding values.
- Header files specified with #include are incorporated into the source code, effectively pasting their contents.
- Conditional compilation directives (like #ifdef) are evaluated to include or exclude specific blocks of code.
- The output is a preprocessed source file, typically with a ```.i``` extension.
- We use some commands to get or to stop the process of compilation in the middle.
  
  ```command
  gcc -E FileName.c
  ```

- It constists of the **PREPROCESSER DIRECTIVES** in the file that is created after the preprocesser stage.
- **Preprocesser Directives** : Preprocessor directives in C programming are special commands that begin with a hash symbol (#) and are processed by the C preprocessor before the actual compilation phase. They provide instructions to the preprocessor to modify the source code, include files, define macros, or control conditional compilation.
  ```c
    #include #define #line #pragma #error #endif #undef
  ```

## Compilation Stage
- The preprocessed source code is then fed to the compiler.
- The compiler translates the C code into assembly language specific to the target architecture.
- This stage also involves syntax checking and semantic analysis.
- The output is an assembly file, usually with a .s extension.
- We use the following command to get the ```.s``` file or to stop the process of compilation at the compilation stage

  ```command
  gcc -S FileName.c
  ```

- It consists of the **ASSEMBLY CODE** where for every instruction their will be a corresponding assembly code.

## Assembly Stage
- The assembler takes the assembly code generated in the previous stage as input.
- It translates the assembly instructions into machine code (binary instructions) that the computer's processor can directly understand.
- The output is an object file, typically with a ```.o``` (on Unix-like systems) or ```.obj``` (on Windows) extension. This file contains machine code but is not yet executable as it may have unresolved references to functions or data in other files or libraries.
- For Creating a object code we use the command
  
  ```command
  gcc -c FileName.c
  ```
  
- The object code consists of the instructions in the binary format.
- To display or to see the object code we need to use the special tools they are **objdump** and **readELF ( Executable File Format )**.
  
  ```command
  objdump FileName.o
  ```

- To display the instructions and their corresponding Assembly code we use the ```-S```.

  ```command
  objdump -S FileName.o
  ```
- During the compilation we use the following commands

  ```command
  gcc -S FileName.c
  ```

## Linker Stage
- The final stage is linking, performed by the linker.
- The linker combines one or more object files and necessary library files (e.g., standard C library functions like printf).
- It resolves all external references, ensuring that calls to functions defined in other object files or libraries are correctly linked to their respective implementations.
- The result of the linking stage is the final executable file, which can be run directly by the operating system.
- It combines all the ```.o``` object files to create one executable file ```a.out```.
- To Combine N no.of ```.c``` files and get one executable file we use the following command

  ```command
  gcc FileName1.c FileName2.c FileName3.c ...... FileNameN.c
  ```

- This will gives use the one executable file after compiling all the ```.c``` files.
- We can also include the FileName in one single program using the preprocessive directives ```#include "FileName.c```.





