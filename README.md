# BOOLEAN_FUNCTION_MINIMIZATION

## Aim:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

## Software:

Quartus prime

## Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

## Program:

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: M.N.SOUNDARIYAN 

RegisterNumber: 212222230146

```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule

```
## RTL realization:

![image](https://github.com/soundariyan18/BOOLEAN_FUNCTION_MINIMIZATION/assets/119393307/cbad0ebc-ada5-4df8-bf6b-7cd79ea21902)


## Truthtable:

![image](https://github.com/soundariyan18/BOOLEAN_FUNCTION_MINIMIZATION/assets/119393307/fe446241-757c-4e7d-98ba-8fecfab7c320)


## Output:

![image](https://github.com/soundariyan18/BOOLEAN_FUNCTION_MINIMIZATION/assets/119393307/1b88361c-9811-4aed-92f8-d9aea23607ab)


## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
