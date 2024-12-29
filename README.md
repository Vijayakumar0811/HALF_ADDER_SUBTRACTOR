# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**EXP3: HALF ADDER AND SUBTRACTOR**

NAME: VIJAYAKUMAR.S

REG NO: 24900562

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

![half-adder2](https://github.com/user-attachments/assets/152001ee-8d87-4b49-ad17-1873da25efbc)
![half-subtractor2](https://github.com/user-attachments/assets/7aea9729-82c7-4284-93a8-f13c5bce8ca4)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

module hadd(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule


**RTL Schematic**

![Screenshot 2024-12-22 212351](https://github.com/user-attachments/assets/3e57f5dd-148f-4e69-b794-628a8f3769b4)
![Screenshot 2024-12-29 141048](https://github.com/user-attachments/assets/9c3a09b7-18ec-4318-9feb-c4800ccad9d5)

**Output/TIMING Waveform**

![Screenshot 2024-12-29 141817](https://github.com/user-attachments/assets/ccaf8c51-5520-4463-8b34-41068c2d92c3)
![Screenshot 2024-12-29 141235](https://github.com/user-attachments/assets/d1cbde11-e4fb-4a8a-b63b-fc249124d5c5)

**Result:**


Thus a half adder and half subtractor circuit is designed and its truth table is verified in Quartus using Verilog programming.

