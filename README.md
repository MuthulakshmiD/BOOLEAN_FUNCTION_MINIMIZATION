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

**Developed by:Muthulakshmi D
RegisterNumber:212223040122**
```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
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
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```
**logic symbol and truth table**

![{A938CF54-39DE-4B4F-B001-2D32DCB584B6}](https://github.com/user-attachments/assets/003ece39-e191-4e01-88bd-164cd8e734a4)

![{25565ACD-ED95-4970-901F-20E0F63C9D90}](https://github.com/user-attachments/assets/30ffc492-5d4f-4341-8743-e99e6f61bd77)
**RTL realization**

![{F3B3C80A-0C36-4CFE-9FFD-CAC11703A915}](https://github.com/user-attachments/assets/5be29395-3423-43c2-bd7d-8798806b2102)
**Output:**

![380815383-50a187d8-1971-487a-b826-3f3d8e2d70db](https://github.com/user-attachments/assets/4c32010a-4581-4a3d-9902-5d8c546d8a2f)
**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
