The list below covers several hardware targets supporting P4 in abphabetical order.  Supporting p4 entails the target supports a p4c (P4 compiler) backend.  Specifically, a target that only supports p4runtime is not included.

Cisco and Arista have switches running the Barefoot Tofino asic.

Barefoot Networks Tofino asic in ODM switches (supports p4-16).  Two ODM vendors are Edgecore and Netberg.  Stordis and Kaloom use ODM switches with open or proprietary switch OS. 

Intel has P4 to DPDK, supports p4-16: https://www.youtube.com/watch?v=uI29_q-SoPU

Netcope : https://www.netcope.com/en/products/netcopep4.  Has software tools to program FPGA with P4 (p4-16?)

Netronome NIC using NPU - has p4 compiler (supports p4-16).

Orange: Has a p4c backend for linux user space (supports p4-16).  See https://github.com/P4-Research/p4c/tree/master/backends/ubpf

p4lang/p4c EBPF (Enhanced Berkeley Packet Filter) (supports p4-16).  EBPF runs inside Linux kernel.

Xilinx FPGA with P4 compiler (supports p4-16?).



Specifically, no p4rt implementation for P4 exists.
 
