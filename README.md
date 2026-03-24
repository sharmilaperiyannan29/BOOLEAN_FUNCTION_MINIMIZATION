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
module ex2 (
   input A, B, C, D,
    output F
    
);
assign F= (~A & ~B & ~C & ~D) |
         ( A & ~C & ~D)      |
   		 (~B &  C & ~D)      |
   		 (~A &  B &  C &  D) |
   		 ( B & ~C &  D);
   		 
endmodule

Developed by:  Sharmila RegisterNumber:212225230261


**RTL realization**
![WhatsApp Image 2026-03-14 at 11 07 26 AM](https://github.com/user-attachments/assets/affe440c-60e9-4d7e-8a3b-6cc6fd5615c4)

**Output:**

**RTL**
![WhatsApp Image 2026-03-14 at 11 03 58 AM](https://github.com/user-attachments/assets/116cc150-d94e-4489-8dee-2dfff8c5f4d1)

**Timing Diagram**
![WhatsApp Image 2026-03-14 at 11 03 58 AM](https://github.com/user-attachments/assets/f9143e06-84bc-4b8a-8498-e52c022e0ee2)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

