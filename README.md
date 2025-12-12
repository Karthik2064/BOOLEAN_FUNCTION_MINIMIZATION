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

~~~
 module ex2 (a,b,c,d,w,x,y,z,f1,f2);
 input a,b,c,d,w,x,y,z; output f1,f2;
 assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
 assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
 endmodule
~~~


Developed by: K.Karthik

RegisterNumber:25017589


**Truth Table**

<img width="483" height="292" alt="image" src="https://github.com/user-attachments/assets/10292b50-90ce-4958-b99e-e826a88436d9" />

**RTL realization**

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/68e91143-1f00-44d2-963c-8d5ad8696f13" />

**Timing Diagram**

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/4aeada5d-0086-479f-abdb-031200be1f1f" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

