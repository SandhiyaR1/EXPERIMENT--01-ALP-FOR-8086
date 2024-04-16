### Name : SANDHIYA R

### Roll no : 212222230129
# EXPERIMENT-01 ALP FOR 8086

## Aim: 
To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 
8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 ![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)


9.	Click on emulate to start emulation 

![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)


10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 


![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)

### Programs for arithmetic  operations

### Addition  of 16 bit ALP 
```
MOV Ax,04D2h;
MOV Bx,01C5h;
ADD Ax,Bx;
MOV [2346h],Ax;    
ret
```
## Output 
![image](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/dea2b26d-9376-4fd4-bc91-319f0ef3e59f)

 
### Subtraction   of 16 bit numbers  ALP 
 ```
MOV Ax,04a3h;
MOV Bx,01b2h;
SUB Ax,Bx;
MOV [2346h],Ax;    
ret
```       
### Output  
![image](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/d7b3d0eb-8d44-4b4f-bc0a-06dcae2548e8)

### Multiplication alp 
```
MOV AL,0a2H;
MOV BL,0c3H;
MUL BL;
MOV [2345H],AL;
ret
```
### Output  
![image](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/a5ca15a2-89b0-4067-aaec-147dc3de383e)


### Division alp 
```
MOV AX,1102H;
MOV BX,1100H;
DIV BX;
ret
```

### Output  
![image](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/309d5e6d-1d67-4139-abf6-e4caa90fe9e9)

### AND
```
ORG 100H
MOV BX,10000H;
AND BX,1111H;
MOV [0040H+02],BX;
ret
```
### Output
![WhatsApp Image 2024-04-16 at 15 57 08_43efb06a](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/47bf23d1-2a23-4721-b71f-d183189226ff)


### OR 
```
ORG 100H
MOV AX,[0040H+06];
MOV BX,1000H;
OR AX,BX;
MOV [0040H+02],AX;
ret
```
### Output
![WhatsApp Image 2024-04-16 at 15 57 34_e46aef15](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/4fcf19ed-1d12-43ef-a36c-bacb8344b6d3)


### NOT
```
ORG 100H
MOV BX,0040H;
MOV AX,[BX];
NOT AL;
MOV [0040H+04],AX;
ret

```
### Output
![WhatsApp Image 2024-04-16 at 15 58 08_518352a0](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/ba7f1cad-82c9-402e-9982-a558f94ec99d)


### XOR
```
org 100h
mov bx,0040h;
mov ax,[bx]; 
xor ax,bx;
mov [0040h+04],ax;
ret
```
### Output

![WhatsApp Image 2024-04-16 at 15 58 27_92869fad](https://github.com/SandhiyaR1/EXPERIMENT--01-ALP-FOR-8086/assets/113497571/a8238626-6a6a-42a9-a724-802ae394ba2a)


### Result :
Thus the ALP on fundamental arithmetic and logical operations are executed successfully.
 








