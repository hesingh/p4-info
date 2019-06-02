## Terminology 

(a) A hardware target is a switching asic, FPGA, or generic compute.  
(b) A hardware platform is a switch (using asic), smartNIC (using FPGA), or server/laptop machine. 

## List
The list covers hardware targets and platforms supporting P4-16 in abphabetical order.  Supporting p4 entails the target supports a p4c (P4 compiler) backend.  A hardware target is useles without a P4 compiler (p4c) - therefore compiler vendors are also listed.  Lastly, a target that only supports p4runtime is not included.

First, Cisco and Arista have switches running the Barefoot Tofino asic.  Second, for FPGA, Xilinx provides their P4 programming tools chain.  There is also Netcope who has a tools chain for P4 programming of FPGA from Intel and Xilinx.

###
1. Barefoot Networks Tofino asic in ODM switches - two ODM vendors are Edgecore and Netberg.  Stordis and Kaloom use ODM switches with open or proprietary switch OS. 

2. Intel has P4 to DPDK: https://www.youtube.com/watch?v=uI29_q-SoPU

3. Netcope : https://www.netcope.com/en/products/netcopep4.  Has tools chain to program FPGA with P4 (p4-16?)

4. Netronome NIC using NPU - has p4 compiler.

5. Orange: Has a p4c backend for linux user space.  See https://github.com/P4-Research/p4c/tree/master/backends/ubpf

6. p4lang/p4c EBPF (Enhanced Berkeley Packet Filter).  EBPF runs inside Linux kernel.

7. Xilinx FPGA with P4 compiler.



Specifically, no openwrt access point implementation for P4 exists.
 
