# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

1.Open Quartus II and create a new project.

2.Use schematic design entry to draw the full adder and full subtractor circuit.

3.The circuit consists of XOR, AND, and OR gates.

4.Compile the design, verify its functionality through simulation.

5.Implement the design on the target device and program it.

**Program:**

/* Program to design a full adder and full subtractor circuit and verify its truth table in quartus using Verilog programming. 
Developed by: Karthick Raja k
RegisterNumber: 212223240066
*/

```
module Encoder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
//add logic here using dataflow modelling
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule
```
![Screenshot 2024-04-19 101426](https://github.com/Karthickraja23006120/FULL_ADDER_SUBTRACTOR/assets/139335315/4c92350e-1719-40b1-a0e5-dff874a8fea1)

**RTL Schematic**
![Screenshot 2024-04-19 101455](https://github.com/Karthickraja23006120/FULL_ADDER_SUBTRACTOR/assets/139335315/7fcf9ebc-7203-406e-aa5f-ed6a96662a58)

**Output Timing Waveform**
![Screenshot 2024-04-19 101523](https://github.com/Karthickraja23006120/FULL_ADDER_SUBTRACTOR/assets/139335315/5ac69443-100a-409e-9230-a949dc10c9f0)

**Result:**
Thus,the Encoder 8 To 3 in Dataflow Modelling using verilog has been implemented successfully and their functionality is validated using their functional tables.
Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



