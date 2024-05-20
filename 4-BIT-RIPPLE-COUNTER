# NAME:-adhl hameed Reg no:- 212223050002
# AIM:-
Simulate verilog HDL for 4 bit Ripple Carry Adder using Quartus II 
PROCEDURE:-
Step 1: Open Quartus II and Create a New Project
Launch Quartus II:

Open the Quartus II software.
Create a New Project:

Go to File > New Project Wizard.
Follow the steps to set the project directory and name (e.g., RippleCarryAdder).
Skip adding files initially.
Step 2: Create the Verilog Design File
Create a New Verilog File:

Go to File > New > Design Files > Verilog HDL File.
Save the file with a suitable name, such as ripple_carry_adder.v.
Write the Verilog Code for the 4-bit Ripple Carry Adder and Full Adder:

Type or paste the necessary Verilog code for the ripple carry adder.
Save the File:

Save your work by going to File > Save.
Step 3: Create a Testbench File
Create a New Verilog Testbench File:

Go to File > New > Design Files > Verilog HDL File.
Save the file as ripple_carry_adder_tb.v.
Write the Testbench Code:

Type or paste the Verilog testbench code that will simulate the operation of the 4-bit ripple carry adder.
Save the File:

Save your work by going to File > Save.
Step 4: Compile the Design
Add Files to Project:

Go to Project > Add/Remove Files in Project.
Add both ripple_carry_adder.v and ripple_carry_adder_tb.v to the project.
Set the Top-Level Entity:

Go to Assignments > Settings > General.
Set the top-level entity to your testbench module, ripple_carry_adder_tb.
Compile the Project:

Go to Processing > Start Compilation.
Wait for the compilation process to complete and ensure there are no errors.
Step 5: Set Up the Simulation
Open the Simulation Tool:

Go to Tools > Simulation > RTL Simulation.
Set Simulation Settings:

In the simulation settings, select Functional as the simulation type.
Ensure the correct testbench file is selected.
Step 6: Run the Simulation
Run the Simulation:

Click on Start or Run to begin the simulation.
The simulation waveform window will open.
View the Results:

In the waveform window, observe the output signals.
Verify that the outputs match the expected results.
Step 7: Analyze and Debug
Check Outputs:

Ensure the Sum and Carry outputs are correct for all input test vectors.
Use the Zoom and Cursor tools to inspect specific time points and transitions.
Debug if Necessary:

If the simulation results are not as expected, review your Verilog code and testbench for any errors.
Make corrections and recompile if necessary.
Save Simulation Results:
# PROGRAM
"
Program : 
module ripple_carry_adder_4bit (
    input [3:0] a, b,
    input cin,
    output [3:0] sum,
    output cout
);
    wire c1, c2, c3;

    full_adder fa0 (.a(a[0]), .b(b[0]), .cin(cin),  .sum(sum[0]), .cout(c1));
    full_adder fa1 (.a(a[1]), .b(b[1]), .cin(c1),   .sum(sum[1]), .cout(c2));
    full_adder fa2 (.a(a[2]), .b(b[2]), .cin(c2),   .sum(sum[2]), .cout(c3));
    full_adder fa3 (.a(a[3]), .b(b[3]), .cin(c3),   .sum(sum[3]), .cout(cout));
endmodule

Create a Testbench:

module testbench;
    reg [3:0] a, b;
    reg cin;
    wire [3:0] sum;
    wire cout;

    ripple_carry_adder_4bit rca (.a(a), .b(b), .cin(cin), .sum(sum), .cout(cout));

    initial begin
        // Apply test vectors
        a = 4'b0000; b = 4'b0000; cin = 0;
        #10;
        a = 4'b0001; b = 4'b0001; cin = 0;
        #10;
        a = 4'b0010; b = 4'b0010; cin = 1;
        #10;
        a = 4'b1111; b = 4'b1111; cin = 1;
        #10;
        $stop; // End simulation
    end
endmodule



Save the waveform results by going to File > Save As in the waveform viewer.
# RTL LOGIC DIAGRAM
![image](https://github.com/adhlhameed/adhl-hameed/assets/168260238/8715b46c-7ca4-4745-9b0a-51fb183e99a7)
# TIMING DIGRAMS
![image](https://github.com/adhlhameed/adhl-hameed/assets/168260238/d79a3dc4-4289-4eef-abb1-bc63fa9cca77)
# RESULTS



