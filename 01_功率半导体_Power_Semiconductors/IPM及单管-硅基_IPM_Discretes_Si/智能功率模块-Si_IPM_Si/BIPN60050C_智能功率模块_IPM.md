# 比亚迪半导体 (BYD) 家电级 IPM 智能功率模块 - BIPN60050C

[![Package](https://img.shields.io/badge/Package-DIP27--4426-blue.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BIPN60050C** 是一款高度集成的先进三相逆变智能功率模块 (IPM)。该模块结合了优化匹配的门极驱动与低损耗 IGBT 功率器件，并内置了全面的电路保护功能。由于采用了陶瓷覆铜板 (DBC) 和分立的负直流端子设计，产品在紧凑的体积下实现了优异的低热阻性能与独立的相电流监测。

### 🌟 核心特性 (Features)
* **高度集成**：600V / 50A 三相 IGBT 逆变全桥，内置自举二极管与高压集成电路 (HVIC)，实现单电源、无需光耦隔离的门极驱动能力。
* **全面保护**：集成控制电源及自举电路欠压闭锁保护 (UVLO)，以及低端（下桥）短路过流保护 (SCP)。
* **高效散热**：采用陶瓷覆铜板 (DBC) 材质基板，具备极低的热阻特性。
* **分立负端**：提供分立的三相直流负端 (Divided negative dc-link)，支持独立检测各相电流。
* **高绝缘性**：具备达 2500Vrms/min 的绝缘耐压等级。

### 🚗 典型应用 (Applications)
* 空调、洗衣机等变频家用电器 (Home appliances like air conditioner and washing machine)
* 小功率通用工业变频器 (Low-power inverter-driven applications)
* 伺服控制系统与小功率交流电机传动系统 (Servo control & Small power ac motor drive)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 功率端耐压 (V<sub>CES</sub>) | 逆变电流 (I<sub>C</sub>) | 绝缘等级 (V<sub>ISO</sub>) | 内置拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **BIPN60050C** | 600 V | 50 A | 2500 Vrms/min | 三相六管全桥 (Three-Phase Inverter) | DIP27-4426 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>J</sub> = 25 °C，除非另外注明）

### 1. 逆变器功率部分 (Inverter Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>PN</sub> | 电源电压 (Supply voltage) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 450 | V |
| V<sub>PN(surge)</sub> | 电源浪涌电压 (Supply voltage (surge)) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 500 | V |
| V<sub>CES</sub> | 集电极-发射极电压 (Collector-emitter voltage) | V<sub>GE</sub> = 0 V, I<sub>C</sub> = 100 μA | 600 | V |
| ± I<sub>C</sub> | 各 IGBT 集电极电流 (Each IGBT collector current) | T<sub>C</sub> = 25 °C | 50 | A |
| I<sub>CP</sub> | 晶圆集电极脉冲电流 (Each IGBT collector current (peak)) | T<sub>C</sub> = 25 °C, 脉宽 < 1 ms | 100 | A |
| P<sub>C</sub> | 集电极功耗 (Collector dissipation) | T<sub>C</sub> = 25 °C, 每一片小芯片 | 367 | W |
| T<sub>J</sub> | 结温 (Junction temperature) | 功率芯片极限最大结温限值（注 1） | -20 ~ +150 | °C |

> **注 1**：模块内集成的功率芯片最大结温额定值为 150 °C (@ T<sub>C</sub> ≤ 100 °C)。但在实际连续工作方案设计中，为了确保 IPM 的长期系统安全，平均结温建议限制在 T<sub>J</sub>(ave) ≤ 125 °C。

### 2. 控制与保护部分 (Control Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>D</sub> | 控制电源电压 (Control supply voltage) | 施加在 V<sub>D(HU)</sub>, V<sub>D(HV)</sub>, V<sub>D(HW)</sub>, V<sub>D(L)</sub> - COM 之间 | 20 | V |
| V<sub>DB</sub> | 高端控制辅助供电电压 (High-side bias voltage) | 施加在自举端 V<sub>B(U)</sub>-V<sub>S(U)</sub>, V<sub>B(V)</sub>-V<sub>S(V)</sub>, V<sub>B(W)</sub>-V<sub>S(W)</sub> | 20 | V |
| V<sub>IN</sub> | 信号输入电压 (Input voltage) | 施加在控制信号输入 IN 与 COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| V<sub>FO</sub> | 故障输出电压 (Fault output voltage) | 施加在 V<sub>FO</sub> - COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| I<sub>FO</sub> | 故障输出电流 (Fault output current) | 在 V<sub>FO</sub> 端子的最大允许灌电流 | 5.0 | mA |
| V<sub>CIN</sub> | 电流检测输入电压 (Current sensing input voltage) | 施加在 C<sub>IN</sub> - COM 采样端之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |

### 3. 自举二极管部分 (Bootstrap Diode Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>RRM</sub> | 最大重复反向电压 (Max. Repetitive Reverse Voltage) | 自举二极管耐压值 | 600 | V |
| I<sub>F</sub> | 正向直流电流 (Forward Current) | T<sub>C</sub> = 25 °C | 1 | A |
| I<sub>FP</sub> | 峰值正向脉冲电流 (Forward Current (Peak)) | T<sub>C</sub> = 25 °C, 脉宽 < 1 ms | 2 | A |
| T<sub>J</sub> | 自举二极管结温 (Junction temperature) | - | -20 ~ +150 | °C |

### 4. 整个系统特性 (Total System)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :---: | :--- | :---: | :---: |
| V<sub>PN(PROT)</sub> | 自保护电源电压限制 (短路保护供电限制) | V<sub>D</sub> = 13.5 ~ 16.5 V, T<sub>J</sub> = 125 °C, 非重复性短路, < 5 μs | 400 | V |
| T<sub>C</sub> | 模块壳体工作温度 (Module case operation temperature) | -20 °C ≤ T<sub>J</sub> ≤ 125 °C, 壳温检测位置详见尺寸图 | -20 ~ +100 | °C |
| T<sub>STG</sub> | 存储/保存温度 (Storage temperature) | - | -40 ~ +125 | °C |
| V<sub>ISO</sub> | 绝缘内部耐压 (Isolation voltage) | 60 Hz 正弦波，交流电压持续 1 分钟，所有连接引脚到散热片基板之间 | 2500 | Vrms |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 最大值 (Max.) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| R<sub>th(j-c)Q</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 IGBT 部分 (每 1/6 模块) | 0.34 | °C/W |
| R<sub>th(j-c)F</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 FRD 续流二极管部分 (每 1/6 模块) | 0.64 | °C/W |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. 逆变器功率部分 (Inverter Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数说明 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>CE(SAT)</sub> | 集电极-发射极饱和电压 | V<sub>D</sub> = V<sub>BS</sub> = 15 V, V<sub>IN</sub> = 5 V, I<sub>C</sub> = 50 A, T<sub>J</sub> = 25 °C | - | 1.8 | 2.2 | V |
| V<sub>F</sub> | FRD 正向导通电压 | V<sub>IN</sub> = 0 V, I<sub>C</sub> = 30 A, T<sub>J</sub> = 25 °C | - | 1.7 | 2.35 | V |
| I<sub>CES</sub> | 集电极-发射极间漏电流 | V<sub>CE</sub> = V<sub>CES</sub>, V<sub>GE</sub> = 0 V, T<sub>J</sub> = 25 °C | - | - | 0.1 | mA |

### 2. 开关动态损耗特性 (Switching Times, 感性负载测试)
测试条件：V<sub>PN</sub> = 300 V, V<sub>D</sub> = V<sub>BS</sub> = 15 V, I<sub>C</sub> = 50 A, V<sub>IN</sub> = 0 ↔ 5 V, T<sub>J</sub> = 25 °C（注 2）

| 驱动区域 | 符号 (Symbol) | 参数说明 (Parameter) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| **高端上桥臂**<br>(High-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 900 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 500 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 1050 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 200 | - | ns |
| **低端下桥臂**<br>(Low-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 900 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 660 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 1100 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 240 | - | ns |

> **注 2**：t<sub>ON</sub> 和 t<sub>OFF</sub> 包含了模块内部高低端驱动 IC 的传输延迟时间。而 t<sub>c(ON)</sub> 和 t<sub>c(OFF)</sub> 指的是在内部集成给定的驱动门极阻抗下，IGBT 晶圆本身的本征切换时间。

### 3. 控制与保护部分 (Control Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数名称 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| I<sub>DL</sub> | 低端低压供电静态电流 | V<sub>D</sub> = 15 V, IN<sub>(LU, LV, LW)</sub> = 0 V，V<sub>D(L)</sub> - COM | - | - | 600 | μA |
| I<sub>DH</sub> | 高端驱动每路静态电流 | V<sub>D</sub> = 15 V, IN<sub>(HU, HV, HW)</sub> = 0 V，每单相高压侧偏置 | - | - | 300 | μA |
| I<sub>QBS</sub> | 自举电路每路静态电流 | V<sub>BS</sub> = 15 V, IN<sub>(HU, HV, HW)</sub> = 0 V，高端悬浮回路 | - | - | 150 | μA |
| V<sub>FOH</sub> | 故障输出高电平电压 | V<sub>CIN</sub> = 0 V，故障引脚外接 4.7 kΩ 上拉到 5 V 电源 | 4.5 | - | - | V |
| V<sub>FOL</sub> | 故障输出低电平电压 | V<sub>CIN</sub> = 1 V，故障引脚外接 4.7 kΩ 上拉到 5 V 电源 | - | - | 0.8 | V |
| V<sub>CIN(ref)</sub> | 短路保护触发电压阈值 | T<sub>C</sub> = -20 ~ 100 °C, V<sub>D</sub> = 15 V（下桥 SCP 触发点，注 3）| 0.44 | 0.51 | 0.56 | V |
| UV<sub>DLD</sub> | 低端电源欠压检测电平 | 控制供电电源检测电平（电压下降脱扣） | 11.0 | 12.0 | 13.0 | V |
| UV<sub>DLR</sub> | 低端电源欠压复位电平 | 控制供电电源迟滞复位电平（电压回升恢复） | 12.0 | 13.0 | 14.0 | V |
| UV<sub>BSD</sub> | 高端自举电路欠压检测 | 自举浮动供电监测（电压下降脱扣） | 9.0 | 10.0 | 11.0 | V |
| UV<sub>BSR</sub> | 高端自举电路欠压复位 | 自举浮动供电监测（电压回升恢复） | 10.0 | 11.0 | 12.0 | V |
| t<sub>FO</sub> | 故障输出脉冲宽度 | 供电电路欠压保护或短路保护 | 50 | - | - | μs |
| V<sub>IN(ON)</sub> | 控制信号导通阈值电压 | 输入高电平有效（逻辑由低到高） | - | - | 3.0 | V |
| V<sub>IN(OFF)</sub> | 控制信号关断阈值电压 | 输入低电平有效（逻辑由高到低） | 0.8 | - | - | V |

> **注 3**：短路/过流保护功能仅在模块的**低端下桥臂**驱动电路中有效。

### 4. 自举二极管电气特性 (Bootstrap Diode)

| 符号 (Symbol) | 参数名称 (Parameter) | 测试条件 (Conditions) | 典型值 (Typ.) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>F</sub> | 二极管正向导通电压 | I<sub>F</sub> = 1 A, T<sub>J</sub> = 25 °C | 24.7 | V |
| t<sub>rr</sub> | 反向恢复时间 | I<sub>F</sub> = 1 A, T<sub>J</sub> = 25 °C | 130 | ns |

---

## 🔩 机械特性与额定机械值 (Mechanical Characteristics)

| 符号 (Symbol) | 参数与测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 (Units) |
| :--- | :--- | :---: | :---: | :---: | :---: |
| 安装扭矩 | 紧固安装螺钉：M3 规格螺丝螺纹（推荐选择稳定力矩：0.62 N·m） | 0.51 | 0.62 | 0.72 | N·m |
| 重量 (Weight) | 模块整体产品克重 | - | 15 | - | g |
| 器件平面度 | 模块背板 DBC 陶瓷平面翘曲平面度控制范围要求 | 0 | - | 120 | μm |

---

## 📈 推荐工作条件 (Recommended Operating Conditions)

| 符号 (Symbol) | 参数名称 (Parameter) | 推荐测试/应用条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>PN</sub> | 电源主干电压 | 施加在主变频端子 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | - | 300 | 400 | V |
| V<sub>D</sub> | 低端控制电源电压 | 施加在下桥偏置电源 V<sub>D(L)</sub> - COM 之间 | 13.5 | 15.0 | 16.5 | V |
| V<sub>BS</sub> | 高端悬浮供电电压 | 施加在高端自举控制端子驱动回路两端 | 13.5 | 15.0 | 18.5 | V |
| Δ V<sub>D</sub>, Δ V<sub>DB</sub>| 控制电压动态波动率 | 供电电平的动态瞬态电压变化波动范围（防止误触发）| -1 | - | 1 | V/μs |
| t<sub>DEAD</sub> | 桥臂互锁防直通死区 | 作用于控制 MCU 侧输出的同桥臂上下两路 PWM 信号互锁死区时间限制 | 2.0 | - | - | μs |
| f<sub>PWM</sub> | PWM 调制载波频率 | 系统推荐开关载波工作范围，-20 °C ≤ T<sub>J</sub> ≤ 125 °C, T<sub>C</sub> ≤ 100 °C| - | - | 20 | kHz |
| V<sub>SEN</sub> | 电流检测采样输出电压 | 施加在负端采样电阻端子 N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> - COM 之间（含允许纹波浪涌）| -4 | - | 4 | V |

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Package) | 每料管装数 (pcs/tube) | 每内盒料管数 (tube/inner box) | 每箱内盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| 抗静电料管 (Tube) | 10 | 7 | 5 | 350 |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
