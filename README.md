# AIM: 
To simulate and synthesis JK flipflop  using vivado. 
# APPARATUS REQUIRED: 
vivado 2023.2 software. 
# PROCEDURE: 
STEP:1 Start the vivado software, Select and Name the New project. 
STEP:2 Select the device family, device, package and speed. 
STEP:3 Select new source in the New Project and select Verilog Module as the 
Source type. 
STEP:4 Type the File Name and module name and Click Next and then finish 
button. Type the code and save it. 
STEP:5 Select the run simulation and then run Behavioral Simulation in the 
Source Window and click the check syntax. 
STEP:6 Click the simulation to simulate the program and give the inputs and 
verify the outputs as per the truth table. 
STEP:7 compare the output with truth table.
# JK_FLIPFLOP
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/094e9d55-5f30-4984-90b9-dd51d5297974)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/5b973ee8-9ee2-402d-8cba-1adfa2e4d5f2)
# Truth Table
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/04d4ff52-ae20-4e08-bd70-58137b129890)
# verilog code
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
# output
![image](https://github.com/lathika024/JK_FLIPFLOP/assets/165888553/7e1db144-1e0d-4189-9809-257fa78ca300)
# result
thus the JK flipflop is verified successfully 
