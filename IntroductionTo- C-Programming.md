## Introduction To C- Programming
C is a powerful, general-purpose programming language developed by Dennis Ritchie in the early 1970s at Bell Labs. It is known for its speed, efficiency, and close-to-hardware capabilities, making it ideal for system programming, such as operating systems and embedded systems. C provides low-level memory access, a simple set of keywords, and a clean style, making it a popular choice for beginners and professionals alike. Its influence can be seen in many modern languages like C++, Java, and Python.
## **1. Basic Elements**
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


-**Numerics** : The integer values are the numbers are also called as Character set in which these Numerics are also having the corresponding **ASCII** values.

 
 
