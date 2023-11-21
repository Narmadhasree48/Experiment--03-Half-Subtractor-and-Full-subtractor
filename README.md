# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure



Write the detailed procedure here 


## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
## Half Subtractor:
![Screenshot 2023-11-21 215206](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/a8d566b0-5c70-4e2b-a7a5-50500baf6e0a)

## Full Subtractor:
![Screenshot 2023-11-21 215210](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/87603587-384b-4ef1-b792-4f5effef33bb)

## Output:

## Truthtable:
## Half Subtractor:
![Screenshot 2023-11-21 215222](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/8663e4f4-dbb7-4e5c-b0ec-f945994320e5)

## Full Subtractor:
![Screenshot 2023-11-21 215228](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/fdc18ff7-245c-4397-a8d4-e3ccfd7971cb)

##  RTL realization:
## Half Subtractor:
![Screenshot 2023-11-21 215253](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/1fc3412e-fa14-49d5-83e2-a8323f0c620b)

## Full Subtractor:
![Screenshot 2023-11-21 215307](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/a02110bc-c5fc-4b5f-bbc8-e3cbc3cbd327)

## Timing diagram :
## Half Subtractor:
![Screenshot 2023-11-21 215343](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/e4aa8414-269d-4db5-9dc8-6253e84e1492)

## Full Subtractor:
![Screenshot 2023-11-21 215358](https://github.com/Narmadhasree48/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979451/52765a73-cd9a-463c-8583-83cc2f5713ba)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
