# JK_FLIPFLOP
# Aim:

To simulate and synthesis JK flipflop using vivado.

# Apparatus Required:

vivado 2023.2 software.

# Procedure:

STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.
# Block Diagram:
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/094e9d55-5f30-4984-90b9-dd51d5297974)
# Circuit Diagram:
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/5b973ee8-9ee2-402d-8cba-1adfa2e4d5f2)
# Truth Table:
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/04d4ff52-ae20-4e08-bd70-58137b129890)
# Program:
module jkff(clk,j,k,rst,q );

input j,k,clk,rst;

output reg q;

always@(posedge clk)

begin

if(rst==1)

q=1'b0;

else

begin

case({j,k})

2'b00: q=q;

2'b01:q=1'b0;

2'b10:q=1'b1;

2'b11:q=~q;

endcase

end

end

endmodule
# Output:
![image](https://github.com/padhmapriya06/JK_FLIPFLOP/assets/160568779/266617fc-2ab7-4fde-bba2-bb82750651ae)

# Result:
Thus the verilog program for JK flipflop has been simulated and verified successfully.

