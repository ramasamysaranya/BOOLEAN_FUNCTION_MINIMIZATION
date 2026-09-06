# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```

Developed by: Saranya R RegisterNumber: 212225040384


**RTL realization**

<img width="787" height="623" alt="WhatsApp Image 2026-09-05 at 6 22 05 PM" src="https://github.com/user-attachments/assets/25afdcbd-4c35-4c1b-941e-72ec382ccb89" />


**Output RTL:**

<img width="1600" height="899" alt="WhatsApp Image 2026-09-05 at 6 21 55 PM" src="https://github.com/user-attachments/assets/5838d3ee-e7d7-4c8b-8359-4d3eac594a5e" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

