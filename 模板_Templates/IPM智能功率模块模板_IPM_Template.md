# 比亚迪半导体 (BYD) IPM 智能功率模块数据转换模板

> 💡 **贡献者填写指南**：
> [cite_start]1. 本模板专门用于处理【功率半导体】板块下的 **IPM 智能功率模块 (Intelligent Power Modules)** [cite: 436]。
> [cite_start]2. 相比普通单管，IPM 模块增加了【控制端子特性】、【内置保护功能】及【NTC 热敏电阻】等特有参数，提取 PDF 数据时切勿漏掉 。
> 3. 括号内的中文/英文提示语（如 `[型号]`）在实际转换时，请替换为规格书（Datasheet）中的真实数据。

---

# 比亚迪半导体 (BYD) [产品级别：如工业级/家电级] IPM 模块 - [产品型号]

[![Package](https://img.shields.io/badge/Package-[封装形式：如DIP--25/SOP--23]-blue.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

[cite_start]本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验 [cite: 430]。

---

## 📌 产品概述 (Product Overview)

[cite_start]**[产品型号]** 是一款集成度极高的 [如：三相无刷直流电机驱动] 智能功率模块 (IPM) [cite: 432, 436][cite_start]。该模块内部集成了 [如：6个低损耗场终止 IGBT] 和反并联快恢复二极管，并配置了优化的配套栅极驱动及保护电路 。主要针对 [如：高档变频家电、伺服驱动及低功率变频器] 市场设计。

### 🌟 核心特性 (Features)
* **高度集成**：内置三相逆变拓扑、高压栅极驱动（HVIC）及单电源偏置设计
* [cite_start]**全面保护**：控制端具备欠压锁定保护 (UVLO) 及全相短路/过流保护 (SCP) 
* [cite_start]**温度监控**：内置 NTC 热敏电阻，可实现实时的模块过温监测 
* **逻辑兼容**：输入接口兼容 3.3V 和 5V 的 CMOS/TTL 逻辑电平

### 🚗 典型应用 (Applications)
* 变频空调与冰箱压缩机驱动 (Inverter Air Conditioner & Refrigerator)
* 变频洗衣机及洗碗机驱动 (Inverter Washing Machine)
* 工业小功率伺服驱动器与风机 (Low-power Servo Driver & Fan Motor)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 功率端耐压 ($V_{CES}$) | 逆变电流 ($I_C$) | 控制电源电压 ($V_{DD}$) | 内置拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **[产品型号]** | [电压] V | [电流] A | [电压] V | [如：三相全桥 Three-Phase Bridge] | [封装名称] |

---

## ⚡ 最大额定参数 (Maximum Rated Values)

### 1. 逆变功率部分 (Inverter Part)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 供电主电压 | $V_{CC}$ | 应用在 $P$ 与 $N$ 端子之间 | [数值] | V |
| 集电极-发射极电压 | $V_{CES}$ | - | [数值] | V |
| 每相集电极电流 | $I_C$ | $T_C = 25^\circ\text{C}$<br>$T_C = 100^\circ\text{C}$ | [数值]<br>[数值] | A |
| 集电极脉冲电流 | $I_{CP}$ | 脉宽受限，低于 $1\,\text{ms}$ | [数值] | A |
| 模块总耗散功率 | $P_{tot}$ | 每只 IGBT 晶圆，$T_C = 25^\circ\text{C}$ | [数值] | W |

### 2. 控制与保护部分 (Control & Protection Part)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 控制电源电压 | $V_{DD}$ | 应用在 $V_{DD}$ 与 $V_{SS}$ 之间 | [数值] | V |
| 自举电源电压 | $V_{BS}$ | 应用在 $V_{B(U)}-V_{S(U)}$, $V_{B(V)}-V_{S(V)}$, $V_{B(W)}-V_{S(W)}$ | [数值] | V |
| 信号输入电压 | $V_{IN}$ | 应用在 $IN_{(UH)}$, $IN_{(VH)}$, $IN_{(WH)}$, $IN_{(UL)}$, $IN_{(VL)}$, $IN_{(WL)}$ | [数值] | V |
| 故障输出电压 | $V_{FO}$ | 应用在 $V_{FO}$ 与 $V_{SS}$ 之间 | [数值] | V |

---

## 🔌 电学特性 (Electrical Characteristics)

### 1. 功率部分 (Power Part, $T_j = 25^\circ\text{C}$)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极截止电流 | $I_{CES}$ | $V_{CE} = V_{CES}$ | - | - | [数值] | $\mu\text{A}$ |
| 集电极-发射极饱和电压 | $V_{CE(sat)}$ | $V_{DD} = 15\text{V}, V_{IN} = 5\text{V}, I_C = [数值]\text{A}$ | - | [数值] | [数值] | V |
| 二极管正向导通电压 | $V_F$ | $V_{IN} = 0\text{V}, I_F = [数值]\text{A}$ | - | [数值] | [数值] | V |

### 2. 控制与保护部分 (Control & Protection Part, $T_j = 25^\circ\text{C}$)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 控制电源静态电流 | $I_{DDR}$ | $V_{DD} = 15\text{V}, V_{IN} = 0\text{V}$ | - | [数值] | [数值] | $\text{mA}$ |
| 故障输出电平电压 | $V_{FO(H)}$<br>$V_{FO(L)}$ | 正常状态 ($V_{FO}$ 内部上拉)<br>过流/欠压故障保护动作状态 | [数值]<br>- | -<br>- | -<br>[数值] | V |
| 控制电源欠压保护 | $UV_{DDD}$<br>$UV_{DDR}$ | 脱扣电平 (检测电压下降)<br>复位电平 (检测电压上升) | [数值]<br>[数值] | [数值]<br>[数值] | [数值]<br>[数值] | V |
| 短路/过流保护阈值 | $V_{SC}$ | 内部比较器动作电压（依托 $C_{SC}$ 采样端） | [数值] | [数值] | [数值] | V |

---

## 🌡️ NTC 热敏电阻特性 (NTC Thermistor Characteristic)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 电阻值 | $R_{25}$ | $T_C = 25^\circ\text{C}$ | - | [数值] | - | $\text{k}\Omega$ |
| 电阻值 | $R_{100}$ | $T_C = 100^\circ\text{C}$ | - | [数值] | - | $\text{k}\Omega$ |
| B 常数 | $B$ | 测算范围: $25^\circ\text{C}$ 到 $100^\circ\text{C}$ | - | [数值] | - | K |

---

## 📐 封装外形尺寸 (Outline Dimensions)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

*(此处可根据具体封装引脚排布绘制尺寸和参数表格)*

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
[cite_start]技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供 [cite: 431]。
