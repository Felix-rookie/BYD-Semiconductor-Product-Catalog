# 比亚迪半导体 (BYD) 家电级 IPM 智能功率模块 - BIP60006B

[![Package](https://img.shields.io/badge/Package-DIP25--B--3215-blue.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BIP60006B** 是一款紧凑型全塑封智能功率模块 (IPM)。该产品内部集成高可靠性的高压栅极驱动电路，内置带限流电阻的自举二极管，集成欠压、过流和使能关断等保护功能，自带温度输出功能，提供了优异的保护和较宽的安全工作范围，是小功率白色家电的理想选择。由于采用了分立的负端子，可独立监测逆变器的每一相电流。

### 🌟 核心特性 (Features)
* **紧凑全塑封**：结构紧凑，全塑封设计，适合小功率应用
* **低损耗芯片**：采用低损耗 BYD IGBT 5.0 芯片
* **全面保护**：内置欠压保护、过流保护、使能关断功能和高低边输入互锁功能
* **温度输出**：内置温度电压输出功能
* **逻辑兼容**：输入高电平有效，兼容 3.3V、5V 电压
* **分立负端**：提供分立的三相直流负端，支持独立检测各相电流

### 🚗 典型应用 (Applications)
* 空调风机 (Air conditioning fan)
* 冰箱 (Refrigerator)
* 洗衣机 (Washing machine)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 功率端耐压 (V<sub>CES</sub>) | 逆变电流 (I<sub>C</sub>) | 绝缘等级 (V<sub>ISO</sub>) | 内置拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **BIP60006B** | 600 V | 6 A | 1650 Vrms/min | 三相六管全桥 (Three-Phase Inverter) | DIP25-B-3215 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>J</sub> = 25 °C，除非另外注明）

### 1. 逆变器功率部分 (Inverter Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>PN</sub> | 电源电压 (Supply voltage) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 450 | V |
| V<sub>PN(surge)</sub> | 电源浪涌电压 (Supply voltage (surge)) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 500 | V |
| V<sub>CES</sub> | 集电极-发射极电压 (Collector-emitter voltage) | V<sub>GE</sub> = 0 V, I<sub>C</sub> = 0.1 mA, T<sub>J</sub> = 25 °C | 600 | V |
| ± I<sub>C</sub> | 各 IGBT 集电极持续电流 (Each IGBT collector current) | T<sub>C</sub> = 25 °C, T<sub>J</sub> ≤ 150 °C | 6 | A |
| I<sub>CP</sub> | 晶圆集电极峰值电流 (Each IGBT collector peak current) | T<sub>C</sub> = 25 °C, T<sub>J</sub> ≤ 150 °C, 脉宽 < 1 ms | 12 | A |
| P<sub>C</sub> | 集电极功耗 (Collector dissipation) | T<sub>C</sub> = 25 °C, 每一片小芯片 | 21 | W |
| T<sub>J</sub> | 结温 (Junction temperature) | 功率芯片极限最大结温限值（注 1） | -40 ~ +150 | °C |

> **注 1**：模块内集成的功率芯片最大结温额定值为 150 °C (@ T<sub>C</sub> ≤ 100 °C)。但在实际连续工作方案设计中，为了确保 IPM 的长期系统安全，平均结温建议限制在 T<sub>J</sub>(ave) ≤ 125 °C。

### 2. 控制与保护部分 (Control Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>D</sub> | 控制电源电压 (Control supply voltage) | 施加在 V<sub>D(U)</sub>, V<sub>D(V)</sub>, V<sub>D(W)</sub> - COM 之间 | -0.3 ~ 20 | V |
| V<sub>BS</sub> | 高边控制电源电压 (High side control supply voltage) | 施加在 V<sub>B(U)</sub>-U, V<sub>B(V)</sub>-V, V<sub>B(W)</sub>-W 之间 | -0.3 ~ 20 | V |
| V<sub>IN</sub> | 信号输入电压 (Input voltage) | 施加在控制信号输入 IN 与 COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| V<sub>FO</sub> | 故障输出电压 (Fault output voltage) | 施加在 /FO,/SDW,VOT - COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| I<sub>FO</sub> | 故障输出电流 (Fault output current) | 在 /FO,/SDW,VOT 端子的最大允许灌电流 | 2 | mA |
| V<sub>CIN</sub> | 过流检测输入电压 (Over current sensing input voltage) | 施加在 C<sub>IN</sub> - COM 采样端之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |

### 3. 整个系统特性 (Total System)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :---: | :--- | :---: | :---: |
| V<sub>PN(PROT)</sub> | 自保护电源电压限制 (短路保护供电限制) | V<sub>D</sub> = 13.5 ~ 16.5 V, T<sub>J</sub> = 150 °C, 非重复性短路, < 5 μs | 400 | V |
| T<sub>C</sub> | 模块壳体工作温度 (Module case operation temperature) | -40 °C ≤ T<sub>J</sub> ≤ 150 °C | -40 ~ +125 | °C |
| T<sub>STG</sub> | 存储/保存温度 (Storage temperature) | - | -40 ~ +125 | °C |
| V<sub>ISO</sub> | 绝缘内部耐压 (Isolation voltage) | 60 Hz 正弦波，交流电压持续 1 分钟，所有连接引脚到 DBC 之间 | 1650 | Vrms |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 最大值 (Max.) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| R<sub>th(j-c)Q</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 IGBT 部分 (每 1/6 模块) | 5.8 | °C/W |
| R<sub>th(j-c)F</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 FRD 续流二极管部分 (每 1/6 模块) | 7.4 | °C/W |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. 逆变器功率部分 (Inverter Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数说明 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>CE(SAT)</sub> | 集电极-发射极饱和电压 | V<sub>D</sub> = V<sub>BS</sub> = 15 V, V<sub>IN</sub> = 5 V, I<sub>C</sub> = 6 A, T<sub>J</sub> = 25 °C | - | 1.7 | 2.2 | V |
| V<sub>F</sub> | FRD 正向导通电压 | V<sub>IN</sub> = 0 V, I<sub>F</sub> = 6 A, T<sub>J</sub> = 25 °C | - | 1.8 | 2.3 | V |
| I<sub>CES</sub> | 集电极-发射极间漏电流 | V<sub>CE</sub> = V<sub>CES</sub>, V<sub>GE</sub> = 0 V, T<sub>J</sub> = 25 °C | - | - | 0.1 | mA |

### 2. 开关动态损耗特性 (Switching Times, 感性负载测试)
测试条件：V<sub>PN</sub> = 300 V, V<sub>D</sub> = V<sub>BS</sub> = 15 V, I<sub>C</sub> = 6 A, V<sub>IN</sub> = 0 ↔ 5 V, T<sub>J</sub> = 25 °C（注 2）

| 驱动区域 | 符号 (Symbol) | 参数说明 (Parameter) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| **高边上桥臂**<br>(High-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 450 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 130 | - | ns |
| | t<sub>rr</sub> | 反向恢复时间 (Reverse recovery time) | - | 85 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 550 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 90 | - | ns |
| **低边下桥臂**<br>(Low-side) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 460 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 135 | - | ns |
| | t<sub>rr</sub> | 反向恢复时间 (Reverse recovery time) | - | 90 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 560 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 100 | - | ns |

> **注 2**：t<sub>ON</sub> 和 t<sub>OFF</sub> 包含了模块内部高低端驱动 IC 的传输延迟时间。而 t<sub>c(ON)</sub> 和 t<sub>c(OFF)</sub> 指的是在内部集成给定的驱动门极阻抗下，IGBT 晶圆本身的本征切换时间。

### 3. 控制与保护部分 (Control Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数名称 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| I<sub>QD</sub> | VD 静态电流 | V<sub>D(U,V,W)</sub> = 15 V, IN<sub>(HU,HV,HW,LU,LV,LW)</sub> = 0 V | - | - | 1.0 | mA |
| I<sub>QBS</sub> | VBS 静态电流 | V<sub>BS(U,V,W)</sub> = 15 V, IN<sub>(HU,HV,HW)</sub> = 0 V | - | - | 150 | μA |
| V<sub>CIN(ref)</sub> | 短路保护触发电压 | V<sub>D(U,V,W)</sub> = 15 V | 0.43 | 0.48 | 0.53 | V |
| UV<sub>DD</sub> | 低边电源欠压检测电平 | 控制供电电源检测电平（电压下降脱扣） | 9.0 | 10.0 | 11.0 | V |
| UV<sub>DR</sub> | 低边电源欠压复位电平 | 控制供电电源迟滞复位电平（电压回升恢复） | 10.0 | 11.0 | 12.0 | V |
| UV<sub>BSD</sub> | 高边自举电路欠压检测 | 自举浮动供电监测（电压下降脱扣） | 9.0 | 10.0 | 11.0 | V |
| UV<sub>BSR</sub> | 高边自举电路欠压复位 | 自举浮动供电监测（电压回升恢复） | 10.0 | 11.0 | 12.0 | V |
| I<sub>FO-T</sub> | 温度输出电流 | V<sub>D(W)</sub> = V<sub>B(W)</sub> = 15 V, T<sub>HVIC</sub> = 25 °C | - | 110 | - | μA |
| | | V<sub>D(W)</sub> = V<sub>B(W)</sub> = 15 V, T<sub>HVIC</sub> = 100 °C | - | 279 | - | μA |
| V<sub>FO-T</sub> | 温度输出电压 | V<sub>D(W)</sub> = V<sub>B(W)</sub> = 15 V, T<sub>HVIC</sub> = 25 °C, 6.8 kΩ to 5 V Pull-up | - | 4.25 | - | V |
| | | V<sub>D(W)</sub> = V<sub>B(W)</sub> = 15 V, T<sub>HVIC</sub> = 100 °C, 6.8 kΩ to 5 V Pull-up | - | 3.1 | - | V |
| t<sub>FO</sub> | 故障输出脉冲宽度 | - | 40 | - | - | μs |
| V<sub>FSDR</sub> | 使能关断复位电压 | 施加在 /FO-COM | - | - | 2.4 | V |
| V<sub>FSDD</sub> | 使能关断检测电压 | 施加在 /FO-COM | 0.8 | - | - | V |
| V<sub>IN(ON)</sub> | 控制信号导通阈值电压 | 施加在输入引脚与 COM 之间 | - | - | 3.0 | V |
| V<sub>IN(OFF)</sub> | 控制信号关断阈值电压 | 施加在输入引脚与 COM 之间 | 0.8 | - | - | V |
| R<sub>BS(ON)</sub> | 自举二极管限流电阻 | V<sub>D(U,V,W)</sub> = 15 V | - | 100 | - | Ω |

> **注 3**：短路/过流保护和过温保护功能仅在模块的**低边下桥臂**驱动电路中有效。

---

## 🔩 机械特性与额定机械值 (Mechanical Characteristics)

| 符号 (Symbol) | 参数与测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 (Units) |
| :--- | :--- | :---: | :---: | :---: | :---: |
| 安装扭矩 | 紧固安装螺钉：M3 规格螺丝螺纹（推荐选择稳定力矩：0.62 N·m） | 0.6 | 0.7 | 0.8 | N·m |
| 重量 (Weight) | 模块整体产品克重 | - | 3.9 | - | g |
| 器件平面度 | 模块背板 DBC 陶瓷平面翘曲平面度控制范围要求 | -50 | - | 100 | μm |

---

## 📈 推荐工作条件 (Recommended Operating Conditions)

| 符号 (Symbol) | 参数名称 (Parameter) | 推荐测试/应用条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>PN</sub> | 电源主干电压 | 施加在主变频端子 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | - | 300 | 400 | V |
| V<sub>D</sub> | 控制电源电压 | 施加在 V<sub>D(U)</sub>, V<sub>D(V)</sub>, V<sub>D(W)</sub> - COM 之间 | 13.5 | 15.0 | 16.5 | V |
| V<sub>BS</sub> | 高边控制电源电压 | 施加在 V<sub>B(U)</sub>-U, V<sub>B(V)</sub>-V, V<sub>B(W)</sub>-W 之间 | 13.5 | 15.0 | 18.5 | V |
| dV<sub>D</sub>/dt, dV<sub>BS</sub>/dt | 控制电压动态波动率 | 供电电平的动态瞬态电压变化波动范围 | -1 | - | 1 | V/μs |
| t<sub>DEAD</sub> | 桥臂互锁防直通死区 | 作用于控制 MCU 侧输出的同桥臂上下两路 PWM 信号互锁死区时间限制 | 1.0 | - | - | μs |
| f<sub>PWM</sub> | PWM 调制载波频率 | 系统推荐开关载波工作范围 | - | - | 20 | kHz |
| V<sub>SEN</sub> | 电流检测采样输出电压 | 施加在负端采样电阻端子 N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> - COM 之间（含允许纹波浪涌）| -4 | - | 4 | V |
| PW<sub>IN(ON)</sub> | 最小输入脉宽 (导通) | V<sub>D</sub> = V<sub>BS</sub> = 15 V | 0.7 | - | - | μs |
| PW<sub>IN(OFF)</sub> | 最小输入脉宽 (关断) | V<sub>D</sub> = V<sub>BS</sub> = 15 V | 0.7 | - | - | μs |

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Package) | 每料管装数 (pcs/tube) | 每内盒料管数 (tube/inner box) | 每箱内盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| 抗静电料管 (Tube) | 14 | 6 | 5 | 420 |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
