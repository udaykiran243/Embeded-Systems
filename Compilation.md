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
  ```
  







