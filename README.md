# PCIE-FPGA

基于 PCI  Express 通信协议的航空总线数据收发板卡，系统包
含两路独立的 ARINC429 收发通道和 32 路离散量输入、32 路离散量输出接口，满
足了实验室测试时的绝大多数需求。板卡采用 Intel 公司生产的 Cyclone IV GX 系列
FPGA 芯片，利用其内部自带的 PCIe 硬 IP 核实现 PCIe 协议，编写自定义 IP 实现
ARINC429 数据收发逻辑，使用 Qsys 系统在 FPGA 内部实现 PCIe、离散量输入输
出、ARINC429 以及 DDR2 控制单元的互联。电脑端使用 WinDriver 软件设计板卡
驱动，基于 MFC 设计用户操作界面，完成对板卡的交互式操作。 
