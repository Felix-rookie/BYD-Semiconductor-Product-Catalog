# 比亚迪半导体 (BYD) 家电级 IPM 智能功率模块 - BIPN60020C

[![Package](https://img.shields.io/badge/Package-DIP27--4426-blue.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BIPN60020C** 是一款由比亚迪半导体设计开发的智能功率模块 (IPM)。该产品具有封装小、抗干扰能力强等特点，内部集成了欠压闭锁电路、过流保护电路、驱动电路以及与低损耗 IGBT 匹配的功率器件。内置高压集成电路 (HVIC) 可提供无需光耦隔离的单电源 IGBT 门极驱动能力，分立三相直流负端子支持独立监测逆变器各相电流，适用于结构紧凑、高效率的小功率交流电机驱动系统。

### 🌟 核心特性 (Features)
* **高度集成**：600V / 20A 三相 IGBT 逆变全桥，内置门极驱动与功率器件保护用控制 IC。
* **全面保护**：集成欠压闭锁保护 (UVLO) 与低端（下桥）过流/短路保护 (SCP)，提升系统可靠性。
* **高效散热**：采用陶瓷覆铜板 (DBC) 低热阻结构设计。
* **分立负端**：提供分立三相直流负端 (Divided negative dc-link)，支持各相电流独立检测。
* **单电源驱动**：内置高压集成电路 (HVIC) 和自举二极管，可采用单电源驱动方案。
* **高绝缘性**：具备达 2500Vrms/min 的绝缘耐压等级。

### 🚗 典型应用 (Applications)
* 空调、洗衣机等变频家用电器 (Home appliances like air conditioner and washing machine)
* 小功率变频器 (Low-power inverter-driven applications)
* 伺服控制系统 (Servo control systems)
* 小功率交流电机传动系统使用的三相逆变器 (Three-phase inverter drive for small power AC motor control)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 功率端耐压 (V<sub>CES</sub>) | 逆变电流 (I<sub>C</sub>) | 绝缘等级 (V<sub>ISO</sub>) | 内置拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **BIPN60020C** | 600 V | 20 A | 2500 Vrms/min | 三相六管全桥 (Three-Phase Inverter) | DIP27-4426 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>J</sub> = 25 °C，除非另外注明）

### 1. 逆变器功率部分 (Inverter Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>PN</sub> | 电源电压 (Supply voltage) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 450 | V |
| V<sub>PN(surge)</sub> | 电源浪涌电压 (Supply voltage (surge)) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 500 | V |
| V<sub>CES</sub> | 集电极-发射极电压 (Collector-emitter voltage) | V<sub>GE</sub> = 0 V, I<sub>C</sub> = 100 μA, T<sub>J</sub> = 25 °C | 600 | V |
| ± I<sub>C</sub> | 单颗 IGBT 集电极电流 (Each IGBT collector current) | T<sub>C</sub> = 25 °C | 20 | A |
| ± I<sub>CP</sub> | 单颗 IGBT 集电极脉冲电流 (Each IGBT collector current (peak)) | T<sub>C</sub> = 25 °C, 持续 1 ms 的脉冲宽度 | 40 | A |
| P<sub>C</sub> | 集电极功耗 (Collector dissipation) | T<sub>C</sub> = 25 °C, 每一片芯片 | 61 | W |
| T<sub>J</sub> | 结温 (Junction temperature) | 功率芯片极限最大结温限值（注 1） | -40 ~ +150 | °C |

> **注 1**：模块内集成的功率芯片最大结温额定值为 150 °C (@ T<sub>C</sub> ≤ 100 °C)。但为了确保 IPM 安全工作，平均结温建议限制在 T<sub>J</sub>(avg) ≤ 125 °C (@ T<sub>C</sub> ≤ 100 °C)。

### 2. 控制与保护部分 (Control Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>D</sub> | 控制电源电压 (Control supply voltage) | 施加在 V<sub>D(HU)</sub>, V<sub>D(HV)</sub>, V<sub>D(HW)</sub>, V<sub>D(L)</sub> - COM 之间 | 20 | V |
| V<sub>DB</sub> | 高端控制辅助供电电压 (High-side bias voltage) | 施加在 V<sub>B(U)</sub>-V<sub>S(U)</sub>, V<sub>B(V)</sub>-V<sub>S(V)</sub>, V<sub>B(W)</sub>-V<sub>S(W)</sub> 之间 | 20 | V |
| V<sub>IN</sub> | 输入电压 (Input voltage) | 施加在 IN(HU), IN(HV), IN(HW), IN(LU), IN(LV), IN(LW) - COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| V<sub>FO</sub> | 故障输出电压 (Fault output voltage) | 施加在 V<sub>FO</sub> - COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| I<sub>FO</sub> | 故障输出电流 (Fault output current) | 在 V<sub>FO</sub> 端子的最大允许灌电流 | 5.0 | mA |
| V<sub>CIN</sub> | 电流检测输入电压 (Current sensing input voltage) | 施加在 C<sub>IN</sub> - COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |

### 3. 自举二极管部分 (Bootstrap Diode Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>RRM</sub> | 最大重复反向电压 (Maximum Repetitive Reverse Voltage) | 自举二极管耐压值 | 600 | V |
| I<sub>F</sub> | 正向电流 (Forward Current) | T<sub>C</sub> = 25 °C | 1 | A |
| I<sub>FP</sub> | 正向脉冲电流 (Forward Current (Peak)) | T<sub>C</sub> = 25 °C, 持续 1 ms 的脉冲宽度 | 2 | A |
| T<sub>J</sub> | 自举二极管结温 (Junction temperature) | - | -40 ~ +150 | °C |

### 4. 整个系统特性 (Total System)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :---: | :--- | :---: | :---: |
| V<sub>PN(PROT)</sub> | 自保护电源电压限制 (短路保护能力) | V<sub>D</sub> = 13.5 ~ 16.5 V, T<sub>J</sub> = 125 °C, 非重复性短路, 小于 5 Ωs | 400 | V |
| T<sub>C</sub> | 模块壳体工作温度 (Module case operation temperature) | -20 °C ≤ T<sub>J</sub> ≤ 125 °C | -20 ~ +100 | °C |
| T<sub>STG</sub> | 存储/保存温度 (Storage temperature) | - | -40 ~ +125 | °C |
| V<sub>ISO</sub> | 绝缘电压 (Isolation voltage) | 60 Hz 正弦波，交流电压持续 1 分钟，所有引脚与 DBC 之间 | 2500 | Vrms |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| R<sub>th(j-c)Q</sub> | 结点-壳体热阻 (Junction to case thermal resistance) | 逆变器 IGBT 部分 (每 1/6 模块) | - | - | 1.63 | °C/W |
| R<sub>th(j-c) F</sub> | 结点-壳体热阻 (Junction to case thermal resistance) | 逆变器 FRD 部分 (每 1/6 模块) | - | - | 2.48 | °C/W |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. 逆变器功率部分 (Inverter Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数说明 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>CE(SAT)</sub> | 集电极-发射极饱和电压 | V<sub>D</sub> = V<sub>BS</sub> = 15 V, V<sub>IN</sub> = 5 V, I<sub>C</sub> = 20 A, T<sub>J</sub> = 25 °C | - | 1.9 | 2.3 | V |
| V<sub>F</sub> | FRD 正向电压 | V<sub>IN</sub> = 0 V, I<sub>C</sub> = 15 A, T<sub>J</sub> = 25 °C | - | 1.7 | 2.2 | V |
| I<sub>CES</sub> | 集电极-发射极间漏电流 | V<sub>CE</sub> = V<sub>CES</sub>, V<sub>GE</sub> = 0 V, T<sub>J</sub> = 25 °C | - | - | 0.1 | mA |

### 2. 开关动态损耗特性 (Switching Times, 感性负载测试)
测试条件：V<sub>PN</sub> = 300 V, V<sub>D</sub> = V<sub>BS</sub> = 15 V, I<sub>C</sub> = 20 A, V<sub>IN</sub> = 0 ↔ 5 V, T<sub>J</sub> = 25 °C（注 2）

| 驱动区域 | 符号 (Symbol) | 参数说明 (Parameter) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| **高端上桥臂**<br>(High-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 800 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 250 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 1150 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 220 | - | ns |
| **低端下桥臂**<br>(Low-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 700 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 300 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 1150 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 220 | - | ns |

> **注 2**：t<sub>ON</sub> 和 t<sub>OFF</sub> 包含模块内部驱动集成电路 (IC) 的传输延迟时间。t<sub>c(ON)</sub> 和 t<sub>c(OFF)</sub> 指在内部给定的门极驱动条件下 IGBT 本身的切换时间。

### 3. 控制与保护部分 (Control Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数名称 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| I<sub>DL</sub> | V<sub>D</sub> 低端静态电流 (Quiescent V<sub>D</sub> supply current) | V<sub>D</sub> = 15 V, IN(LU, LV, LW) = 0 V，施加在 V<sub>D(L)</sub> - COM | - | - | 600 | μA |
| I<sub>DH</sub> | V<sub>D</sub> 高端静态电流 (Quiescent V<sub>D</sub> supply current) | V<sub>D</sub> = 15 V, IN(HU, HV, HW) = 0 V，施加在 V<sub>D(HU)</sub>, V<sub>D(HV)</sub>, V<sub>D(HW)</sub> - COM | - | - | 300 | μA |
| I<sub>QBS</sub> | V<sub>BS</sub> 静态电流 (Quiescent V<sub>BS</sub> supply current) | V<sub>BS</sub> = 15 V, IN(HU, HV, HW) = 0 V，施加在 V<sub>B(U)</sub>-V<sub>S(U)</sub>, V<sub>B(V)</sub>-V<sub>S(V)</sub>, V<sub>B(W)</sub>-V<sub>S(W)</sub> | - | - | 150 | μA |
| V<sub>FOH</sub> | 故障输出高电平电压 | V<sub>CIN</sub> = 0 V，V<sub>FO</sub> 电路 4.7 kΩ 上拉到 5 V | 4.5 | - | - | V |
| V<sub>FOL</sub> | 故障输出低电平电压 | V<sub>CIN</sub> = 1 V，V<sub>FO</sub> 电路 4.7 kΩ 上拉到 5 V | - | - | 0.8 | V |
| V<sub>CIN(ref)</sub> | 短路保护触发电压阈值 | T<sub>C</sub> = -20 ~ 100 °C, V<sub>D</sub> = 15 V （注 3） | 0.44 | 0.51 | 0.56 | V |
| UV<sub>DLD</sub> | 低端供电欠压检测电平 | 检测电平（低端） | 11.0 | 12.0 | 13.0 | V |
| UV<sub>DLR</sub> | 低端供电欠压复位电平 | 复位电平（低端） | 12.0 | 13.0 | 14.0 | V |
| UV<sub>BSD</sub> | 高端自举欠压检测电平 | 检测电平（高端） | 9.1 | 10.0 | 10.9 | V |
| UV<sub>BSR</sub> | 高端自举欠压复位电平 | 复位电平（高端） | 10.1 | 11.0 | 11.9 | V |
| t<sub>FO</sub> | 故障信号输出脉冲宽度 | C<sub>FO</sub> = 26 nF（注 4）<br>C<sub>FO</sub> = 33 nF（注 4） | -<br>- | 1.80<br>2.30 | -<br>- | ms |
| V<sub>IN(ON)</sub> | 导通阈值电压 | 施加在 IN(HU), IN(HV), IN(HW), IN(LU), IN(LV), IN(LW) - COM 之间 | - | - | 3.0 | V |
| V<sub>IN(OFF)</sub> | 关断阈值电压 | 施加在 IN(HU), IN(HV), IN(HW), IN(LU), IN(LV), IN(LW) - COM 之间 | 0.8 | - | - | V |

> **注 3**：短路保护功能仅在模块的**低端下桥臂**驱动电路中有效。
> **注 4**：故障信号输出脉冲宽度 t<sub>FO</sub> 依赖外接电容 C<sub>FO</sub> 的容值，其近似计算公式为：C<sub>FO</sub> ≈ 14.3 × 10<sup>-6</sup> × t<sub>FO</sub> [F]。

### 4. 自举二极管电气特性 (Bootstrap Diode)

| 符号 (Symbol) | 参数名称 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>F</sub> | 正向电压 (Forward Voltage) | I<sub>F</sub> = 1 A, T<sub>J</sub> = 25 °C | - | 24.7 | - | V |
| t<sub>rr</sub> | 反向恢复时间 (Reverse Recovery Time) | I<sub>F</sub> = 1 A, T<sub>J</sub> = 25 °C | - | 130 | - | ns |

---

## 🔩 机械特性与额定值 (Mechanical Characteristics and Ratings)

| 符号 (Symbol) | 参数与测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 (Units) |
| :--- | :--- | :---: | :---: | :---: | :---: |
| 安装扭矩 (Mounting torque) | 安装螺钉：M3，推荐选用 0.62 N·m | 0.51 | 0.62 | 0.72 | N·m |
| 重量 (Weight) | 模块整体产品克重 | - | 15 | - | g |
| 器件平面度 (Device flatness) | 参见封装平面度测量位置 | 0 | - | 120 | μm |

---

## 📈 推荐工作条件 (Recommended Operating Conditions)

| 符号 (Symbol) | 参数名称 (Parameter) | 推荐测试/应用条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>PN</sub> | 电源电压 (Supply voltage) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | - | 300 | 400 | V |
| V<sub>D</sub> | 控制电源电压 (Control supply voltage) | 施加在 V<sub>D(HU)</sub>, V<sub>D(HV)</sub>, V<sub>D(HW)</sub>, V<sub>D(L)</sub> - COM 之间 | 13.5 | 15.0 | 16.5 | V |
| V<sub>BS</sub> | 高端辅助供电电压 (High-side bias voltage) | 施加在 V<sub>B(U)</sub>-V<sub>S(U)</sub>, V<sub>B(V)</sub>-V<sub>S(V)</sub>, V<sub>B(W)</sub>-V<sub>S(W)</sub> 之间 | 13.5 | 15.0 | 18.5 | V |
| Δ V<sub>D</sub>, Δ V<sub>DB</sub> | 控制电源电压波动 (Control supply variation) | - | -1 | - | 1 | V/μs |
| t<sub>DEAD</sub> | 防止桥臂直通的死区时间 | 适用于每个输入信号 | 2.0 | - | - | μs |
| f<sub>PWM</sub> | PWM 输入信号 | -20 °C ≤ T<sub>C</sub> ≤ 100 °C, -20 °C ≤ T<sub>J</sub> ≤ 125 °C | - | - | 20 | kHz |
| V<sub>SEN</sub> | 电流检测产生的电压 | 施加在 N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> - COM 之间（包括浪涌电压） | -4 | - | 4 | V |

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Package) | 每料管装数 (pcs/tube) | 每内盒料管数 (tube/inner box) | 每箱内盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| 抗静电料管 (Tube) | 10 | 7 | 5 | 350 |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
