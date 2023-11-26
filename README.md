## Name : Ananda Rakshan K V

## Roll No : 23001531

# Experiment--02-Implementation of combinational logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
 
 
## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime


## Theory:
 
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

## Procedure:

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.

## Program:

module exp2(A,B,C,D,F1);

input A,B,C,D;

output F1;

wire x1,x2,x3,x4,x5;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign F1=x1|x2|x3|x4|x5;

endmodule

## RTL realization:
![RTL-exp2](https://github.com/anandarakshan/Experiment--02-Implementation-of-combinational-logic-/assets/139217934/a760755e-7a19-4daa-81ae-b6b56a74bb5a)


## Truth Table:

![Truth Table-exp2](https://github.com/anandarakshan/Experiment--02-Implementation-of-combinational-logic-/assets/139217934/01f54815-c131-4e30-b32b-d08e28ebc0b3)

## Timing Diagram:

![Wave diagram-exp2](https://github.com/anandarakshan/Experiment--02-Implementation-of-combinational-logic-/assets/139217934/a5db4157-4dfd-4bea-aa37-08ab92f36517)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
