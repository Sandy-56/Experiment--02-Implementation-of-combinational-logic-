# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 



## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


 

## Logic Diagram
## Procedure
## Program:
Connect the supply (+5V) to the circuit Switch ON the main switch Press the switches for inputs “A” and “B”. The switch is ON state when 1 is pressed. The switch is OFF state when 0 is pressed. If the output is 1, then the bulb glows. Check all the gates following the same procedure.
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Santhosh D M
RegisterNumber: 23013934
```

module DE_02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1= x1 | x2 | x3 | x4  |x5;
endmodule

```
*/
## RTL realization

## Output![263437285-de2e9e3f-6a9c-4e4c-8b7f-6a5889265057](https://github.com/Sandy-56/Experiment--02-Implementation-of-combinational-logic-/assets/152118022/b569f174-8eea-4a0a-a2b0-10da9bbb2ab8)
:![263437304-462ac9cc-7510-4fa9-ab8d-e2355c53830f](https://github.com/Sandy-56/Experiment--02-Implementation-of-combinational-logic-/assets/152118022/30da52c4-4fea-48c4-abf3-0bee03304914)


## RTL
![263437331-250474a6-747e-40cb-be3b-4d0c5473adb6](https://github.com/Sandy-56/Experiment--02-Implementation-of-combinational-logic-/assets/152118022/6213cd59-4e06-4918-9be4-714507c37211)


## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
