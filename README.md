# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

![WhatsApp Image 2024-12-21 at 09 37 42_81ca9c31](https://github.com/user-attachments/assets/716bee5a-edf5-4263-927c-ea3b786ae05a)


Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

![WhatsApp Image 2024-12-21 at 09 36 47_51967542](https://github.com/user-attachments/assets/7551aae7-e387-4b02-9bc7-9e6c2a9a91ed)


Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

Half subtractor
![WhatsApp Image 2024-12-21 at 09 36 46_6c621b77](https://github.com/user-attachments/assets/752fa2bc-8328-44b3-8415-8bba2eedf137)
Half adder

![WhatsApp Image 2024-12-21 at 09 37 41_42367385](https://github.com/user-attachments/assets/78eab8af-ce06-4387-995e-9771cec25e05)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and half subtractor circuit and verify its truth table in quartus using Verilog programming.
```
module Huff_adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=(a^b);
assign carry=(a&b);
endmodule
```
```
module half_sub(a,b,diff,borr);
input a,b;
output diff,borr;
assign diff=(a^b);
assign borr=(~a&b);
endmodule
```

Developed by: Thilak raj .P

RegisterNumber:24900585

**RTL**
![Screenshot 2024-11-05 135522](https://github.com/user-attachments/assets/9507253b-a57b-47e4-a83e-eccd455a4904)
![Screenshot 2024-11-05 140919](https://github.com/user-attachments/assets/818b4fe7-c0b5-46d3-8ab8-5c82f58f76f8)


**Output/TIMING Waveform**
![Screenshot 2024-11-05 135746](https://github.com/user-attachments/assets/0887f9f3-86b1-4b13-a1c8-663f3f44d17b)
![Screenshot 2024-11-05 142436](https://github.com/user-attachments/assets/42ba636e-c30f-4b79-bf7e-119899e45e93)

**Result:**
To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming is verified.
