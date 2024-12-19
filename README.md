# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */
Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.
module de12(
input wire clk, // Clk input
output reg [3:0] count //4-bit counter output
);
// Counter logic
always @(posedge clk) begin
if (count ==4'b1111) // Reset when count reaches 15
    count <=4'b0000;
else 
    count <= count + 1; // Increment count
end
endmodule


 Developed by: S.NITHYASREE
 RegisterNumber:24900149
*/

**RTL LOGIC FOR 4 Bit Ripple Counter**

<img width="664" alt="lg12" src="https://github.com/user-attachments/assets/fb2bd808-c94a-471c-87ae-8acfdd92f2a2" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**

<img width="956" alt="wf12" src="https://github.com/user-attachments/assets/eb970746-7acd-4133-a624-bb9c49758751" />

**RESULTS**
Therefore 4-Bit-ripple-counter in always@ method using verilog and validating their functionally using their functional tables is verify.
