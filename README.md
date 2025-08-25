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
MVI A, 01H
JMP L2
L1: MVI A, 02H
L2: STA 4300H
HLT
```

## Output:
ODD (input)

<img width="1920" height="765" alt="MP MC EXP-2 ODD INPUT" src="https://github.com/user-attachments/assets/ef9ad6c1-9dfb-4614-8393-15cf9b98d229" />

ODD (output)

<img width="1920" height="735" alt="MP MC EXP-2 ODD OUTPUT" src="https://github.com/user-attachments/assets/4a6fbb0f-0d3c-4679-8759-0f5e4f72bb95" />

EVEN(input)

<img width="1920" height="787" alt="MP MC EXP-2 EVEN INPUT" src="https://github.com/user-attachments/assets/ae4a690e-ef1e-476b-b1cb-d0dad6eff17e" />

EVEN(output)

<img width="1920" height="688" alt="MP MC EXP-2 EVEN OUTPUT" src="https://github.com/user-attachments/assets/a2d5b0d6-62ce-4f53-bb88-c3e5333e2b55" />

EXPLANATION

![EXP-2 EXP](https://github.com/user-attachments/assets/f6925384-42f0-4e2c-890e-c51e55257c6a)

## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

