# HALF_ADDER_SUBTRACTOR
**EXP3: HALF ADDER AND SUBTRACTOR**

NAME: VIJAYAKUMAR.S

REG NO: 24900562


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

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

![half-adder-truth-table](https://github.com/user-attachments/assets/c49aa077-e0b6-4e14-b578-7278cc8540cb)
![Half Substractor Truth Table](https://github.com/user-attachments/assets/d2e7e093-f9e3-414a-8c94-cdc434084e5b)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and half subtractor circuit and verify its truth table in quartus using Verilog programming.

Half adder program:

  module halfadd(a,b,sum,count);

  input a,b;

  output sum,count;

  xor (sum,a,b);

  and (cout,a,b);

  endmodule



Half subtractor program:

  module halfsub(a,b,diff,borr);

  input a,b;

  output diff,borr;

  wire w1;

  xor g1(diff,a,b);

  not g2(w1,a);

  and g3(borr,w1,b);

  endmodule

**RTL Schematic**


![half add rtl](https://github.com/user-attachments/assets/4830f194-9ad4-48c8-a1fe-a2a33a18d515)
![half sub rtl](https://github.com/user-attachments/assets/e8531dda-5c21-42c4-97fa-78234917e645)

**Output/TIMING Waveform**
![halfadd wave](https://github.com/user-attachments/assets/a0543c9f-ce6d-4243-b60a-c3ba8ec46084)
![half sub wave](https://github.com/user-attachments/assets/440f32ee-7ea7-4435-8e8f-5aef34ce3b6b)
**Result:**

Thus a half adder and half subtracter circuits are designed and its truthtable is verified in Quartus II using Verilog programming
