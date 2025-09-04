# EXPERIMENT--01-ALP-FOR-8086
Name :
Roll no 
Date of experiment :





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
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
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```

## Output  
<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/53005cb3-00bd-4113-ada3-35491603d5cf" />

 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
 
## Output 

<img width="2555" height="1599" alt="image" src="https://github.com/user-attachments/assets/37e0098e-70be-40d7-a077-ca19ac5c88d0" />

## Multiplication alp 

```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```

 ## Output  
<img width="2557" height="1599" alt="image" src="https://github.com/user-attachments/assets/8768ef9a-7eb1-4d63-aeb6-5a554d944f66" />


## Division alp 

```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  

<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/e8bd257d-588d-4016-a566-3a2f56fa0281" />

LOGICAL OPERATIONS

TRUTH TABLE FOR LOGICAL OPERATIONS

<img width="1957" height="1717" alt="image" src="https://github.com/user-attachments/assets/b77f4a3f-8a01-48dc-8001-7c0bf3ecca2b" />

AND alp

```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```

Output

<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/61f38199-a96f-446f-8f41-18a226817d2c" />

OR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```

Output

<img width="2559" height="1570" alt="image" src="https://github.com/user-attachments/assets/521638d4-d4b3-4901-a6cb-b6e0caf1e429" />


NAND alp

```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```

Output

<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/fa3f5ffe-4f59-4eaf-b822-ed06b9de2820" />

NOR alp

```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

Output

<img width="2559" height="1596" alt="image" src="https://github.com/user-attachments/assets/349206e0-4d70-430e-a77d-f31caf6a1642" />

NOT alp

```
MOV AX,[3001H]
MOV BX,[3003H]
NOT AX
MOV [3005H],AX
HLT
```

Output


<img width="2544" height="1599" alt="image" src="https://github.com/user-attachments/assets/6add7446-aa79-41ad-9f71-97680b975934" />

XOR alp

```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```

Output


<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/49d33bd4-77b3-4982-babc-f42bdb5984b0" />

XNOR alp

```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

Output


<img width="2559" height="1599" alt="image" src="https://github.com/user-attachments/assets/01d537cb-8e91-4f06-8c86-ae0ed796290e" />



## Result :
 
The Write and execute ALP on fundamental arithmetic and logical operations is executed successfully.







