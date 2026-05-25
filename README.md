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

Developed by: DHARNEESH S
RegisterNumber: 212225220022
*/
```
module deexp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
**RTL realization**

<img width="1123" height="736" alt="image" src="https://github.com/user-attachments/assets/a5e292f0-85b5-4f5f-b31b-11034a4237a0" />

**Output:**

**RTL**

<img width="1262" height="534" alt="image" src="https://github.com/user-attachments/assets/3b7fb7b4-003c-4a8d-a0b1-f41e6e5e26e4" />


**Timing Diagram**

<img width="1259" height="526" alt="image" src="https://github.com/user-attachments/assets/7ce21013-7b3b-4a79-896d-1b30337e0b51" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

