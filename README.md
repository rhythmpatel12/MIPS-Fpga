# MIPS-Fpga
## Implementation of a Microprocessor without Interlocked Pipelined Stages (MIPS) Architecture using VHDL on Basys3
The MIPS architecture is a reduced instruction set computing (RISC) architecture, known for its simplicity and efficiency. This project implements a subset of the MIPS instruction set, focusing on core instructions that demonstrate the capabilities of the architecture. The implementation is tailored for the Basys3 FPGA board, leveraging its features to simulate the MIPS processor's operation.
### Implemented MIPS Architecture
![image](https://github.com/rhythmpatel12/MIPS-Fpga/assets/77693221/3482f024-30b8-434f-8fee-41ad73273dd9)

### Test Bench Results
![image](https://github.com/rhythmpatel12/MIPS-Fpga/assets/77693221/024cdff5-cb7a-45e6-9d93-4426adc31358)
For the test above, multiple commands were tested for the MIPS instruction set.
-The first instruction was Addi Instruction to put in the value 0x10 into $t1 (x0010)
-The second instruction was Addi Instruction to put in the value 0x20 into $t0 (x0020)
-The third instruction was $t1 and $t0 being added and stored to $t2 (x0030)
-The fourth instruction was $t0 and $t1 being subtracted and stored to $t4 (x0010)
-The fifth instruction was $t1 and $t0 being multiplied and stored to $t2 (0x200)
-The sixth instruction was Addi Instruction to put in the value 0x04 into $t0 (x0004)
-The seventh instruction was a left logical shift where $t1 was shifted by the amount in $t0
and then the result was stored in $t2 (0x0100)

The eighth instruction was a right arithmetic shift where $t1 was shifted by the amount in
$t0 and then the result was stored in $t2 (0x0001)

![image](https://github.com/rhythmpatel12/MIPS-Fpga/assets/77693221/688e9a06-f3f5-4085-bbe2-3c05fb553e7b)
The final number that was obtained in the simulation was 0x37 which is 55 in decimal and is the
10th unique number in the fibonacci sequence by order. All the fibonacci numbers were also
stored in the memory after they were calculated using the store word functionality.
