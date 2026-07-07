# 比亚迪半导体 (BYD) 家电级 IPM 智能功率模块 - BIPE60030G-TD

[![Package](https://img.shields.io/badge/Package-BIP25--3824-blue.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BIPE60030G-TD** 是一款集成度极高的超小型封装三相逆变智能功率模块 (IPM)。该模块采用先进设计，在极度紧凑的封装内实现了优化匹配的门极驱动与低损耗 IGBT 功率器件，并内置了全面的电路保护功能。由于采用了陶瓷覆铜板 (DBC) 和分立的负直流端子设计，产品在超小体积下实现了优异的低热阻性能与独立的相电流监测，同时内置温度模拟电压输出功能。

### 🌟 核心特性 (Features)
* **高度集成**：600V / 30A 三相 IGBT 逆变全桥，内置自举二极管与高压集成电路 (HVIC)，实现单电源、无需光耦隔离的门极驱动能力。
* **全面保护**：集成控制电源及自举电路欠压闭锁保护 (UVLO)，以及低端（下桥）短路过流保护 (SCP) 和过温保护。
* **高效散热**：采用陶瓷覆铜板 (DBC) 材质基板，具备低热阻特性。
* **分立负端**：提供分立的三相直流负端 (Divided negative dc-link)，支持独立检测各相电流。
* **温度输出**：内置 LVIC 温度模拟电压输出功能，支持实时温度监测。

### 🚗 典型应用 (Applications)
* 空调、洗衣机等变频家用电器 (Home appliances like air conditioner and washing machine)
* 小功率通用工业变频器 (Low-power inverter-driven applications)
* 伺服控制系统与小功率交流电机传动系统 (Servo control & Small power ac motor drive)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 功率端耐压 (V<sub>CES</sub>) | 逆变电流 (I<sub>C</sub>) | 绝缘等级 (V<sub>ISO</sub>) | 内置拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **BIPE60030G-TD** | 600 V | 30 A | 1500 Vrms/min | 三相六管全桥 (Three-Phase Inverter) | BIP25-3824 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>J</sub> = 25 °C，除非另外注明）

### 1. 逆变器功率部分 (Inverter Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>PN</sub> | 电源电压 (Supply voltage) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 450 | V |
| V<sub>PN(surge)</sub> | 电源浪涌电压 (Supply voltage (surge)) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 500 | V |
| V<sub>CES</sub> | 集电极-发射极电压 (Collector-emitter voltage) | V<sub>GE</sub> = 0 V, I<sub>C</sub> = 0.1 mA, T<sub>J</sub> = 25 °C | 600 | V |
| ± I<sub>C</sub> | 各 IGBT 集电极电流 (Each IGBT collector current) | T<sub>C</sub> = 25 °C | 30 | A |
| I<sub>CP</sub> | 晶圆集电极脉冲电流 (Each IGBT collector current (peak)) | T<sub>C</sub> = 25 °C, 脉宽 < 1 ms | 60 | A |
| P<sub>C</sub> | 集电极功耗 (Collector dissipation) | T<sub>C</sub> = 25 °C, 每一片小芯片 | 83 | W |
| T<sub>J</sub> | 结温 (Junction temperature) | 功率芯片极限最大结温限值（注 1） | -40 ~ +150 | °C |

> **注 1**：模块内集成的功率芯片最大结温额定值为 150 °C (@ T<sub>C</sub> ≤ 100 °C)。但在实际连续工作方案设计中，为了确保 IPM 的长期系统安全，平均结温建议限制在 T<sub>J</sub>(ave) ≤ 125 °C。

### 2. 控制与保护部分 (Control Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>D</sub> | 控制电源电压 (Control power supply voltage) | 施加在 V<sub>D(H)</sub>-COM(H), V<sub>D(L)</sub>-COM(L) 之间 | -0.3 ~ 20 | V |
| V<sub>DB</sub> | 高端控制辅助供电电压 (High side control supply voltage) | 施加在 V<sub>B(U)</sub>-U, V<sub>B(V)</sub>-V, V<sub>B(W)</sub>-W 之间 | -0.3 ~ 20 | V |
| V<sub>IN</sub> | 信号输入电压 (Input voltage) | 施加在控制信号输入 IN 与 COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| V<sub>FO</sub> | 故障输出电压 (Fault output voltage) | 施加在 V<sub>FO</sub> - COM(L) 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| I<sub>FO</sub> | 故障输出电流 (Fault output current) | 在 V<sub>FO</sub> 端子的最大允许灌电流 | 8 | mA |
| V<sub>CIN</sub> | 电流检测输入电压 (Current sensing input voltage) | 施加在 C<sub>IN</sub> - COM(L) 采样端之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |

### 3. 整个系统特性 (Total System)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :---: | :--- | :---: | :---: |
| V<sub>PN(PROT)</sub> | 自保护电源电压限制 (短路保护供电限制) | V<sub>D</sub> = 13.5 ~ 16.5 V, T<sub>J</sub> = 125 °C, 非重复性短路, < 5 μs | 400 | V |
| T<sub>C</sub> | 模块壳体工作温度 (Module case operation temperature) | -40 °C ≤ T<sub>J</sub> ≤ 150 °C | -40 ~ +125 | °C |
| T<sub>STG</sub> | 存储/保存温度 (Storage temperature) | （注 2） | -40 ~ +125 | °C |
| V<sub>ISO</sub> | 绝缘内部耐压 (Isolation voltage) | 60 Hz 正弦波，交流电压持续 1 分钟，所有连接引脚到散热器之间 | 1500 | Vrms |

> **注 2**：推荐的模块贮存温度和湿度分别为 5 ~ 35 °C 和 45 ~ 75%。

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 最大值 (Max.) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| R<sub>th(j-c)Q</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 IGBT 部分 (每 1/6 模块) | 1.5 | °C/W |
| R<sub>th(j-c)F</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 FRD 续流二极管部分 (每 1/6 模块) | 2.2 | °C/W |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. 逆变器功率部分 (Inverter Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数说明 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>CE(SAT)</sub> | 集电极-发射极饱和电压 | V<sub>D</sub> = V<sub>BS</sub> = 15 V, V<sub>IN</sub> = 5 V, I<sub>C</sub> = 30 A, T<sub>J</sub> = 25 °C | - | 1.7 | 2.2 | V |
| V<sub>F</sub> | FRD 正向导通电压 | V<sub>IN</sub> = 0 V, I<sub>C</sub> = 30 A, T<sub>J</sub> = 25 °C | - | 1.8 | 2.3 | V |
| I<sub>CES</sub> | 集电极-发射极间漏电流 | V<sub>CE</sub> = V<sub>CES</sub>, V<sub>GE</sub> = 0 V, T<sub>J</sub> = 25 °C | - | - | 0.1 | mA |

### 2. 开关动态损耗特性 (Switching Times, 感性负载测试)
测试条件：V<sub>PN</sub> = 400 V, V<sub>D</sub> = V<sub>BS</sub> = 15 V, I<sub>C</sub> = 30 A, V<sub>IN</sub> = 0 ↔ 5 V, T<sub>J</sub> = 25 °C（注 3）

| 驱动区域 | 符号 (Symbol) | 参数说明 (Parameter) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| **高端上桥臂**<br>(High-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 770 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 280 | - | ns |
| | t<sub>rr</sub> | 反向恢复时间 (Reverse recovery time) | - | 110 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 860 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 98 | - | ns |
| **低端下桥臂**<br>(Low-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 940 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 340 | - | ns |
| | t<sub>rr</sub> | 反向恢复时间 (Reverse recovery time) | - | 115 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 890 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 110 | - | ns |

> **注 3**：t<sub>ON</sub> 和 t<sub>OFF</sub> 包含了模块内部高低端驱动 IC 的传输延迟时间。而 t<sub>c(ON)</sub> 和 t<sub>c(OFF)</sub> 指的是在内部集成给定的驱动门极阻抗下，IGBT 晶圆本身的本征切换时间。

### 3. 控制与保护部分 (Control Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数名称 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| I<sub>DL</sub> | 低端 VD 静态电流 | V<sub>D(L)</sub> = 15 V, IN<sub>(LU, LV, LW)</sub> = 0 V，V<sub>D(L)</sub> - COM(L) | - | 0.36 | 1.3 | mA |
| I<sub>DH</sub> | 高端 VD 静态电流 | V<sub>D(H)</sub> = 15 V, IN<sub>(HU, HV, HW)</sub> = 0 V，V<sub>D(HW)</sub> - COM(H) | - | 130 | 600 | μA |
| I<sub>QBS</sub> | 每相 VBS 静态电流 | V<sub>BS</sub> = 15 V, IN<sub>(HU, HV, HW)</sub> = 0 V，自举回路 | - | 75 | 150 | μA |
| V<sub>FOH</sub> | 故障输出高电平电压 | V<sub>CIN</sub> = 0 V，故障引脚外接 10 kΩ 上拉到 5 V 电源 | 4.9 | - | - | V |
| V<sub>FOL</sub> | 故障输出低电平电压 | V<sub>CIN</sub> = 1 V，故障引脚外接 10 kΩ 上拉到 5 V 电源 | - | - | 0.8 | V |
| V<sub>CIN(ref)</sub> | 短路保护触发电压阈值 | T<sub>C</sub> = -40 ~ 100 °C, V<sub>D</sub> = 15 V（注 4）| 0.455 | 0.48 | 0.505 | V |
| t<sub>cin_filter</sub> | 内部短路保护滤波时间 | Integrated filter | - | 400 | - | ns |
| T<sub>cin_Fo</sub> | 短路触发到 FO 故障输出延时 | Short circuit trip to FO output delay | 450 | 850 | 1050 | ns |
| UV<sub>DLD</sub> | 低端电源欠压检测电平 | 控制供电电源检测电平（电压下降脱扣） | 9.0 | 10.0 | 11.0 | V |
| UV<sub>DLR</sub> | 低端电源欠压复位电平 | 控制供电电源迟滞复位电平（电压回升恢复） | 10.0 | 11.0 | 12.0 | V |
| UV<sub>BSD</sub> | 高端自举电路欠压检测 | 自举浮动供电监测（电压下降脱扣） | 9.0 | 10.0 | 11.0 | V |
| UV<sub>BSR</sub> | 高端自举电路欠压复位 | 自举浮动供电监测（电压回升恢复） | 10.0 | 11.0 | 12.0 | V |
| t<sub>FO</sub> | 故障输出脉冲宽度 | - | 40 | - | - | μs |
| V<sub>OT</sub> | 温度输出电压 | LVIC T<sub>J</sub> = 90 °C | 2.63 | 2.77 | 2.91 | V |
| | | LVIC T<sub>J</sub> = 25 °C | 0.88 | 1.13 | 1.39 | V |
| T<sub>SD</sub> | 过温保护 | V<sub>D(L)</sub> = 15 V，检测 LVIC 温度 | 100 | 120 | 140 | °C |
| R<sub>BS(ON)</sub> | 自举二极管限流电阻 | BS driver ON resistance | - | - | 30 | Ω |
| V<sub>IN(ON)</sub> | 导通阈值电压 | HIN | - | 2.1 | 2.5 | V |
| | | LIN | - | 1.9 | 2.5 | V |
| V<sub>IN(OFF)</sub> | 关断阈值电压 | HIN | 0.8 | 1.1 | - | V |
| | | LIN | 0.8 | 1.4 | - | V |
| R<sub>IN</sub> | 输入下拉电阻 | HIN | 6 | 8 | 10 | kΩ |
| | | LIN | 6 | 7.7 | 11 | kΩ |

> **注 4**：短路/过流保护和过温保护功能仅在模块的**低端下桥臂**驱动电路中有效。

---

## 🔩 机械特性与额定机械值 (Mechanical Characteristics)

| 符号 (Symbol) | 参数与测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 (Units) |
| :--- | :--- | :---: | :---: | :---: | :---: |
| 安装扭矩 | 紧固安装螺钉：M3 规格螺丝螺纹（推荐选择稳定力矩：0.62 N·m） | 0.5 | 0.62 | 0.8 | N·m |
| 重量 (Weight) | 模块整体产品克重 | - | 9.3 | - | g |
| 器件平面度 | 模块背板 DBC 陶瓷平面翘曲平面度控制范围要求 | - | - | 100 | μm |

---

## 📈 推荐工作条件 (Recommended Operating Conditions)

| 符号 (Symbol) | 参数名称 (Parameter) | 推荐测试/应用条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>PN</sub> | 电源主干电压 | 施加在主变频端子 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | - | 300 | 400 | V |
| V<sub>D</sub> | 控制电源电压 | 施加在 V<sub>D(H)</sub>-COM(H), V<sub>D(L)</sub>-COM(L) 之间 | 13.5 | 15.0 | 16.5 | V |
| V<sub>DB</sub> | 高端控制辅助供电电压 | 施加在 V<sub>B(U)</sub>-U, V<sub>B(V)</sub>-V, V<sub>B(W)</sub>-W 之间 | 13.5 | 15.0 | 18.5 | V |
| Δ V<sub>D</sub>, Δ V<sub>DB</sub>| 控制电压动态波动率 | 供电电平的动态瞬态电压变化波动范围 | -1 | - | 1 | V/μs |
| t<sub>DEAD</sub> | 桥臂互锁防直通死区 | 作用于控制 MCU 侧输出的同桥臂上下两路 PWM 信号互锁死区时间限制 | 1.0 | - | - | μs |
| f<sub>PWM</sub> | PWM 调制载波频率 | 系统推荐开关载波工作范围 | - | - | 20 | kHz |
| V<sub>SEN</sub> | 电流检测采样输出电压 | 施加在负端采样电阻端子 N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> - COM(L) 之间（含允许纹波浪涌）| -4 | - | 4 | V |

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Package) | 每料管装数 (pcs/tube) | 每内盒料管数 (tube/inner box) | 每箱内盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| 抗静电料管 (Tube) | 12 | 6 | 5 | 360 |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
