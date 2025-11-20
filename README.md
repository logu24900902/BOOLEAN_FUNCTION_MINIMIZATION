# EXP2 . BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**logic diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: LOGU R
RegisterNumber: 212224230141 

```
module DE2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=X1|X2|X3|X4|X5;
assign F2=X6|X7|X8|X|X10;
endmodule
```
## K-map :
![kmap1](https://github.com/user-attachments/assets/9e884bb5-cb9d-4b69-9183-5377aa21a5fe)




**RTL realization**
![Screenshot 2024-11-25 184617](https://github.com/user-attachments/assets/c6ddd8e1-5555-47b2-a21f-275b724d5495)

**Output:**
![Screenshot 2024-11-25 184642](https://github.com/user-attachments/assets/413d90b7-6f57-453c-bb7d-3b5c4e2e08f2)
**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

