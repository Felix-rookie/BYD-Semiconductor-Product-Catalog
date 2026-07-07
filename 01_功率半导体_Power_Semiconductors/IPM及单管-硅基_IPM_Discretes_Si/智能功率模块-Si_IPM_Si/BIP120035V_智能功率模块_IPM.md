# 比亚迪半导体 (BYD) 工业级 IPM 智能功率模块 - BIP120035V

[![Package](https://img.shields.io/badge/Package-DIP30--7931-blue.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BIP120035V** 是一款最新设计开发的 1200V/35A 大封装智能功率模块 (IPM)。该产品具有功耗小、抗干扰能力强等优点，与绝缘栅双极型晶体管 (IGBT) 相匹配。内部集成了欠压闭锁电路、温度模拟输出功能、过流保护电路和 IGBT 驱动电路，进一步丰富了模块功能，提高了系统的可靠性和稳定性。采用了分立的负端子和传感 IGBT 电流检测技术，可使外围电路独立监测逆变器的每一相电流，使用更灵活。主要面向 AC 400V 级电机控制应用。

### 🌟 核心特性 (Features)
* **高压大电流**：1200V / 35A 三相 IGBT 全桥逆变器，适合 AC 400V 级应用
* **全面保护**：内置 LVIC、HVIC，具有欠压闭锁保护和可调的过流保护（通过集成 Sense-IGBTs）
* **温度输出**：内置 LVIC 温度模拟输出功能
* **分立负端**：提供分立的三相直流负端，可独立检测各相电流
* **高绝缘性**：具备达 2500Vrms/min 的绝缘耐压等级

### 🚗 典型应用 (Applications)
* 商用空调、新能源汽车空调 (Commercial conditioner, new energy auto AC controller)
* AC 400V 级电机控制，如伺服、变频器 (AC 400V class motor control)
* 通用变频器 (General-purpose inverter)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 功率端耐压 (V<sub>CES</sub>) | 逆变电流 (I<sub>C</sub>) | 绝缘等级 (V<sub>ISO</sub>) | 内置拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **BIP120035V** | 1200 V | 35 A | 2500 Vrms/min | 三相六管全桥 (Three-Phase Inverter) | DIP30-7931 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>J</sub> = 25 °C，除非另外注明）

### 1. 逆变器功率部分 (Inverter Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>PN</sub> | 电源电压 (Supply voltage) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 900 | V |
| V<sub>PN(surge)</sub> | 电源浪涌电压 (Supply voltage (surge)) | 施加在 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 1000 | V |
| V<sub>CES</sub> | 集电极-发射极电压 (Collector-emitter voltage) | V<sub>GE</sub> = 0 V, I<sub>C</sub> = 100 μA, T<sub>J</sub> = 25 °C | 1200 | V |
| ± I<sub>C</sub> | 各 IGBT 集电极电流 (Each IGBT collector current) | T<sub>C</sub> = 25 °C | 35 | A |
| I<sub>CP</sub> | 晶圆集电极脉冲电流 (Each IGBT collector current (peak)) | T<sub>C</sub> = 25 °C, 脉宽 < 1 ms | 70 | A |
| P<sub>C</sub> | 集电极功耗 (Collector dissipation) | T<sub>C</sub> = 25 °C, 每一片小芯片 | 129.9 | W |
| T<sub>J</sub> | 结温 (Junction temperature) | 功率芯片极限最大结温限值（注 1） | -40 ~ +150 | °C |

> **注 1**：模块内集成的功率芯片最大结温额定值为 150 °C (@ T<sub>C</sub> ≤ 100 °C)。但在实际连续工作方案设计中，为了确保 IPM 的长期系统安全，平均结温建议限制在 T<sub>J</sub>(avg) ≤ 125 °C。

### 2. 控制与保护部分 (Control Part)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| V<sub>D</sub> | 控制电源电压 (Control supply voltage) | 施加在 V<sub>D(L)</sub> - COM(L), V<sub>D(HU)</sub>, V<sub>D(HV)</sub>, V<sub>D(HW)</sub> - COM(H) 之间 | 20 | V |
| V<sub>DB</sub> | 控制电源电压 (Control supply voltage) | 施加在 V<sub>B(U)</sub>-V<sub>S(U)</sub>, V<sub>B(V)</sub>-V<sub>S(V)</sub>, V<sub>B(W)</sub>-V<sub>S(W)</sub> 之间 | 20 | V |
| V<sub>IN</sub> | 信号输入电压 (Input Signal voltage) | 施加在控制信号输入 IN 与 COM 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| V<sub>FO</sub> | 故障输出电压 (Fault output voltage) | 施加在 V<sub>FO</sub> - COM(L) 之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |
| I<sub>FO</sub> | 故障输出电流 (Fault output current) | 在 V<sub>FO</sub> 端子的最大允许灌电流 | 2.0 | mA |
| V<sub>CIN</sub> | 电流检测输入电压 (Current sensing input voltage) | 施加在 C<sub>IN</sub> - COM(L) 采样端之间 | -0.3 ~ V<sub>D</sub> + 0.3 | V |

### 3. 整个系统特性 (Total System)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 额定值 (Ratings) | 单位 (Units) |
| :--- | :---: | :--- | :---: | :---: |
| V<sub>PN(PROT)</sub> | 自保护电源电压限制 (短路保护供电限制) | V<sub>D</sub> = 13.5 ~ 16.5 V, T<sub>J</sub> = 125 °C, 非重复性短路, < 2 μs | 800 | V |
| T<sub>C</sub> | 模块壳体工作温度 (Module case operation temperature) | - | -20 ~ +100 | °C |
| T<sub>STG</sub> | 存储/保存温度 (Storage temperature) | - | -40 ~ +150 | °C |
| V<sub>ISO</sub> | 绝缘内部耐压 (Isolation voltage) | 60 Hz 正弦波，交流电压持续 1 分钟，所有连接引脚到散热片基板之间 | 2500 | Vrms |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 符号 (Symbol) | 参数名称 (Parameter) | 工作条件 (Conditions) | 最大值 (Max.) | 单位 (Units) |
| :--- | :--- | :--- | :---: | :---: |
| R<sub>th(j-c)Q</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 IGBT 部分 (每 1/6 模块) | 0.77 | °C/W |
| R<sub>th(j-c)F</sub> | 结点-壳体热阻 (Junction to case) | 逆变器 FRD 续流二极管部分 (每 1/6 模块) | 1.25 | °C/W |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. 逆变器功率部分 (Inverter Part)

| 符号 (Symbol) | 参数说明 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>CE(SAT)</sub> | 集电极-发射极饱和电压 | V<sub>D</sub> = V<sub>BS</sub> = 15 V, V<sub>IN</sub> = 5 V, I<sub>C</sub> = 35 A, T<sub>J</sub> = 25 °C | - | 2.2 | 2.6 | V |
| | | T<sub>J</sub> = 125 °C | - | 2.3 | 2.7 | V |
| V<sub>F</sub> | FRD 正向导通电压 | V<sub>IN</sub> = 0 V, I<sub>C</sub> = 35 A, T<sub>J</sub> = 25 °C | - | 1.9 | 2.4 | V |
| I<sub>CES</sub> | 集电极-发射极间漏电流 | V<sub>CE</sub> = V<sub>CES</sub>, V<sub>GE</sub> = 0 V, T<sub>J</sub> = 25 °C | - | - | 0.1 | mA |
| | | T<sub>J</sub> = 125 °C | - | - | 1.0 | mA |

### 2. 开关动态损耗特性 (Switching Times, 感性负载测试)
测试条件：V<sub>PN</sub> = 600 V, V<sub>D</sub> = V<sub>BS</sub> = 15 V, I<sub>C</sub> = 35 A, V<sub>IN</sub> = 0 ↔ 5 V, T<sub>J</sub> = 25 °C（注 2）

| 驱动区域 | 符号 (Symbol) | 参数说明 (Parameter) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| **高端上桥臂**<br>(HS) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 1100 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 100 | - | ns |
| | t<sub>rr</sub> | 反向恢复时间 (Reverse recovery time) | - | 75 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 1400 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 140 | - | ns |
| **低端下桥臂**<br>(LS) | t<sub>ON</sub> | 开通时间 (Turn-on time) | - | 660 | - | ns |
| | t<sub>c(ON)</sub> | 开通交叉时间 (Turn-on across time) | - | 220 | - | ns |
| | t<sub>rr</sub> | 反向恢复时间 (Reverse recovery time) | - | 200 | - | ns |
| | t<sub>OFF</sub> | 关断时间 (Turn-off time) | - | 1000 | - | ns |
| | t<sub>c(OFF)</sub> | 关断交叉时间 (Turn-off across time) | - | 150 | - | ns |

> **注 2**：t<sub>ON</sub> 和 t<sub>OFF</sub> 包含了模块内部高低端驱动 IC 的传输延迟时间。而 t<sub>c(ON)</sub> 和 t<sub>c(OFF)</sub> 指的是在内部集成给定的驱动门极阻抗下，IGBT 晶圆本身的本征切换时间，t<sub>rr</sub> 指 FRD 反向恢复时间。

### 3. 控制与保护部分 (Control Part, T<sub>J</sub> = 25 °C)

| 符号 (Symbol) | 参数名称 (Parameter) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| I<sub>QDH</sub> | 高端 VD 静态电流 | V<sub>D(HU,HV,HW)</sub> = 15 V, IN<sub>(HU,HV,HW)</sub> = 0 V / 5 V | - | - | 340 | μA |
| I<sub>QDL</sub> | 低端 VD 静态电流 | V<sub>DL</sub> = 15 V, IN<sub>(LU,LV,LW)</sub> = 0 V / 5 V | - | - | 1.0 | mA |
| I<sub>QBS</sub> | VBS 静态电流 | V<sub>BS</sub> = 15 V, IN<sub>(HU,HV,HW)</sub> = 0 V / 5 V | - | - | 230 | μA |
| V<sub>FOH</sub> | 故障输出高电平电压 | V<sub>CIN</sub> = 0 V，故障引脚外接 4.7 kΩ 上拉到 5 V 电源 | 4.5 | - | - | V |
| V<sub>FOL</sub> | 故障输出低电平电压 | V<sub>CIN</sub> = 1 V，故障引脚外接 4.7 kΩ 上拉到 5 V 电源 | - | - | 0.8 | V |
| V<sub>CIN(ref)</sub> | 短路保护触发电压阈值 | V<sub>DL</sub> = 15 V（注 3） | 0.9 | 1.0 | 1.1 | V |
| UV<sub>DLD</sub> | 低端电源欠压检测电平 | 控制供电电源检测电平（电压下降脱扣） | 11 | 12 | 13 | V |
| UV<sub>DLR</sub> | 低端电源欠压复位电平 | 控制供电电源迟滞复位电平（电压回升恢复） | 12 | 13 | 14 | V |
| UV<sub>BSD</sub> | 高端自举电路欠压检测 | 自举浮动供电监测（电压下降脱扣） | 7.9 | 9.3 | 10.7 | V |
| UV<sub>BSR</sub> | 高端自举电路欠压复位 | 自举浮动供电监测（电压回升恢复） | 8.7 | 10.2 | 11.7 | V |
| V<sub>OT</sub> | 温度模拟输出电压 | LVIC 温度 = 110 °C（注 4） | 3.12 | 3.20 | 3.28 | V |
| t<sub>FO</sub> | 故障输出脉冲宽度 | C<sub>FO</sub> = 33 nF（注 5） | - | 2.30 | - | ms |
| V<sub>IN(ON)</sub> | 控制信号导通阈值电压 | 施加在输入引脚与 COM 之间 | - | - | 3.3 | V |
| V<sub>IN(OFF)</sub> | 控制信号关断阈值电压 | 施加在输入引脚与 COM 之间 | 0.8 | - | - | V |

> **注 3**：短路/过流保护功能仅在模块的**低端下桥臂**驱动电路中有效。
> **注 4**：当温度上升过多时 IPM 自身并不会自动关闭 IGBT，也无 VFO 输出。当温度超过用户设定的保护值时，控制器 (MCU) 应立即发出关断信号停止 IPM 工作。
> **注 5**：故障信号输出脉冲宽度 t<sub>FO</sub> 依赖电容 C<sub>FO</sub> 的容值，近似的计算公式如下：C<sub>FO</sub> ≈ 14.3 × 10<sup>-6</sup> × t<sub>FO</sub> [F]。

---

## 🔩 机械特性与额定机械值 (Mechanical Characteristics)

| 符号 (Symbol) | 参数与测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 (Units) |
| :--- | :--- | :---: | :---: | :---: | :---: |
| 安装扭矩 | 紧固安装螺钉：M3 规格螺丝螺纹（推荐选择稳定力矩：1.18 N·m） | 0.98 | 1.18 | 1.47 | N·m |
| 端子拉力强度 | 负载 19.6 N | 10 | - | - | s |
| 端子弯曲强度 | 负载 9.8 N, 90 度弯曲 | 2 | - | - | times |
| 重量 (Weight) | 模块整体产品克重 | - | 43 | - | g |
| 器件平面度 | 模块背板 DBC 陶瓷平面翘曲平面度控制范围要求 | 0 | - | 200 | μm |

---

## 📈 推荐工作条件 (Recommended Operating Conditions)

| 符号 (Symbol) | 参数名称 (Parameter) | 推荐测试/应用条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :--- | :--- | :---: | :---: | :---: | :---: |
| V<sub>PN</sub> | 电源主干电压 | 施加在主变频端子 P - N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> 之间 | 350 | 600 | 800 | V |
| V<sub>D</sub> | 控制电源电压 | 施加在 V<sub>D(L)</sub> - COM(L), V<sub>D(H)</sub> - COM(H) 之间 | 13.5 | 15.0 | 16.5 | V |
| V<sub>BS</sub> | 高端辅助电源电压 | 施加在 V<sub>B(U)</sub>-V<sub>S(U)</sub>, V<sub>B(V)</sub>-V<sub>S(V)</sub>, V<sub>B(W)</sub>-V<sub>S(W)</sub> 之间 | 13.5 | 15.0 | 18.5 | V |
| dV<sub>D</sub>/dt, dV<sub>DB</sub>/dt | 控制电压动态波动率 | 供电电平的动态瞬态电压变化波动范围 | -1 | - | 1 | V/μs |
| t<sub>DEAD</sub> | 桥臂互锁防直通死区 | 作用于控制 MCU 侧输出的同桥臂上下两路 PWM 信号互锁死区时间限制 | 3.0 | - | - | μs |
| PW<sub>IN(on)</sub> | 最小输入脉冲宽度 (导通) | V<sub>D</sub> = V<sub>BS</sub> = 15 V, I<sub>C</sub> ≤ 70 A（注 6） | 2.0 | - | - | μs |
| PW<sub>IN(off)</sub> | 最小输入脉冲宽度 (关断) | V<sub>D</sub> = V<sub>BS</sub> = 15 V, I<sub>C</sub> ≤ 70 A（注 6） | 2.0 | - | - | μs |
| f<sub>PWM</sub> | PWM 调制载波频率 | 系统推荐开关载波工作范围，-20 °C ≤ T<sub>J</sub> ≤ 125 °C, T<sub>C</sub> ≤ 100 °C | - | - | 20 | kHz |
| V<sub>SEN</sub> | 电流检测采样输出电压 | 施加在负端采样电阻端子 N<sub>U</sub>, N<sub>V</sub>, N<sub>W</sub> - COM(L) 之间（含允许纹波浪涌）| -5 | - | 5 | V |

> **注 6**：如果输入脉冲宽度小于推荐值，IPM 可能不会做出正确的响应。

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Package) | 每料管装数 (pcs/tube) | 每箱料管数 (tube/box) | 总装箱量 (pcs/box) |
| :---: | :---: | :---: | :---: |
| 抗静电料管 (Tube) | 6 | 30 | 180 |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
