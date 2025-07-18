# DESIGN AND IMPLEMENTATION OF 1X3 ROUTER

This RTL Design of the Project was completed and verified using Testbench Code.
It contains RTL Implementation of a basic Router1x3 (Single Ingress, 3 Egress Ports).
It is designed accepts data packets on a single 8-bit port and routes them to one of the three output ports.

**Router 1x3 Block Diagram:**
![image](https://github.com/user-attachments/assets/d53d4cd9-902d-4a79-8db6-d024270bb7cf)


**Functionality:**
1. Input Register:
    This block is responsible for extracting the header, calculating and checking the
    parity.
2. Synchronizer:
    This block is responsible for decoding the header and determining the output portIt also provides synchronization between FSM and FIFO Modules. It allows faithful communication between the input port and the output port.
3. FSM:
    This block is basically a controller for the router. It generates necessary controls for FIFO, Synchroniser based on the values of status signals.
4. FIFO:
    This is an synchronous active low reset FIFO which allows simultaneous read and write operations.

Steps covered during the project:
  1. Designed a the block level structure for the Router.
  2. Implemented the RTL Design using Verilog HDL and verified using individual verilog testbenches.
  3. Synthesized and Implemented the design to generate a bit file and tested on FPGA.
  4. Generated functional and code coverage for the RTL verification sign-off.# DESIGN-OF-3X1-ROUTER
