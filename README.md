# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:
```
LDA 4200H
ANI 01H
JZ L1
MVI A,01H
JMP L2
L1:MVI A,02H
L2:STA 4201H
HLT
```
## Output:
ODD: 
<img width="1825" height="644" alt="Screenshot 2026-02-06 162348" src="https://github.com/user-attachments/assets/31407761-838e-42ce-a654-f266ca1cfb3a" />
EVEN:
<img width="1835" height="529" alt="Screenshot 2026-02-06 162420" src="https://github.com/user-attachments/assets/cf98d876-f374-4494-9171-676cbc212c35" />


## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

