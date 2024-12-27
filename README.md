# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**DATE:** 18/10/2024

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder:**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/user-attachments/assets/77cd9dd4-5d09-4bc7-917b-6ec27971cf25)


Figure -01 HALF ADDER

**Half Subtractor:**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

![image](https://github.com/user-attachments/assets/8f0e28f2-f593-46a9-998c-a3d6570ce7b3)

Figure -02 HALF Subtractor

**Procedure:**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:  B.Surya Prakash 

RegisterNumber: 212224230281

**Half Adder:**
```
module Exp3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule
```
**Half Subtractor:**
```
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```
**RTL Diagram:**

**Half Adder:**

![image](https://github.com/user-attachments/assets/55acd450-f912-4011-838c-09aae7ef76f8)

**Half Subtractor:**

![image](https://github.com/user-attachments/assets/2c4945b5-eadf-442c-b75b-22b2375d334d)

**Output/TIMING Waveform:**

**Half Adder:**

![image](https://github.com/user-attachments/assets/1d27465b-337e-4286-8d56-07e883238cdc)

**Half Subtractor:**

![image](https://github.com/user-attachments/assets/63e79da8-f4bc-4cb4-ad92-69abe4b2fd8f)

**Result:**

 Thus the are Half-Adder-and-Half Subtractor-circuit studied and the output is
verified
