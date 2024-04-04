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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

~~~

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

Developed by: Naresh Kumar V
Register Number:212223040126
~~~



## Logic Symbol and Truth table
![319427043-ab520f8d-0d6f-4bb9-96e6-33968a037418](https://github.com/NARESH-KUMAR-V/BOOLEAN_FUNCTION_MINIMIZATION/assets/145842937/8bc3ac66-5363-42bc-b5b8-652a2a68bd36)

![319427157-21cb2aef-7529-4ced-a473-68b7a9e53d62](https://github.com/NARESH-KUMAR-V/BOOLEAN_FUNCTION_MINIMIZATION/assets/145842937/5b17ec02-0a62-40ad-9dee-ac084c1cc08e)

**RTL realization**

![319427331-4d407a87-3dc2-49e6-bea8-bb7683f1857d](https://github.com/NARESH-KUMAR-V/BOOLEAN_FUNCTION_MINIMIZATION/assets/145842937/023d38ba-c92d-4ea7-bb78-98754a925812)

**RTL**

![319427514-042b4487-4220-4e63-a855-f1475debf723](https://github.com/NARESH-KUMAR-V/BOOLEAN_FUNCTION_MINIMIZATION/assets/145842937/0899a6ce-fd9c-4757-9bc2-f117ea2e201e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

