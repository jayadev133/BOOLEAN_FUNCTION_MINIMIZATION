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


```
Developed by: JAYADEV PALLINTI
RegisterNumber: 212223240058

module EXP_02(a,b,c,d,w,x,y,z,f1,f2);
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
and(s,ydash,z);
and(t,x,y);
and(u,w,y);
or(f2,s,t,u);  

endmodule 
```


**RTL realization**

**Output:**
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5cb50b54-7ffa-42e6-80fe-0c21cfe4d1e6" />


**RTL**
<img width="1919" height="1079" alt="Screenshot 2025-09-26 113016" src="https://github.com/user-attachments/assets/012b0d92-0cc3-4391-b49c-45d3baa5996c" />


**Timing Diagram**

<img width="1919" height="1079" alt="Screenshot 2025-09-26 113016" src="https://github.com/user-attachments/assets/ae176ed8-19bf-4f5b-a4b9-fbfc20ebceb2" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

