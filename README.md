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



Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B



Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
<img width="487" height="315" alt="Screenshot 2025-12-03 090228" src="https://github.com/user-attachments/assets/01a1a56f-c197-4f96-a40d-5fcbf4747f61" />
<img width="532" height="323" alt="Screenshot 2025-12-03 092255" src="https://github.com/user-attachments/assets/c1026937-47e8-4a7f-b32c-5117a2b15897" />


module exp3no1(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

module exp3no2(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule



/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: RegisterNumber:*/

**RTL Schematic**
<img width="356" height="170" alt="Screenshot 2025-12-03 090201" src="https://github.com/user-attachments/assets/97efc41c-be09-42b6-9f2d-39f90ddb67fd" />
<img width="395" height="188" alt="Screenshot 2025-12-03 091945" src="https://github.com/user-attachments/assets/10d9342c-150b-47a1-98a3-4bd2f25e437c" />



**Output/TIMING Waveform**
<img width="1915" height="324" alt="Screenshot 2025-12-03 090642" src="https://github.com/user-attachments/assets/7a7569b5-c0c4-41d4-8163-818521da8ac1" />
<img width="1894" height="316" alt="Screenshot 2025-12-03 092207" src="https://github.com/user-attachments/assets/a3d62be8-f606-4386-acb0-1773be6c00e4" />



**Result:**




