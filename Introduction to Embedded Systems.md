# 1.Introduction to Embedded Systems:

**Embedded System** is a combination of Hardware and Software. Software that running on hardware is called Embedded systems. With the help of micro controller and micro processor's we build the devices and with the help of these, we do the tasks. **SOC's** (System of Chip) used in smartphone, TV, CCTV, infotainment systems used in cars.**Micro controller | Micro Processors | SOC's**They execute the instructions given by the user and convert into the machine language | low level lang. Audino is not the name of Micro controller. It is the name of software | hardware platform.

## **Key Differences between Microcontroller and Microprocessor:**

| **Micro Controller**              | **Micro Processor**               |
|-----------------------------------|-----------------------------------|
| It has less speed or less clock speed compared to micro processor    | It executes the instructions in more clock speed compared to the  micro controller   |
| (intel) 8051 -- 12MHz (1980) The micro controller measured in  Hz (no. of cycles/sec) advance version of 8051 which can work at 22MHz to 80MHz | intel i3, i5, i7, i9 Speed 1GHz to 5GHz (\> 1GHz) |                                                   
| (Atmel) Audino -> Atmaga 2560  runs instructions in 16MHz. | The speed is the major difference b/w micro controller and microprocessor. AMD Ryzen speed 1GHz  5GHz (> 1GHz).|
| (ARM holdings)   ARM7 -\> 12MHz (1990) advanced  variants -\> 88MHz .| Intel SBC's (single board  computer's) used in defence and aerospace, medical technology.|                        
| SBCs are (rugged SBC's) where Most of the micro controllers are  running below 100MHz. |  they can withstand heavy atmosphere.|
| It uses the single core for execution; they only have the single core and have less speed.| It uses multiple cores of execution (Quart core -\> each core can have 2GHz and for 4 cores 4 \* 2 -\> 8GHz) they are used in servers and have multiple cores.|

**SOCs**: they are combination of best in Microcontroller and
Microprocessor.

# 2.**Linux:**

Linux is an integrated development environment (IDE). We can use it for
the Command Line interface (CMD) tools like Vi (visual Interface), Vim
(visual interface Machine).**\**

we use all the tools as Commands Using terminal. It is pre-installed to
with every Linux OS, Printf () a 'c' standard function.

## **Linux commands:** 
```ls:``` shows list of files in a directory.
```.s:``` file is the assembly Code.
```-a, -i, -l:``` These are flags / options
## **File information:**
1\. File permission ( Read /write/ Execute)
2\. User name / Group name.
3\. Size of the file in Kbs.
4\. Date & time when the file is created
5\. Name of the file.

For all the flags /options and other commands.
```
man ls 
ls --help
```
CPU understand only instructions; these instructions are present in
executable file (a.out - assembler output).

C statements -\> compiler (GCC) -\> instructions -\> executable file
(a.out) \[assembler output\]

G -\> GNU

C -\> c

C -\> compiler

**\$ rm filename**: To remove a file.

**-I:** data and information of the file.

Assembler output: ./a.out: tp execute the 'c' program.

## **Commands to manage Directories / folders**
To go to a directory.
```
cd Dirname
```
To go to the Previous directory.
```
cd..
```
Directory jump to the main directory.
```
cd:
```
Present Working Directory.
```
pwd:
```
To go to the root Directory.
```
cd/
``` 
To Create a new directory.
```
mkdir Dirname
```
## **Removing a directory**

## In Empty directory:
To remove an empty directory.
```
rm -d DirectoryName
rmdix DirectoryName
```
```-d:``` can also indicate a directory when looking at file permissions with ls -l (the first character will be d if it's a directory). 
## Non - Empty directory:
To remove a non- empty directory.
```
rm -r DirectoryName
```
```-r``` recessively go to the sub flies /directories and delete.
