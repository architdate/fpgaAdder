# fpgaAdder
Lucid Code for a 1 bit full adder.

How the adder is being tested

A) Initialization of the inputs and outputs in the module box of FPGA:

The first 5 LED's are initialised for the 3 inputs (namely a,b,c) and the 2 outputs of sum and carry.
The a b and c variables are the outputs for the FPGA so that they can become inputs for the circuit.
The output sum and carry of the circuit goes to the FPGA.
3 switches (io_dip) were initialized to control the high and low for a, b and c.

B) Configuring locations on the IO shield

They are configured under buttons_led.ucf
format: NET "a" LOC = P74 | IOSTANDARD = LVTTL;
