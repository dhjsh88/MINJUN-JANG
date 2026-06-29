
## FC Accelerator on FPGA

### Overview
8-bit Fully Connected layer accelerator 
implemented on Xilinx FPGA using AXI4-Lite interface

### Architecture
- 4-core parallel MAC units
- Dual BRAM (node / weight)
- FSM-based data mover
- AXI4-Lite slave for PS-PL communication

### Verification
- C golden model vs RTL simulation comparison
- Tested with 4096-depth random input (srand)

### What I learned
- FSM design with read/write pipeline separation
- BRAM timing (1-cycle read latency compensation)
- AXI4-Lite register map design
- HW/SW co-verification methodology
