# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

### Half Subtractor Full Subtractor
### Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

### Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

### Procedure

STEP 1: Use module project name(input,output) to start the Verilog programmming.
STEP 2: Assign inputs and outputs using the word input and output respectively.
STEP 3: Use defined keywords like wire,assign and required logic gates to represent the boolean
expression.
STEP 4: Use each output to represnt onre for differnce and the other for borrow.
STEP 5: End the verilog program using keyword endmodule.


### Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
### Developed by: GUGHAN S
### RegisterNumber: 212223240043 
*/

### CODE:

### HALF SUBRACTOR:
![Exp4 hs code](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/2f8ec1f8-28f4-41b8-846d-cc330552eb35)

### FULL SUBRACTOR:
![Exp4 fs code](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/942481a7-7ca1-4f62-a24c-3facc4cd464c)


### Output:

## Truthtable:

### HALF SUBRACTOR:
![Exp4 truthtable hs](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/c516319a-d9f8-4be9-8ba6-ebcaeffeea0d)

### FULL SUBRACTOR:
![Exp4 truthtable fs](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/8edc7af9-a0bd-4684-a625-4e138054b5f4)



###  RTL realization:

### HALF SUBRACTOR:
![Exp4 hs RTL diagram](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/8d617622-2a9d-4863-afa1-da8105b62380)

### FULL SUBRACTOR:
![Exp4 fs RTL diagram](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/04d408a2-acc6-4599-b7b3-c7b4880211ce)


### Timing diagram:

### HALF SUBRACTOR:
![hs wave](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/088bb30d-0127-441c-b5f3-270acd08bf5b)

### FULL SUBRACTOR:
![fs wave](https://github.com/GUGHAN-3001/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009432/07178e9b-b3d4-4a6c-b7d3-0f2670e1b32f)


## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
