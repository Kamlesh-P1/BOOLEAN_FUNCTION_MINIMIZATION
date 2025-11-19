# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of simplifying a Boolean expression to its most basic form, using the fewest logic gates, variables, and operators possible. This is crucial in digital circuit design to create more efficient, faster, and cheaper circuits by reducing complexity and power consumption. Key methods for minimization include algebraic manipulation and Karnaugh maps. 

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

~~~
module ex2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|(w & y)|(x & y));
endmodul
~~~


**RTL realization**

<img width="820" height="808" alt="ex 2" src="https://github.com/user-attachments/assets/a73209fd-b85a-489e-a45d-cc22a665b187" />


**Output:**

<img width="1920" height="1125" alt="ex2" src="https://github.com/user-attachments/assets/9719681a-7cce-4508-acd6-374238468368" />

**RTL**

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

