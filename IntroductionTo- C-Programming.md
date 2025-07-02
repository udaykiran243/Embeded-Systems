# **Introduction To C- Programming**
C is a powerful, general-purpose programming language developed by Dennis Ritchie in the early 1970s at Bell Labs. It is known for its speed, efficiency, and close-to-hardware capabilities, making it ideal for system programming, such as operating systems and embedded systems. C provides low-level memory access, a simple set of keywords, and a clean style, making it a popular choice for beginners and professionals alike. Its influence can be seen in many modern languages like C++, Java, and Python.
# **Basic Elements**
The Elements which are used for the programming in C or any other language these elements are used to write the code in the specific language which can be same in all the languages like C++, Java, etc,.. The following Elements are explained based on the C Programming language. The Following are the **Basic Elements** in C programming language.
  1. **Character Set** : Character Set are Used to write C programming and they are Divided into **Four** types.
  2. **Identifiers** : Identifiers are the names of the words that are *pre-determined | User-defined*
  3. **KeyWords** : Keywords are the predefined words which are called as library names.
  4. **Data Types** : Data Types are the Predefined keywords used to store the data in a specific format.
  5. **Constants** : Constants are the values or the integers used in the program.
  6. **Variable** : Names given to the *Memory Locations* or to store a value in the Memory.
  7. **Expression** : Expressions are the combination of variables, Operators, and Operands which can be used to do a task.
  8. **Statements** : A Statement is a set of expression or the set of task.

# 1.Character Set
Character Set are Used to write C programming and they are Divided into **Four** types. The Four Catagories in character set are as Follows:
## **Printable Character Set**
- **Alphabet** : Alphabets are the characters used in the Character Set which can be Both Lower and Upper Case [a-z = a-97, b-98, ...] [A-Z = A-65, B-66, ...]. These are having their Corresponding **ASCII(American Standard Code Information Interchange)** values.

