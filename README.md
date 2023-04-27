# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: BALA MURUGAN.P
RegisterNumber:  212222230017
*/
```
module tt1(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,Y,X,Z;
output F1,F2;
wire A1,A2,A3,A4,A5,B1,B2,B3,B4,B5;
assign A1 = ((~A)&(~B)&(~C)&(~D));
assign A2=(A&(~C)&(~D));
assign A3=((~B)&C&(~D));
assign A4=((~A)&B&C&D);
assign A5=(B&(~C)&D);
assign B1=(X&(~Y)&Z);
assign B2=((~X)&(~Y)&Z);
assign B3=((~W)&X&Y);
assign B4=(W&(~X)&Y);
assign B5=(W&X&Y);
assign F1=(A1|A2|A3|A4|A5);
assign F2=(B1|B2|B3|B4|B5);
endmodule
*/
```
## RTL realization
## Output:
## RTL

F1


![r](https://user-images.githubusercontent.com/118680410/234773568-18e26013-eb03-430e-9ad8-95188dad4ce9.png)

F2
![rt](https://user-images.githubusercontent.com/118680410/234773573-06f52483-33d6-465f-ac1d-b08aa34f69db.png)

## Timing Diagram
![w](https://user-images.githubusercontent.com/118680410/234773494-5af1e099-3717-435b-9120-ab8c531d7cb4.png)

TRUTH TABLE


![Uploading s1.png…]()

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
