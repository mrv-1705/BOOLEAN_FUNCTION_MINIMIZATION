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

![EXP 2 DE](https://github.com/mrv-1705/BOOLEAN_FUNCTION_MINIMIZATION/assets/114565075/cd2a3cd0-76c8-46f5-8957-1f8bdb99edc1)


![DE EXP2](https://github.com/mrv-1705/BOOLEAN_FUNCTION_MINIMIZATION/assets/114565075/dc6c4278-ea15-48ef-9b1a-79adb97d6c87)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```

Name: Kurapati Vishnu Vardhan Reddy
Developed by: RegisterNumber: 212223040103
```
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




**RTL realization**

![DE EXP 2 RTL](https://github.com/mrv-1705/BOOLEAN_FUNCTION_MINIMIZATION/assets/114565075/a1e5e7c2-eae4-4a33-aea7-026fde0e529c)


**Output:**

![DE EXP 2 OUTPUT](https://github.com/mrv-1705/BOOLEAN_FUNCTION_MINIMIZATION/assets/114565075/a2709398-688a-4fb2-8748-28368437b7cb)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

