The list below covers several hardware targets supporting P4-16 in abphabetical order.  Supporting p4 entails the target supports a p4c (P4 compiler) backend.  Specifically, a target that only supports p4runtime is not included.

First, Cisco and Arista have switches running the Barefoot Tofino asic.  Second, for FPGA, Xilinx provides their P4 programming tools chain.  However, there is Netcope who has a tools chain for P4 programming of FPGA as well.

###
Barefoot Networks Tofino asic in ODM switches - two ODM vendors are Edgecore and Netberg.  Stordis and Kaloom use ODM switches with open or proprietary switch OS. 

Intel has P4 to DPDK: https://www.youtube.com/watch?v=uI29_q-SoPU

Netcope : https://www.netcope.com/en/products/netcopep4.  Has software tools to program FPGA with P4 (p4-16?)

Netronome NIC using NPU - has p4 compiler.

Orange: Has a p4c backend for linux user space.  See https://github.com/P4-Research/p4c/tree/master/backends/ubpf

p4lang/p4c EBPF (Enhanced Berkeley Packet Filter).  EBPF runs inside Linux kernel.

Xilinx FPGA with P4 compiler.



Specifically, no p4rt implementation for P4 exists.
 
