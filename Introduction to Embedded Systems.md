**Introduction to Embedded Systems:**

Embedded System is a combination of Hardware and Software. Software that
running on hardware is called Embedded systems. With the help of micro
controller and micro processor's we build the devices and with the help
of these, we do the tasks.

SOC's (System of Chip) used in smartphone, TV, CCTV, infotainment
systems used in cars.

**Micro controller \| Micro Processors \| SOC's**

They execute the instructions given by the user and convert into the
machine language \| low level lang.

Audino is not the name of Micro controller. It is the name of software\|
hardware platform.

**Differences between Microcontroller and Microprocessor:**

+-----------------------------------+-----------------------------------+
| **Micro Controller**              | **Micro Processor**               |
+===================================+===================================+
| It has less speed or less clock   | It executes the instructions in   |
| speed compared to micro processor | more clock speed compared to the  |
|                                   | micro controller                  |
+-----------------------------------+-----------------------------------+
| (intel) 8051 -- 12MHz (1980)      | intel i3, i5, i7, i9 Speed 1GHz   |
|                                   | to 5GHz                           |
| The micro controller measured in  |                                   |
| Hz (no. of cycles/sec) advance    | (\> 1GHz)                         |
| version of 8051 which can work at |                                   |
| 22MHz to 80MHz                    |                                   |
+-----------------------------------+-----------------------------------+
| (Atmel) Audino -\> Atmaga 2560    | The speed is the major difference |
| runs instructions in 16MHz.       | b/w micro controller and          |
|                                   | microprocessor.                   |
|                                   |                                   |
|                                   | AMD Ryzen speed 1GHz -- 5GHz (\>  |
|                                   | 1GHz).                            |
+-----------------------------------+-----------------------------------+
| (ARM holdings)                    | Intel SBC's (single board         |
|                                   | computer's) used in defence and   |
| ARM7 -\> 12MHz (1990) advanced    | aerospace, medical technology     |
| variants -\> 88MHz                |                                   |
|                                   | SBCs are (rugged SBC's) where     |
| Most of the micro controllers are | they can withstand heavy          |
| running below 100MHz              | atmosphere.                       |
+-----------------------------------+-----------------------------------+
| It uses the single core for       | It uses multiple cores of         |
| execution; they only have the     | execution (Quart core -\> each    |
| single core and have less speed.  | core can have 2GHz and for 4      |
|                                   | cores 4 \* 2 -\> 8GHz) they are   |
|                                   | used in servers and have multiple |
|                                   | cores.                            |
+-----------------------------------+-----------------------------------+

SOCs: they are combination of best in Microcontroller and
Microprocessor.

**Linux:**

Linux is an integrated development environment (IDE). We can use it for
the Command Line interface (CMD) tools like Vi (visual Interface), Vim
(visual interface Machine).**\**

we use all the tools as Commands Using terminal. It is pre-installed to
with every Linux OS, Printf () a 'c' standard function.

Vi: **\$vi filename:** used to open the file in vi Editor.

**\$ls:** shows list of files in a directory

**. S:** file is the assembly Code.

**-a, -i, -l:** These are flags / options

file information:

1\. file permission Read /write/ Execute)

2\. user name / group name.

3\. Size of the file.

4\. Date & time the file is created

5\. name of the file.

**\$ man ls \| \$ ls --help:** for all the flags /options and other
commands.

CPU understand only instructions; these instructions are present in
executable file (a.out - assembler output.

C statements -\> compiler (GCC) -\> instructions -\> executable file
(a.out) \[assembler output\]

G -\> GNU

C -\> c

C -\> compiler

**\$ rm filename**: To remove a file.

**-I:** data and information of the file.

Assembler output: ./a.out: tp execute the 'c' program.

**Commands to manage Directories / folders: -**

**\$ cd Dirname**: To go to a directory.

**\$ cd..** : To go to the Previous directory.

**\$cd:** Directory jump to the main directory.

**\$pwd:** Present Working Directory.

**\$cd/:** To go to the root Directory.

**\$mkdir Dirname:** To Create a new directory.

**Removing a directory: -**

In Empty directory:

**\$ rm -d Dirname \| \$ rmdix Dirname:** To remove an empty directory.

Non - Empty directory:

**\$ rm -r Dirname:** To remove a non- empty directory.

**-r:** recessively go to the sub flies /directories and delete.
