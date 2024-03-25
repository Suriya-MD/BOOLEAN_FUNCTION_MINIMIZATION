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
~~~
module exp2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
~~~
**Developed by: SURIYA M**

 **RegisterNumber: 212223110055**


**RTL realization Output:**

![image](https://github.com/Suriya-MD/BOOLEAN_FUNCTION_MINIMIZATION/assets/147120571/ba12ba41-a6b6-4ed4-84fe-711af48f587a)

**Truth table**

![image](https://github.com/Suriya-MD/BOOLEAN_FUNCTION_MINIMIZATION/assets/147120571/1c135ffa-c643-4d05-ad0c-ec59ff2ee26b)

**Timing Diagram**

![image](https://github.com/Suriya-MD/BOOLEAN_FUNCTION_MINIMIZATION/assets/147120571/8b186339-a4a4-4929-ac32-83965339c5c5)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

