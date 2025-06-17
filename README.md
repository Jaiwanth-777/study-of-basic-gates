### Study-of-Basic-Gates ###

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.


**Equipments Required:**

Software – Quartus prime 


**Theory:**

Introduction-
Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate


**AND gate:**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B


**OR gate:** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B


**NOT gate:**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'


**NAND gate:**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’


**NOR gate:**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’


**Ex-OR gate:**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B


**Ex-NOR gate:**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B


**Procedure:** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.



**Logic Symbols & Truthtable:**

![image](https://github.com/user-attachments/assets/aa6af191-1b7f-4f97-b7df-8d3362fe3adc)


![image](https://github.com/user-attachments/assets/572b42af-3729-4c38-bbce-c59b075515b5)



**PROGRAM:**

Program for logic gates and verify its truth table in quartus using Verilog programming.

 Developed by: Jaiwanth M
 
 RegisterNumber: 212224040125



 ```
module log_ga(a, b, c1, c2, c3, c4, c5, c6, c7);
    input a, b;
    output c1, c2, c3, c4, c5, c6, c7;
    assign c1 = ~a;
    assign c2 = a & b;
    assign c3 = a | b;
    assign c4 = ~(a & b);
    assign c5 = ~(a | b);
    assign c6 = a ^ b;
    assign c7 = ~(a ^ b);
endmodule
```


 
**RTL:**

<img width="683" alt="EXP 1 DE" src="https://github.com/user-attachments/assets/ed4ed740-80a2-49f4-864e-591c4f2f08ea" />



**TIMING WAVEFORM:**

<img width="960" alt="EXP 1 DE {WAVEFORM}" src="https://github.com/user-attachments/assets/e2d26a5c-8980-4f14-aeb4-0f17767f7411" />



**Result:**

The truth table of logic gates in Quartus II verified and studied using Verilog programming.

