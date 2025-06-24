# **1.Introduction To Vi Editor** 
**Vi Editor** is Used to write the code in terminal and also used to create a file using Vi tool. Vi editor has two modes

- To write the code in terminal known as **Insert Mode.**
- To do the adminstrative operations known as **Command Mode.**

When we create a file using Vi tool it will open the file in Command mode where we can choose the mode of writing the code in the terminal using Vi Editor. Vi Editor by default oepens in Command Mode before saving the file the modified / changes will be stored in **Internal memory.**
The Vi Tool has some commands which are used for editing the program or the file using Vi Editor and these commands are used for the programming in Vi Editor these command can make the editing easier and faster to do using Vi editor.
The following are the some of the commands of Vi editor 

# **2.Vi Tool Commands**
To use the Vi editor we need to install the Vi editor, to install Vi editor we use **VIM** 
```
sudo apt install vim
```
To create a file using VIM 
```
vi FileName.extension
```
- After creating the file it will open the file in Command mode by default.

To switch from **Command Mode** to **Insert Mode.**
```
press key 'i'
```
To switch from **Insert Mode** to **Command Mode.**
```
press the 'Esc' key
or
Ctrl + c
```
# **Commands used in Command Mode** 
To save the file for Writing or to edit again.
```
:w
```
To save the file for Execution purpose.
```
:x
```
To replace a single character
```
:r
```
To exit from the command mode and go to the **CMD** to execute file.
```
:q
or
Ctrl + zz
```
To Quit from the Vi editor without saving the file.
```
:q!
```
To copy the single line from the code that we have written from the place where the cursor is placed.
```
yy
```
To copy two lines from the point where the cursor is placed.
```
2yy
```
- If we are copying more than 2 lines a notification appears at bottom left side of the Vi Editor.

To copy more than two lines of the code or the statements.
```
<Number of Lines to be copied>yy
```
To copy single word from the place where the cursor placed.
```
yw
```
To copy more than two words from the place where the cursor is placed.
```
<Number of the words to be copied>yw
```
To delete a single line from the place where the cursor is placed.
```
dd
```
To search for the string in the code in the file that we have created in Vi Editor and this command will gives us the **First Occurence** of th string.
NOTE : Search Operation is Case Sensitive.
```
/<String-Name>
```
To go to the next line of the Occurence of the string in Forward direction.
```
n
```
To go to the next Occurence of the string in Backward direction.
```
Shift + n
```
To get the Documentation of the library or flag or any other funtions we can use the command.
```
man <Library-Name>
```
To paste the coppied line below the current line.
```
p
```
To paste the coppied line above the current line.
```
P
```
To create the New Empty line below the current line.
```
press o
```
To create the New Empty line above the current line.
```
press O
```
To go to the last line in the program or the file.
```
press G
```
To go to the first line of the program or the file.
```
press gg
```
To go to the specific line in the program or the file.
```
:<Line-Number>
or
<Line-Number> G
or
<Line-Number> gg
```


































































