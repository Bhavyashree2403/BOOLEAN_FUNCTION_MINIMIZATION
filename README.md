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

module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);\
input a,b,c,d,w,x,y,z;\
output f1,f2;\
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;\
not(adash,a);\
not(bdash,b);\
not(cdash,c);\
not(ddash,d);\
not(ydash,y);\
and(p,bdash,ddash);\
and(q,adash,b,d);\
and(r,a,b,cdash);\
or(f1,p,q,r);\
endmodule

Developed by:BHAVYASHREE . R\
RegisterNumber:212223110006




**Output:**
![Screenshot (325)](https://github.com/Bhavyashree2403/BOOLEAN_FUNCTION_MINIMIZATION/assets/149219738/32c6f18c-d6d0-4780-8280-a4d9bdea9ba0)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

