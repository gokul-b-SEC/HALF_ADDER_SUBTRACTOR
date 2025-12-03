# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)
module exp301(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)
 module experi333(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule

Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
<img width="491" height="209" alt="Screenshot 2025-11-23 130254" src="https://github.com/user-attachments/assets/76093fd8-10eb-4a7b-8c64-ca2a2d5b3af9" />
<img width="499" height="286" alt="Screenshot 2025-11-23 130315" src="https://github.com/user-attachments/assets/144ea00c-206e-4d12-88d4-0ed80789d8b5" />



/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: RegisterNumber:*/

**RTL Schematic**

**Output/TIMING Waveform**

**Result:**
<img width="788" height="390" alt="Screenshot 2025-11-21 185034" src="https://github.com/user-attachments/assets/2700c470-795c-4ad3-83d1-5ab662fe4870" />
<img width="1899" height="180" alt="Screenshot 2025-11-21 185226" src="https://github.com/user-attachments/assets/ee1d2d56-8441-45b5-a7d2-0d216b55e068" />
<img width="710" height="326" alt="Screenshot 2025-11-21 185722" src="https://github.com/user-attachments/assets/94fa87af-ca69-4796-bb43-820eacb9764d" />
<img width="1894" height="186" alt="Screenshot 2025-11-21 185857" src="https://github.com/user-attachments/assets/d7e8e11d-dad1-490a-bac7-30e1ae5f6f55" />




