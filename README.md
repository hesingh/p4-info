## GOAL
This page is created for newcomers to P4 who ask for "what hardware can one use to prototype P4 code?"

## Terminology 

(a) A hardware target is a switching asic, FPGA, NPU, or generic compute.  
(b) A hardware platform is a switch (using asic), smartNIC (using FPGA or NPU), or server/laptop machine. 

## List
The list covers hardware targets and platforms supporting P4-16 in abphabetical order.  Supporting p4 entails the target supports a p4c (P4 compiler) backend.  A hardware target is useles without a P4 compiler (p4c) - therefore compiler vendors are also listed.  Lastly, a target that only supports p4runtime is not included.

For FPGA, Xilinx provides their P4 programming tools chain.  There is also Netcope who has a tools chain for P4 programming FPGA from Intel and Xilinx.

###
1. Barefoot Networks Tofino/Tofino2 asic in ODM switches - some ODM vendors are Edgecore (https://www.edge-core.com/), Netberg (https://netbergtw.com/about/), Inventec (https://www.inventec.com/english/indexEN.htm), Delta, WNC (http://www.wnc.com.tw/mobile/index.php?action=product_detail&top_id=28&scid=31&tid=99&lid=99&id=353), and Foxconn.  Stordis and Kaloom use ODM switches with open or proprietary switch OS. 

   Sample P4-16 programs for Tofino are at this repo: https://github.com/barefootnetworks/Open-Tofino.

2. Open-source P4 compiler (p4c) has a P4 to DPDK backend: https://github.com/p4lang/p4c/tree/master/backends/dpdk
   Please read the README.md file at the above link to learn how to generate DPDK .spec file using the compiler.

3. Mellanox has Spectrum/Spectrum2 asic. Their switches are SN2100, SN2700 (Spectrum) and SN3700 (Spectrum 2).  Their Linux switch uses TC.  Mellanox has a p4c with front-end and mid-end using open-source p4lang/p4c.  Mellanox has a p4c backend they plan to open source (as soon as we get it modularized from our common backend infra). Marian presented this at this year's netdev conference. https://www.netdevconf.org/0x13/session.html?p4-compiler-backend-for-tc

4. Netcope : https://www.intel.com/content/www/us/en/programmable/solutions/partners/partner-profile/netcope-technologies--a-s-.html.  Has tools chain to program FPGA with P4 (p4-16)

5. Netronome NIC using NPU - has p4 compiler.  https://www.netronome.com/products/datapath-programming-tools/
Update, 04/07/2021: Netronome has closed its California Bay Area office.  Try shopping for Intel/Xilinx NIC which support P4.

6. Orange: Has a p4c backend for linux user space.  See https://github.com/P4-Research/p4c/tree/master/backends/ubpf

7. Pensando has a service card that goes into a PCI slot of a computing machine.  Also, see https://p4.org/p4/pensando-joins-p4.html

8. p4lang/p4c EBPF (Enhanced Berkeley Packet Filter).  EBPF runs inside Linux kernel.  https://github.com/p4lang/p4c/tree/master/backends/ebpf

9. Xilinx FPGA with P4 compiler.  https://www.xilinx.com/support/documentation-navigation/development-tools/software-development/sdnet.html

10. Development platform for $100.  See  https://northboundnetworks.com/collections/zodiac-fx and https://github.com/NorthboundNetworks/p4c-zodiacfx.  The platform converts P4 to C.

Specifically, no openwrt access point implementation for P4 exists.
 
