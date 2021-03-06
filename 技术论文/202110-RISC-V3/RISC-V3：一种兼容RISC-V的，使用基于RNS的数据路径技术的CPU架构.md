**【原创翻译】RISC-V3：一种兼容RISC-V的，使用基于RNS的数据路径技术的CPU架构**

**作者：MARC REICHENBACH , JOHANNES KNÖDTEL, SEBASTIAN RACHUJ, AND DIETMAR FEY**

**INSPEC 备案号：** 20738178                           **出版日期：** 2021 年 3 月 2 日                                **出版商：**IEEE

原文链接：https://ieeexplore.ieee.org/document/9366755

> **摘要**：RNS（Redundant Number Systems，冗余数字系统）是一种广为人知的算术运算电路加速技术。在CPU架构体系中，RNS仅被使用于子电路级别，例如在算术逻辑单元（ALU）内部实现除法。采用基于RNS的数据路径技术的CPU，可以解决ALU中的RNS和二进制之间的转换问题，在一定程度上实现了数据的高速处理。在本文中，作者提出了一种被称为RISC-V3的新型CPU架构，它与现有的RISC-V指令集兼容，但在内部使用了RNS数据处理方式，以加快指令执行时间，从而提高系统性能。RISC-V架构非常适用于RNS技术，因为它没有标志寄存器（标志寄存器在RNS技术下计算成本比较高）。为了直观感受到性能百分比的提升，本文实现的基于RNS的数据路径技术会在不同的半导体技术下。同时，也会使用指令集模拟器和基准测试套件（Embench）来评估系统性能。作者的试验结果显示，在基准测试和CMOS技术下，RISC-V3体系结构的性能，要比二进制体系结构高出81%。

**关键词**：算术和逻辑单元（ALU）、处理器结构、RISC、三进制算术

# 1、绪论

以前，为了构建高效和节能的计算机系统，且为了不局限于传统的二进制数据表示，而提出了一种基于冗余数字系统（RNS）技术的方法 [1]。这种数字系统，允许每个数位使用超过 *r*（> 1） 的数值。虽然这样的实现在硬件资源利用方面，尤其是数据存储方面，乍看效率很低，但是在实际使用这些数字时，可以渐进地、更快地执行基于字宽的算术运算。这种改进的原因是这种数字系统，实现了基于有限进位扩展的算术电路技术。

Parhami [2] 

# 2、RNS算法的电路设计





# 3、RISC-V3：一种三进制RISC-V体系结构





# 4、仿真模拟环境



# 5、评估



# 6、讨论和结论



# 参考文献

[1]

[2]

[3]

[4]

[5]

[6]

[7]

[8]

[9]

[10]

[11]

[12]

[13]

[14]

[15]

[16]

[17]

[18]

[19]

[20]

[21]

[22]

[23]

[24]

[25]

[26]

[27]

[28]

[29]

[30]

[31]

[32]

[33]

[34]

[35]

[36]

# 作者简介

**MARC REICHENBACH（马克 · 莱琛巴赫）**：2010年获得埃尔朗根-纽伦堡University（FAU）计算机科学文凭，2017年获得FAU博士学位。目前是FAU计算机体系结构学院的教授和博士后研究员，研究方向为新型计算机体系结构、忆阻计算技术和适用于不同应用领域的智能传感器体系结构。

**JOHANNES KNÖDTEL（约翰内斯 · 克纳德特尔）**：2016年获得埃尔朗根-纽伦堡University（FAU）计算机科学硕士学位，2017年开始担任FAU计算机体系结构学院的教授和科研人员，研究方向为处理器设计领域中不同层次抽象上的电路设计，以及忆阻技术相关的应用设计。

**SEBASTIAN RACHUJ（塞巴斯蒂安 · 拉丘伊）**：2015年获得埃尔朗根-纽伦堡University（FAU）计算机科学学士学位，2016年获得计算机体系结构系计算机科学专业硕士学位。自2016年以来，一直担任FAU计算机体系结构学院的科研人员，研究方向为基于异构系统仿真环境的提供不同速度和精度的不同处理器模拟方法

**DIETMAR FEY（迪特马尔 · 费伊）**：1992年获得埃尔朗根-纽伦堡University（FAU）计算机科学和计算机体系结构中光学技术的博士学位，并获得FAU的特级任教资格。1994至1999年间在FAU进行科学研究，1999年至2001年在Siegen University担任讲师，2001年开始担任FAU计算机工程教授。自2009年以来，担任FAU计算机体系结构学院的院长。他的研究方向包括并行计算机体系结构、编程环境、嵌入式系统和忆阻计算技术