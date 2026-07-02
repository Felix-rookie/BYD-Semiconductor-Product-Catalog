# 比亚迪半导体 (BYD) IGBT 单管产品数据转换模板

> 💡 **贡献者填写指南**：
> 1. 本模板专门用于处理【功率半导体】板块下的 **硅基/碳化硅基 IGBT 单管 (Discrete IGBTs)**。
> 2. 括号内的中文/英文提示语（如 `[型号]`）在实际转换时，请替换为规格书（Datasheet）中的真实数据。
> 3. 所有电学符号请严格统一使用学术 LaTeX 公式（如 `$V_{CE}$`, `$I_C$`, `$T_j$`），以确保全库参数检索的精准度。

---

# 比亚迪半导体 (BYD) [产品级别：如车规级/工业级] IGBT 单管 - [产品型号，如 BGNE40Q120SD-A]

[![Standard](https://img.shields.io/badge/Standard-[标准：如AEC--Q101/工业级]-[颜色].svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**[产品型号]** 是一款基于先进 [技术类型：如场终止 Field-Stop Technology] 技术构建的高性能、高可靠性 IGBT 单管，内部集成 [二极管特性：如软快恢复反并联二极管]。本产品 [认证标准：如严格符合 AEC-Q101 车规级标准要求]，专为 [应用领域：如严酷的汽车及工业电气环境] 设计。

### 🌟 核心特性 (Features)
* **尖端技术**：[如：1200V 平面栅场终止技术 (Planar Field-Stop Technology)]
* **损耗表现**：[如：极低的开关损耗 (Low switching losses)]
* **温偏特性**：[如：饱和导通电压具有正温度系数，利于并联拓展]
* **短路强韧**：[如：具备高达 10µs 的短路耐受承受能力]

### 🚗 典型应用 (Applications)
* [应用案例 1，如：电动汽车空调压缩机 (Electric Automotive Air-Condition Compressor)]
* [应用案例 2，如：汽车 PTC 加热方案 (Electric Automotive PTC Heater)]
* [应用案例 3，如：通用工业变频器 (General Inverter)]

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 ($V_{CE}$) | 集电极电流 ($I_C$) | 典型饱和电压 ($V_{CE(sat)}$) | 最高结温 ($T_{jmax}$) | 印丝标记 (Marking) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **[产品型号]** | [电压值] V | [电流值] A | [典型饱和电压值] V | [温度] °C | [表面标记] | [封装名称，如 TO-247-3L] |

---

## ⚡ 最大额定参数 (Maximum Rated Values)

下表规定了器件工作或测试时绝不可超过的极限参数（如无特殊说明，$T_j = 25^\circ\text{C}$）：

| 参数名称 (Parameter) | 符号 (Symbol) | 额定值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| 集电极-发射极电压 | $V_{CE}$ | [数值] | V |
| 连续集电极电流 ($T_C = 25^\circ\text{C}$) | $I_C$ | [数值] | A |
| 连续集电极电流 ($T_C = 100^\circ\text{C}$) | $I_C$ | [数值] | A |
| 集电极脉冲电流 (脉宽受 $T_{jmax}$ 限制) | $I_{Cpuls}$ | [数值] | A |
| 二极管正向直流电流 ($T_C = 25^\circ\text{C}$) | $I_F$ | [数值] | A |
| 二极管正向直流电流 ($T_C = 100^\circ\text{C}$) | $I_F$ | [数值] | A |
| 二极管脉冲电流 | $I_{Fpuls}$ | [数值] | A |
| 栅极-发射极电压 | $V_{GE}$ | [数值] | V |
| 短路耐受时间 | $t_{sc}$ | [数值] | $\mu\text{s}$ |
| 总耗散功率 ($T_C = 25^\circ\text{C}$) | $P_{tot}$ | [数值] | W |
| 最高结温 | $T_{jmax}$ | [数值] | °C |
| 工作结温 | $T_{jop}$ | [范围] | °C |
| 储存温度 | $T_{stg}$ | [范围] | °C |
| 焊接温度 (距管壳 1.6mm 处限时 10s) | $T_{st}$ | [数值] | °C |
| 锁装力矩 | $M_d$ | [数值] | Nm |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| IGBT 结-管壳热阻 | $R_{th(j-c)}$ | [数值] | °C/W |
| 二极管结-管壳热阻 | $R_{th(j-c)}$ | [数值] | °C/W |
| 结-环境热阻 | $R_{th(j-a)}$ | [数值] | °C/W |

---

## 🔌 电学特性 (Electrical Characteristics)

### 1. 静态特性 (Static Characteristic, $T_j = 25^\circ\text{C}$ 除非特别声明)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极击穿电压 | $V_{(BR)CES}$ | $V_{GE}=0\text{V}, I_C=[数值]\text{mA}$ | [数值] | - | - | V |
| 集电极-发射极饱和电压 | $V_{CE(sat)}$ | $V_{GE}=15\text{V}, I_C=[数值]\text{A}, T_j=25^\circ\text{C}$<br>$V_{GE}=15\text{V}, I_C=[数值]\text{A}, T_j=[数值]^\circ\text{C}$ | - | [数值]<br>[数值] | [数值]<br>- | V |
| 二极管正向导通电压 | $V_F$ | $V_{GE}=0\text{V}, I_F=[数值]\text{A}, T_j=25^\circ\text{C}$<br>$V_{GE}=0\text{V}, I_F=[数值]\text{A}, T_j=[数值]^\circ\text{C}$ | - | [数值]<br>[数值] | [数值]<br>- | V |
| 栅极-发射极阈值电压 | $V_{GE(th)}$ | $I_C=[数值]\text{mA}, V_{CE}=V_{GE}$ | [数值] | [数值] | [数值 ] | V |
| 集电极-发射极截止电流 | $I_{CES}$ | $V_{CE}=[数值]\text{V}, V_{GE}=0\text{V}$ | - | - | [数值] | $\mu\text{A}$ |
| 栅极-发射极漏电流 | $I_{GES}$ | $V_{CE}=0\text{V}, V_{GE}=\pm20\text{V}$ | [数值] | - | [数值] | nA |

### 2. 动态特性 (Dynamic Characteristic)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :---: | :--- | :---: | :---: |
| 输入电容 | $C_{ies}$ | $V_{CE}=[数值]\text{V}, V_{GE}=0\text{V}, f=1\text{MHz}$ | [数值] | pF |
| 输出电容 | $C_{oes}$ | $V_{CE}=[数值]\text{V}, V_{GE}=0\text{V}, f=1\text{MHz}$ | [数值] | pF |
| 反向传输电容 | $C_{res}$ | $V_{CE}=[数值]\text{V}, V_{GE}=0\text{V}, f=1\text{MHz}$ | [数值] | pF |
| 门极总电量 | $Q_G$ | $V_{CC}=[数值]\text{V}, I_C=[数值]\text{A}, V_{GE}=15\text{V}$ | [数值] | nC |
| 内部发射极电感 | $L_E$ | - | [数值] | nH |
| 短路电流 | $I_{C(sc)}$ | $V_{CC}=[数值]\text{V}, V_{GE}=15\text{V}, T_j=[数值]^\circ\text{C}$ | [数值] | A |
| 反偏安全工作区 | RBSOA | $V_{CC}=[数值]\text{V}, V_{GE}=15\text{V}, T_j\le[数值]^\circ\text{C}$ | [数值] | A |

---

## 🔄 开关特性 (Switching Characteristics)

### 1. $T_j = 25^\circ\text{C}$ 时开关特性（感性负载）
测试条件：$V_{CC}=[数值]\text{V}, I_C=[数值]\text{A}, V_{GE}=[-7.5/15]\text{V}, R_G=[数值]\,\Omega$

| 参数分类 | 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :--- | :---: | :---: | :---: |
| **IGBT 特性** | 开通延迟时间 (Turn-on delay time) | $t_{d(on)}$ | [数值] | ns |
| | 上升时间 (Rise time) | $t_r$ | [数值] | ns |
| | 关断延迟时间 (Turn-off delay time) | $t_{d(off)}$ | [数值] | ns |
| | 下降时间 (Fall time) | $t_f$ | [数值] | ns |
| | 开通损耗 (Turn-on energy)* | $E_{on}$ | [数值] | mJ |
| | 关断损耗 (Turn-off energy) | $E_{off}$ | [数值] | mJ |
| | 总开关损耗 (Total switching energy) | $E_{ts}$ | [数值] | mJ |
| **反并联二极管** | 反向恢复时间 (Reverse recovery time) | $t_{rr}$ | [数值] | ns |
| | 恢复电荷 (Recovered charge) | $Q_{rr}$ | [数值] | $\mu\text{C}$ |
| | 反向恢复峰值电流 (Peak reverse recovery current) | $I_{RM}$ | [数值] | A |
| | 反向恢复损耗 (Reverse recovered energy) | $E_{rec}$ | [数值] | mJ |

*\*注：开通损耗 $E_{on}$ 与总损耗 $E_{ts}$ 包含二极管反向恢复引起的额外损耗。*

### 2. $T_j = [150/175]^\circ\text{C}$ 时开关特性（感性负载）
测试条件：$V_{CC}=[数值]\text{V}, I_C=[数值]\text{A}, V_{GE}=[-7.5/15]\text{V}, R_G=[数值]\,\Omega$

| 参数分类 | 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :--- | :---: | :---: | :---: |
| **IGBT 特性** | 开通延迟时间 (Turn-on delay time) | $t_{d(on)}$ | [数值] | ns |
| | 上升时间 (Rise time) | $t_r$ | [数值] | ns |
| | 关断延迟时间 (Turn-off delay time) | $t_{d(off)}$ | [数值] | ns |
| | 下降时间 (Fall time) | $t_f$ | [数值] | ns |
| | 开通损耗 (Turn-on energy)* | $E_{on}$ | [数值] | mJ |
| | 关断损耗 (Turn-off energy) | $E_{off}$ | [数值] | mJ |
| | 总开关损耗 (Total switching energy) | $E_{ts}$ | [数值] | mJ |
| **反并联二极管** | 反向恢复时间 (Reverse recovery time) | $t_{rr}$ | [数值] | ns |
| | 恢复电荷 (Recovered charge) | $Q_{rr}$ | [数值] | $\mu\text{C}$ |
| | 反向恢复峰值电流 (Peak reverse recovery current) | $I_{RM}$ | [数值] | A |
| | 反向恢复损耗 (Reverse recovered energy) | $E_{rec}$ | [数值] | mJ |

---

## 📐 封装外形尺寸 ([封装形式, 如 TO-247-3L] Outline Dimensions)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

| 符号 (Symbol) | 最小值 (Min.) | 最大值 (Max.) | 符号 (Symbol) | 最小值 (Min.) | 最大值 (Max.) |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **A** | [数值] | [数值] | **E3** | [数值] | [数值] |
| **A1** | [数值] | [数值] | **F** | [数值] | [数值] |
| **A2** | [数值] | [数值] | **F1** | [数值] | [数值] |
| **B** | [数值] | [数值] | **e** | [数值] | [数值] |
| **B1** | [数值] | [数值] | **L** | [数值] | [数值] |
| **B2** | [数值] | [数值] | **L1** | [数值] | [数值] |
| **B3** | [数值] | [数值] | **ΦP** | [数值] | [数值] |
| **C** | [数值] | [数值] | **ΦP1** | [数值] | [数值] |
| **D** | [数值] | [数值] | **ΦP2** | [数值] | [数值] |
| **D1** | [数值] | [数值] | **Q** | [数值] | [数值] |
| **D2** | [数值] | [数值] | **S** | [数值] | [数值] |
| **E** | [数值] | [数值] | **θ** | [角度] | [角度] |
| **E1** | [数值] | [数值] | **θ2** | [角度] | [角度] |
| **E2** | [数值] | [数值] | | | |

*\*备注：因各封装厂的模具存在细微差异，请以实物尺寸为准。*

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Packing) | 每管/盘数量 (pcs/tube) | 每盒箱数 (tube/inner box) | 每箱盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| [如：管装 Tube] | [数值] | [数值] | [数值] | [数值] |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