| Dec | Char | Description            | Dec | Char | Description   | Dec | Char | Description   |
| --- | ---- | ---------------------- | --- | ---- | ------------- | --- | ---- | ------------- |
| 0   | NUL  | Null                   | 43  | +    | Plus          | 86  | V    | Uppercase V   |
| 1   | SOH  | Start of Header        | 44  | ,    | Comma         | 87  | W    | Uppercase W   |
| 2   | STX  | Start of Text          | 45  | -    | Hyphen        | 88  | X    | Uppercase X   |
| 3   | ETX  | End of Text            | 46  | .    | Period        | 89  | Y    | Uppercase Y   |
| 4   | EOT  | End of Transmission    | 47  | /    | Slash         | 90  | Z    | Uppercase Z   |
| 5   | ENQ  | Enquiry                | 48  | 0    | Digit 0       | 91  | \[   | Left bracket  |
| 6   | ACK  | Acknowledge            | 49  | 1    | Digit 1       | 92  | \\   | Backslash     |
| 7   | BEL  | Bell                   | 50  | 2    | Digit 2       | 93  | ]    | Right bracket |
| 8   | BS   | Backspace              | 51  | 3    | Digit 3       | 94  | ^    | Caret         |
| 9   | TAB  | Horizontal Tab         | 52  | 4    | Digit 4       | 95  | \_   | Underscore    |
| 10  | LF   | Line Feed (`\n`)       | 53  | 5    | Digit 5       | 96  | \`   | Grave accent  |
| 11  | VT   | Vertical Tab           | 54  | 6    | Digit 6       | 97  | a    | Lowercase a   |
| 12  | FF   | Form Feed              | 55  | 7    | Digit 7       | 98  | b    | Lowercase b   |
| 13  | CR   | Carriage Return (`\r`) | 56  | 8    | Digit 8       | 99  | c    | Lowercase c   |
| 14  | SO   | Shift Out              | 57  | 9    | Digit 9       | 100 | d    | Lowercase d   |
| 15  | SI   | Shift In               | 58  | :    | Colon         | 101 | e    | Lowercase e   |
| 16  | DLE  | Data Link Escape       | 59  | ;    | Semicolon     | 102 | f    | Lowercase f   |
| 17  | DC1  | Device Control 1       | 60  | <    | Less-than     | 103 | g    | Lowercase g   |
| 18  | DC2  | Device Control 2       | 61  | =    | Equal sign    | 104 | h    | Lowercase h   |
| 19  | DC3  | Device Control 3       | 62  | >    | Greater-than  | 105 | i    | Lowercase i   |
| 20  | DC4  | Device Control 4       | 63  | ?    | Question mark | 106 | j    | Lowercase j   |
| 21  | NAK  | Negative Acknowledge   | 64  | @    | At symbol     | 107 | k    | Lowercase k   |
| 22  | SYN  | Synchronous Idle       | 65  | A    | Uppercase A   | 108 | l    | Lowercase l   |
| 23  | ETB  | End of Trans. Block    | 66  | B    | Uppercase B   | 109 | m    | Lowercase m   |
| 24  | CAN  | Cancel                 | 67  | C    | Uppercase C   | 110 | n    | Lowercase n   |
| 25  | EM   | End of Medium          | 68  | D    | Uppercase D   | 111 | o    | Lowercase o   |
| 26  | SUB  | Substitute             | 69  | E    | Uppercase E   | 112 | p    | Lowercase p   |
| 27  | ESC  | Escape                 | 70  | F    | Uppercase F   | 113 | q    | Lowercase q   |
| 28  | FS   | File Separator         | 71  | G    | Uppercase G   | 114 | r    | Lowercase r   |
| 29  | GS   | Group Separator        | 72  | H    | Uppercase H   | 115 | s    | Lowercase s   |
| 30  | RS   | Record Separator       | 73  | I    | Uppercase I   | 116 | t    | Lowercase t   |
| 31  | US   | Unit Separator         | 74  | J    | Uppercase J   | 117 | u    | Lowercase u   |
| 32  | ␣    | Space                  | 75  | K    | Uppercase K   | 118 | v    | Lowercase v   |
| 33  | !    | Exclamation mark       | 76  | L    | Uppercase L   | 119 | w    | Lowercase w   |
| 34  | "    | Double quote           | 77  | M    | Uppercase M   | 120 | x    | Lowercase x   |
| 35  | #    | Number sign            | 78  | N    | Uppercase N   | 121 | y    | Lowercase y   |
| 36  | \$   | Dollar sign            | 79  | O    | Uppercase O   | 122 | z    | Lowercase z   |
| 37  | %    | Percent sign           | 80  | P    | Uppercase P   | 123 | {    | Left brace    |
| 38  | &    | Ampersand              | 81  | Q    | Uppercase Q   | 124 | \|   | Vertical bar  |
| 39  | '    | Single quote           | 82  | R    | Uppercase R   | 125 | }    | Right brace   |
| 40  | (    | Left parenthesis       | 83  | S    | Uppercase S   | 126 | \~   | Tilde         |
| 41  | )    | Right parenthesis      | 84  | T    | Uppercase T   | 127 | DEL  | Delete        |
| 42  | \*   | Asterisk               | 85  | U    | Uppercase U   |     |      |               |

- **Numerics** : The integer values are the numbers are also called as Character set in which these Numerics are also having the corresponding **ASCII** values.

| Char | ASCII Decimal | Binary   | Hex  | Description |
| ---- | ------------- | -------- | ---- | ----------- |
| 0    | 48            | 00110000 | 0x30 | Digit 0     |
| 1    | 49            | 00110001 | 0x31 | Digit 1     |
| 2    | 50            | 00110010 | 0x32 | Digit 2     |
| 3    | 51            | 00110011 | 0x33 | Digit 3     |
| 4    | 52            | 00110100 | 0x34 | Digit 4     |
| 5    | 53            | 00110101 | 0x35 | Digit 5     |
| 6    | 54            | 00110110 | 0x36 | Digit 6     |
| 7    | 55            | 00110111 | 0x37 | Digit 7     |
| 8    | 56            | 00111000 | 0x38 | Digit 8     |
| 9    | 57            | 00111001 | 0x39 | Digit 9     |

- **Special Symbols** : The Special Characters are the characters which can be used for the Character set. These Special Symbols are also having the corresponding ASCII values.

| Char | ASCII | Description       | Char | ASCII | Description          |
| ---- | ----- | ----------------- | ---- | ----- | -------------------- |
| !    | 33    | Exclamation mark  | :    | 58    | Colon                |
| "    | 34    | Double quote      | ;    | 59    | Semicolon            |
| #    | 35    | Number sign       | <    | 60    | Less-than sign       |
| \$   | 36    | Dollar sign       | =    | 61    | Equal sign           |
| %    | 37    | Percent sign      | >    | 62    | Greater-than sign    |
| &    | 38    | Ampersand         | ?    | 63    | Question mark        |
| '    | 39    | Single quote      | @    | 64    | At symbol            |
| (    | 40    | Left parenthesis  | \[   | 91    | Left square bracket  |
| )    | 41    | Right parenthesis | \\   | 92    | Backslash            |
| \*   | 42    | Asterisk          | ]    | 93    | Right square bracket |
| +    | 43    | Plus sign         | ^    | 94    | Caret                |
| ,    | 44    | Comma             | \_   | 95    | Underscore           |
| -    | 45    | Hyphen or minus   | \`   | 96    | Grave accent         |
| .    | 46    | Period or dot     | {    | 123   | Left curly brace     |
| /    | 47    | Slash or divide   | \|   | 124   | Vertical bar (pipe)  |
|      |       |                   | }    | 125   | Right curly brace    |
|      |       |                   | \~   | 126   | Tilde                |

  
## **Non-Printable Character Set**
These are the Non printable charaters which will be used only for the **Cursor** Changes.
- **Escape Sequence** : These are the Combination of Alphabet and Numberics. They are mainly **six** Escape Sequence Characters. These are not treated as two characters, they are treated as single character. Most of the escape sequence are used in *printf()*. Escape Sequences are used to cgange or alter the position of the cursor they are non printable characters.
  - ``` \n ``` : Used for the Cursor to move to the Next Line ( Line Feed ).
  - ``` \r ``` : Used to Shift the Cursor from the Starting Position of the same line (replace) ( Carrage return ).
  - ``` \b ``` : Used to move Cursor *one position back* or *Back Space*.
  - ``` \t ``` : Used to get a *Tab Space* or Four spaces and start the cursor after the Tab space.
  - ``` \a ``` : Used for the *Alert* Sound when the Cursor reaches to this Escape Sequence.
  - ``` \0 ``` : Used for the *String Termination*.

| Escape Seq | Meaning             | ASCII Value | ASCII Name        |
| ---------- | ------------------- | ----------- | ----------------- |
| `\n`       | New line            | 10          | LF (Line Feed)    |
| `\r`       | Carriage return     | 13          | CR (Carriage Ret) |
| `\t`       | Horizontal tab      | 9           | TAB               |
| `\v`       | Vertical tab        | 11          | VT (Vertical Tab) |
| `\b`       | Backspace           | 8           | BS (Backspace)    |
| `\f`       | Form feed           | 12          | FF (Form Feed)    |
| `\a`       | Alert / Bell        | 7           | BEL (Bell)        |
| `\\`       | Backslash (`\`)     | 92          | Backslash         |
| `\'`       | Single quote (`'`)  | 39          | Apostrophe        |
| `\"`       | Double quote (`"`)  | 34          | Quote             |
| `\?`       | Question mark (`?`) | 63          | Question mark     |
| `\0`       | Null character      | 0           | NUL (Null)        |

# 2.Identifiers
In C programming, identifiers are the names used to represent various program elements such as variables, functions, arrays, structures, and more. They are created by the programmer to make the code readable and meaningful. An identifier must begin with a letter ```(A–Z or a–z)``` or an underscore (_) and can be followed by letters, digits ```0–9```, or underscores. Identifiers are case-sensitive, meaning total and Total are treated as different names. However, they cannot be the same as C keywords like ```int```, ```return```, or ```while```. Choosing clear and descriptive identifiers is essential for writing clean and maintainable code.
The Identifiers are the user defined words. These are having two different types
- Predefined words.
- User Defined words.

```c
int val; // int : predefined word, val : User defined word
```
## Rules for naming an identifier 
- Identifier names can contain alphabets, numerics only one special symbol. ```( _ )```
- Identifier names can start with alphabets or underscore ( _ ) but cannot start with numeric.
- Identifier names should not use keywords ( 32 keywords).
- The C programming is a case sensitive language.
- The Identidier name can be of any length, but the compiler will recognise only first 31 bits in 32 bit compiler, 15 bits in 16 bit compiler.
- blank spaces are not allowed in the naming of Identifier.

# 3.Keywords
In C programming, keywords are reserved words that have predefined meanings and purposes within the language. They are used to perform various operations such as defining data types ```(int, float, char)```, controlling program flow ```(if, else, while, for)```, and handling structures and functions ```(struct, return, void)```. Since these keywords are an integral part of the language syntax, they cannot be used as identifiers like variable or function names. All keywords are written in lowercase and serve specific roles that help the compiler understand and execute the program correctly. C has a total of 32 keywords, and each plays a vital role in building the logic and structure of a program.


| Keyword  | Purpose                                 |
| -------- | --------------------------------------- |
| `int`    | Declares an integer variable            |
| `float`  | Declares a floating-point variable      |
| `char`   | Declares a character variable           |
| `if`     | Used for conditional statements         |
| `else`   | Defines alternate execution path        |
| `while`  | Used for loops                          |
| `for`    | Another looping control                 |
| `return` | Returns a value from a function         |
| `void`   | Specifies no return type for a function |

| Keyword    | Purpose                               |
| ---------- | ------------------------------------- |
| `break`    | Exits from a loop or switch           |
| `continue` | Skips the current iteration in a loop |
| `switch`   | Multi-way branch                      |
| `case`     | Used inside a switch                  |
| `default`  | Fallback case in a switch             |
| `struct`   | Declares a structure                  |
| `typedef`  | Creates a new name for a data type    |
| `const`    | Declares constants                    |
| `sizeof`   | Returns the size of a data type       |

| Keywords   | Keywords   | Keywords   | Keywords |
| ---------- | ---------- | ---------- | -------- |
| `auto`     | `break`    | `case`     | `char`   |
| `const`    | `continue` | `default`  | `do`     |
| `double`   | `else`     | `enum`     | `extern` |
| `float`    | `for`      | `goto`     | `if`     |
| `int`      | `long`     | `register` | `return` |
| `short`    | `signed`   | `sizeof`   | `static` |
| `struct`   | `switch`   | `typedef`  | `union`  |
| `unsigned` | `void`     | `volatile` | `while`  |

# 4. Data Types
In C programming, data types define the type of data a variable can hold. They help the compiler allocate appropriate memory and perform valid operations on the data. The basic data types in C are categorized into primary (or fundamental), derived, and user-defined types. The fundamental types include ```int``` for integers, ```float``` for single-precision floating-point numbers, ```double``` for double-precision floating-point numbers, char for characters, and void for representing no value. Derived types include ```arrays```, ```pointers```, functions, and structures, while user-defined types can be created using ```struct```, ```union```, ```enum```, and ```typedef```. Each data type has a specific size and range, which may vary depending on the system architecture. Choosing the correct data type is important for efficient memory usage and accurate results in a program. The datatype tell us that how many bytes are corresponding variable occupies and What type of data is stored in the corresponding variable. The functions ```printf()``` uses format specifiers to get type and the size of the data ```% + conversion specification character```. We can store integer values in a character variable but with in the specific range which are called as **Sign Qualifier**.
The Data types are divided into two different types 

- Primitive DataTypes : ```int```, ```char```,```short```,```float```, etc,...
- Non-Primitive DataTypes : ```Arrays```,```Structures```,```Unions```.

## **1. Basic (Primary) Data Types**

| Data Type | Description                                     | Example             |
| --------- | ----------------------------------------------- | ------------------- |
| `int`     | Stores integers                                 | `int a = 10;`       |
| `float`   | Stores decimal numbers (single precision)       | `float b = 3.14;`   |
| `double`  | Stores decimal numbers (double precision)       | `double c = 5.678;` |
| `char`    | Stores single characters                        | `char ch = 'A';`    |
| `void`    | Represents absence of value (used in functions) | `void show();`      |

## **2. Derived Data Types**

| Type       | Description                             |
| ---------- | --------------------------------------- |
| Arrays     | Collection of elements of the same type |
| Pointers   | Store address of another variable       |
| Functions  | Block of code that performs a task      |
| References | (Not in C, only in C++)                 |

## **3. User-defined Data Types**

| Keyword   | Description                                |
| --------- | ------------------------------------------ |
| `struct`  | Groups variables of different data types   |
| `union`   | Similar to struct but shares memory        |
| `enum`    | Used to assign names to integral constants |
| `typedef` | Creates alias for data types               |


## Memory Segments or Memory Sections

```c
int y = 25;
int x;
int main(){
  int z;
}
```

| Memory Segments Before compilation    | Discription                                                   |
|---------------------------------------|---------------------------------------------------------------|
|```BSS(Block Started after Symbols)``` | Stores the Global varibles which are un-initialized ```x```   |
| ```Data Segment```                    | Stores the **Global Variables which are initialized ```y```   |
|```Text / code Segment```              | Stores the Instructions                                       |

- These segments are created before the time of **Execution**.
- These Segments are Stored in the HardDisc where then send to the **RAM** for execution.
- Assigning values during declaration is called initialization.
- The memeory for the global initialized variables are present in BSS segment.
- We cannot ise text editor to view contents of executable file we can use the **Objdump** and **readELF**.
- During execution the program gets loaded to HardDisc to RAM.
- After loading, few more additional segments are created , they are called **STACK** and **HEAP**.
- When a function is called / initialized a block of memory is created called **Stack Frame**.
- Stack and Heap are not fixed in size where stack grows Downwards(```↓```), and the Heap grows Upwards(```↑```).
- Text, Data and BSS segments are fixed, they cannot change during execution.
- Stack and Heap are created only when the program is loaded to RAM for execution.
- Except text segment all other segments are read and write segments.
- A block of area of created when a new thread is created and when the function is called stack frame is created.
- The command Line Arguments are stored above the stack.
- The Additional information given during execution of the program are called Command Line Arguments.

  |    **Memory Segments**   | 
  |--------------------------|
  |**Command Line Arguments**|
  |**Stack Frames / Stack**  |
  |         **Heap**         |
  |         **BSS**          |
  |     **Data Segments**    |
  |  **Text/Code Segment**   |

  - The process of Before Compilation Memory Segment is called **PROGRAM** and the loading of data for execution is called **PROCESS**.
  - To know or to see the process that are doing inside the system we use the following commands.
  These commands are for the use of CLI tools.
  ```
  ps -ef
  or
  top
  ```
  These commands are for the use of GUI tools. This is a application in the GUI which can be inside the OS and can be 
  ```
  system moniter
  ```
  # Difference Between ps and top Commands
    | Feature                   | `ps` (Process Status)                                  | `top` (Table of Processes)                           |
    | ------------------------- | ------------------------------------------------------ | ---------------------------------------------------- |
    | **Type**                  | Snapshot (one-time output)                             | Real-time, continuously updating                     |
    | **Interactivity**         | Non-interactive                                        | Interactive (supports key commands during execution) |
    | **Output**                | Static list of processes                               | Dynamic dashboard of processes                       |
    | **Best Use Case**         | Scripting, logging, quick checks                       | Live system monitoring                               |
    | **CPU/Memory Info**       | Shown (with options like `ps aux`)                     | Shown and auto-updated in real time                  |
    | **Resource Usage**        | Very low                                               | Moderate (due to live updates)                       |
    | **Filtering/Sorting**     | Via command-line options (e.g., `ps aux --sort=-%mem`) | Interactive (e.g., press `M` to sort by memory)      |
    | **Custom Output**         | Highly customizable with options and flags             | Limited customization via keystrokes                 |
    | **User-Friendliness**     | Medium (requires options for full info)                | Higher (but output can be overwhelming)              |
    | **Scripting Suitability** | Excellent                                              | Poor (due to real-time output)                       |

## Integer Types
The Integer are the values of numerics and floating point values which can be stored in a variable. The Integer values are the numerics from ```0,1,2,3,4,5,6,7,8,9,....``` the integer types are basically divided into **Two** types and they are as follows
- Numerics 
- Floating Points
## **Numerics**
 Numerics refer to the values that can be stored in variables such as 0, 1, 2, .... These values are used in various number systems in computing. They are mainly divided into three types:
  - **Decimal values** (`0-9`)
    These are the standard numbers we use in everyday life. The decimal system is base-10 and uses digits from 0 to 9.
    Example: 5, 123, 999.
  - **Binary Values** (`0` and `1`)
    Binary numbers use only 0s and 1s. This format is essential in machine-level operations, as it's the language computers understand.
    Example: 1010 (binary for 10), 1101.
⚙️ Note: You can prefix binary values with 0b in some programming languages (e.g., 0b1010).
  - **Hexadecimal values** (prefix - `0x`)
    Hexadecimal (or hex) is base-16 and uses digits 0–9 and letters A–F. Commonly used in memory addresses and color codes.
    Example: 0x1A3F (hex) equals 6719 in decimal.
  - **Octa values** (prefix - `0`)
    Octal numbers use base-8 and digits from 0 to 7. Often used in Unix file permissions and low-level programming.
    Example: 075 (octal), which equals 61 in decimal.
    
## **Floating points**
  Floating point numbers are numbers that have a decimal point. They are used to represent real numbers, including both very large and very small values, with fractional parts. To represent larger floating point values into short we use Exponential Notations.
  
  | Notation Type            | Description                                                                  | Example                                                 |
  | ------------------------ | ---------------------------------------------------------------------------- | ------------------------------------------------------- |
  | **Normal Notation**      | Standard decimal format with digits before and after the decimal point       | `123.456`, `0.01`                                       |
  | **Exponential Notation** | Scientific format used to represent very large/small numbers as powers of 10 | `1.23456e2` (i.e., `123.456`), `1.0e-3` (i.e., `0.001`) |

  **Example of Conversion Table**
  | Value       | Normal Notation | Exponential Notation |
  | ----------- | --------------- | -------------------- |
  | `123.0`     | `123.0`         | `1.23e2`             |
  | `0.00056`   | `0.00056`       | `5.6e-4`             |
  | `1000000.0` | `1000000.0`     | `1.0e6`              |
  | `-0.025`    | `-0.025`        | `-2.5e-2`            |

  # Standard Input/Output Library Functions
  These functions are used in the program which are predefined in C, These functions are declaration is present in the Header files and the functions defination is not present in the header file.
  **scanf()** : The scanf() takes two arguments one is **Format Specifier** and the other is **base address** of the memory where we want to store the data.

  `scanf( " %d ", & val );` : **""** - is the control string , **%d** - Format Specifier, **&val** - base address of the memory.

  - scanf() is a C Input/Output standard function.
  - it is the moment of the data from input device to the system memory ( **RAM** ).
  - If we are not using the `&` we get an **Segmentation Fault** | Runtime Error.
  - According to coding Guide lines the function definations should not present in header files.
  - The function definations are present in the library file **`libc.so`** `so` standards for **Shared Object**.
  - Scanf() block the execution until user provides the input and hit enter.
  - scanf() is a blocking call or it is a blocking function.
  - The input is stored ar the base address passed as 2nd argument to scanf().

## Printing integer values

### Decimal
The decimal values are one of the integer types of values which stores the values in decimal and these values starts from `0, 1, 2, 3, 4, ....` . To print these values we use the format specifiers as `%d`. To get the Decimal integer values we use the `%d` format in `scanf()`. 
```c
int val;
scanf("%d", &val); // input: 32
printf("%d", val); // prints the decimal value 32
```

### HexaDecimal
The Hexadecimal values are one of the integer type values which are having preciding or the prefix values as `0x`.To print the values in Hexadecimal we use the `%x` or `%p` which prints the Hexadecimal values. These values are range from `0, 1, 2, 3, 4, 5, 6, 7, 8, a, b, c, d, e, f `. To get the input from the user of a Hexadecimal values we use 
  - `%p` : To get the input from the user in Hexadecimal format with prefix `0x`.
  - `%x` : To get the input from the user in Hexadecimal format without the prefix `0x`.
    
  | Hex | Binary |
  | --- | ------ |
  | 0   | 0000   |
  | 1   | 0001   |
  | 2   | 0010   |
  | 3   | 0011   |
  | 4   | 0100   |
  | 5   | 0101   |
  | 6   | 0110   |
  | 7   | 0111   |
  | 8   | 1000   |
  | 9   | 1001   |
  | a   | 1010   |
  | b   | 1011   |
  | c   | 1100   |
  | d   | 1101   |
  | e   | 1110   |
  | f   | 1111   |

  ```c
  int val;
  printf("%x", val); // prints the Hexadecimal values without the prefix values
  printf("%p", val); // prints the Hexadecimal values with the prefix value
  ```

### Octal
The octal values are the integer values which are prefixed with `0` and to print the Octal values we use the `%o` and `0%o`. `0, 1, 2, 3, 4, 5, 6, 7`. To get the Octal values from the user we use the `%o`. 
| Octal | Binary |
| ----- | ------ |
| 0     | 000    |
| 1     | 001    |
| 2     | 010    |
| 3     | 011    |
| 4     | 100    |
| 5     | 101    |
| 6     | 110    |
| 7     | 111    |

```c
int val = 073;
printf("%o", val); // prints the value in Octal without prefix.
printf("0%o", val); // prints the value in Octal with prefix.
```
- To take input in any format we can use the common operator taking input in any integer format. `%i` is used to get the input from the user in any format.
  NOTE : When we use `%i` it's mandatory to use the prefix in the input.

### Floating Points 
- when we print the floating values in the fractional part we will get **six** Zero's in the fractional part by defualt.
- we use `%f` to get the values in normal floating points notation.
- we use `%e` to get the values in exponential notation.
- we use `%g` to get the values in both the formats i.e, floating point notaion and expinential notation.
  
```c
  float f = 234.3;
  printf(" %f ", f); // o/p : 234.300000
  printf(" %e ", f); // o/p : 2.343000e+02
  scanf(" %f ", &f); // i/p : 24.03
  printf(" %f ", f); // o/p : 24.030000
  printf(" %e ", f); // o/p : 2.403000e+01
```
  


    


  
  








  

















































 
 
