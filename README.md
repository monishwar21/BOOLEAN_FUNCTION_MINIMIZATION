# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of simplifying Boolean algebraic expressions to reduce the number of logic gates and complexity in a digital circuit, leading to more efficient, faster, and less costly hardware For minimizing Boolean expressions,we can use a set of rules and laws (like distributive, associative, and complement laws) to simplify Boolean expressions. This method focuses on applying algebraic manipulations to reduce the complexity of the expression by eliminating redundant terms.

Identity Law A ⋅ 1 = A, A + 0 = A Null Law A ⋅ 0 = 0, A + 1 = 1 Idempotent Law A ⋅ A = A, A + A = A Complement Law A ⋅ A′ = 0, A + A' = 1 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′ Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C Commutative law A B = B A,A + B = B + A
**Logic Diagram**
1)IDENTITY LAW:
![Identity law](https://github.com/user-attachments/assets/f30ef5aa-d536-4e60-91cc-810f2e6d5902)

2)NULL LAW:
<img width="1034" height="573" alt="Screenshot 2025-11-26 210358" src="https://github.com/user-attachments/assets/9a9a8379-491e-471e-8be8-d1056922e11f" />

3)IDEMPOTENT LAW:
![idempotent law](https://github.com/user-attachments/assets/cec03010-2e80-4556-a117-2ef6e5c333c1)

4)COMPLEMENT LAW:
![complement law](https://github.com/user-attachments/assets/4ae48ceb-2fff-48b9-8e6a-76c73c035a23)

5)DISTRIBUTIVE LAW:
<img width="1035" height="716" alt="Screenshot 2025-11-26 210616" src="https://github.com/user-attachments/assets/c139cd25-6a5d-4765-91fe-ff4927d0b263" />

6)DE-MORGANS LAW:
<img width="1036" height="539" alt="Screenshot 2025-11-26 210804" src="https://github.com/user-attachments/assets/dfb4489e-4442-45cf-9b5c-22beafd0e2e0" />

7)ABSORBTION LAW:
<img width="433" height="158" alt="Screenshot 2025-11-26 210855" src="https://github.com/user-attachments/assets/db5a7c43-168a-40ba-9b63-93132bda2b46" />

8)ASSOCIATIVE LAW:
<img width="691" height="713" alt="Screenshot 2025-11-26 210952" src="https://github.com/user-attachments/assets/7e26f268-b699-4e9c-b24f-c6aabd6bb6fc" />

9)COMMUTATIVE LAW:
<img width="684" height="766" alt="Screenshot 2025-11-26 211019" src="https://github.com/user-attachments/assets/4499bc16-73ba-4015-bb99-28aebeceb1e9" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
i)

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii)

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule

Developed by: K MONISHWAR RegisterNumber: 25014914


**RTL realization**

**Output:**
1)
<img width="1235" height="582" alt="Screenshot 2025-11-26 212618" src="https://github.com/user-attachments/assets/366dccf7-0b74-4ec6-9db2-ed4cc8773d1f" />


<img width="1201" height="577" alt="Screenshot 2025-11-26 212706" src="https://github.com/user-attachments/assets/a5d02ac3-d7ce-4013-b7d1-cc4336b144c6" />



**Timing Diagram**
1)
<img width="1281" height="717" alt="Screenshot 2025-11-26 213136" src="https://github.com/user-attachments/assets/4384d5c3-654a-4896-834e-3c7b596b1480" />
2)
<img width="1279" height="679" alt="Screenshot 2025-11-26 213202" src="https://github.com/user-attachments/assets/7452ffdb-7776-4403-b3b9-b6f043737f8c" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

