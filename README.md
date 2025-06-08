### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

step1: Define the Module and Ports – Create a Verilog module with an 8-bit input and a 3-bit output.

step2: Implement Dataflow Logic – Use continuous assign statements to encode the highest-priority bit into a 3-bit output.

step3: Create the Testbench – Write a testbench to apply different input values and observe outputs.

step4: Simulate the Design – Run the simulation in a Verilog simulator like ModelSim or Vivado.

step5: Verify with the Functional Table – Compare the output values against the expected functional table.

step6: Validate the Results – Ensure the simulation matches the expected results and fix any errors.

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: 212224230118
*/
```hdl
module ex5(din,a,b,c);
input [0:7] din;
output a,b,c;
assign a=(din[4]|din[5]|din[6]|din[7]);
assign b=(din[2]|din[3]|din[6]|din[7]);
assign c=(din[1]|din[3]|din[5]|din[7]);
endmodule
```
## RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling

![Screenshot 2025-03-28 134731](https://github.com/user-attachments/assets/fe489d26-e4f7-47e4-a779-7716c73f523f)

## TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling

![Screenshot 2025-04-11 133711](https://github.com/user-attachments/assets/89f4f227-0551-472b-a656-4f53b7bd7fb7)

**RESULTS**

A designed  a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming.



