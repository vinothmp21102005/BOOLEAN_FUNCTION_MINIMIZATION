# BOOLEAN_FUNCTION_MINIMIZATION

## AIM:

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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. */

## Developed by: VINOTH M P
## RegisterNumber: 212223240182
```
module de2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```
```
module de2(w,x,y,z,F2)
intput w,x,y,z;
output F2;
assign F2=((~y&z)|(x&y)|(w&y));
endmodule
```


**RTL realization**
#### program F1:
![image](https://github.com/user-attachments/assets/449ffb0a-d457-4feb-a20a-02c83215daed)

#### program F2:
![image](https://github.com/user-attachments/assets/c08dde95-ee29-436c-a967-2d93dca389ef)

### Truth Table:
#### F1:
![image](https://github.com/user-attachments/assets/3ba84594-c272-4313-a88c-bb2d8fbb469b)


#### F2:
![image](https://github.com/user-attachments/assets/65aadc93-4d31-4f98-af4b-ace43e67d6c4)





**Output:**
#### for program F1:
![image](https://github.com/user-attachments/assets/8b83ca8d-2232-48d1-bf1c-e032f65bd4c9)

#### for program F2:
![image](https://github.com/user-attachments/assets/4640c4a9-b82b-4b10-b477-46580bb34ff6)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

