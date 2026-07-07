# 比亚迪半导体 (BYD) 工业级 IGBT 单管 - BGF15T65SD

[![Standard](https://img.shields.io/badge/Standard-Industrial-green.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BGF15T65SD** 是一款基于先进 TrenchFS 技术（Trench Field-Stop Technology）构建的高性能、高可靠性 IGBT 单管，内部集成了软快恢复反并联二极管。本产品为工业级标准，专为通用工业变频器及电气应用设计。

### 🌟 核心特性 (Features)
* **尖端技术**：650V Trench 场终止技术 (Trench Field-Stop Technology)
* **损耗表现**：低的导通损耗和开关损耗 (Low conduction and switching losses)
* **温漂特性**：饱和导通电压 (V<sub>CE(sat)</sub>) 具有正温度系数，利于并联拓展
* **短路强韧**：具备 5 μs 的短路耐受承受能力

### 🚗 典型应用 (Applications)
* 工业缝纫机 (Industrial Sewing Machine)
* 通用变频器 (General Inverter)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 (V<sub>CE</sub>) | 集电极电流 (I<sub>C</sub>) | 典型饱和电压 (V<sub>CE(sat)</sub>) | 最高结温 (T<sub>jmax</sub>) | 印丝标记 (Marking) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BGF15T65SD** | 650 V | 15 A | 1.8 V | 175 °C | 15T65SD | TO220F-3 |

---

## ⚡ 最大额定参数 (Maximum Rated Values)

下表规定了器件工作或测试时绝不可超过的极限参数（如无特殊说明，T<sub>j</sub> ≥ 25 °C）：

| 参数名称 (Parameter) | 符号 (Symbol) | 额定值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| 集电极-发射极电压 | V<sub>CE</sub> | 650 | V |
| 连续集电极电流 (T<sub>C</sub> = 25 °C) | I<sub>C</sub> | 30 | A |
| 连续集电极电流 (T<sub>C</sub> = 100 °C) | I<sub>C</sub> | 15 | A |
| 集电极脉冲电流 (脉宽受 T<sub>jmax</sub> 限制) | I<sub>Cpuls</sub> | 60 | A |
| 二极管正向直流电流 (T<sub>C</sub> = 25 °C) | I<sub>F</sub> | 30 | A |
| 二极管正向直流电流 (T<sub>C</sub> = 100 °C) | I<sub>F</sub> | 15 | A |
| 二极管脉冲电流 | I<sub>Fpuls</sub> | 60 | A |
| 栅极-发射极电压 | V<sub>GE</sub> | ± 20 | V |
| 短路耐受时间 (V<sub>GE</sub>=15 V, V<sub>CC</sub>≤400 V, T<sub>j</sub>≤150 °C) | t<sub>sc</sub> | 5 | μs |
| 总耗散功率 (T<sub>C</sub> = 25 °C) | P<sub>tot</sub> | 37.5 | W |
| 最高结温 | T<sub>jmax</sub> | 175 | °C |
| 工作结温 | T<sub>jop</sub> | -40 ... +150 | °C |
| 储存温度 | T<sub>stg</sub> | -55 ... +150 | °C |
| 焊接温度 (距管壳 1.6mm 处限时 10s) | T<sub>st</sub> | 260 | °C |
| 锁装力矩 (M3 螺丝) | M<sub>d</sub> | 0.5 | Nm |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| IGBT 结-管壳热阻 | R<sub>th(j-c)</sub> | 4.0 | °C/W |
| 二极管结-管壳热阻 | R<sub>th(j-c)</sub> | 7.9 | °C/W |
| 结-环境热阻 | R<sub>th(j-a)</sub> | 62.5 | °C/W |

---

## 🔌 电学特性 (Electrical Characteristics)

### 1. 静态特性 (Static Characteristic, T<sub>j</sub> = 25 °C 除非特别声明)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极击穿电压 | V<sub>(BR)CES</sub> | V<sub>GE</sub>=0 V, I<sub>C</sub>=0.5 mA | 650 | - | - | V |
| 集电极-发射极饱和电压 | V<sub>CE(sat)</sub> | V<sub>GE</sub>=15 V, I<sub>C</sub>=15 A, T<sub>j</sub>=25 °C<br>V<sub>GE</sub>=15 V, I<sub>C</sub>=15 A, T<sub>j</sub>=150 °C | - | 1.8<br>2.3 | 2.1<br>- | V |
| 二极管正向导通电压 | V<sub>F</sub> | V<sub>GE</sub>=0 V, I<sub>F</sub>=15 A, T<sub>j</sub>=25 °C<br>V<sub>GE</sub>=0 V, I<sub>F</sub>=15 A, T<sub>j</sub>=150 °C | - | 1.9<br>1.6 | 2.4<br>- | V |
| 栅极-发射极阈值电压 | V<sub>GE(th)</sub> | I<sub>C</sub>=300 μA, V<sub>CE</sub>=V<sub>GE</sub> | 4.5 | 5.5 | 6.5 | V |
| 集电极-发射极截止电流 | I<sub>CES</sub> | V<sub>CE</sub>=650 V, V<sub>GE</sub>=0 V | - | - | 100 | μA |
| 栅极-发射极漏电流 | I<sub>GES</sub> | V<sub>CE</sub>=0 V, V<sub>GE</sub>=±20 V | -200 | - | 200 | nA |

### 2. 动态特性 (Dynamic Characteristic)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :---: | :--- | :---: | :---: |
| 输入电容 | C<sub>ies</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz | 812 | pF |
| 输出电容 | C<sub>oes</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz | 63 | pF |
| 反向传输电容 | C<sub>res</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz | 8 | pF |
| 门极总电量 | Q<sub>G</sub> | V<sub>CC</sub>=400 V, I<sub>C</sub>=30 A, V<sub>GE</sub>=15 V | 21.1 | nC |
| 内部发射极电感 | L<sub>E</sub> | - | - | nH |
| 短路电流 | I<sub>C(sc)</sub> | V<sub>CC</sub>=400 V, V<sub>GE</sub>=15 V, T<sub>j</sub>=150 °C | 50 | A |
| 反偏安全工作区 | RBSOA | - | - | A |

---

## 🔄 开关特性 (Switching Characteristics)

### 1. T<sub>j</sub> = 25 °C 时开关特性（感性负载）
测试条件：V<sub>CC</sub>=400 V, I<sub>C</sub>=15 A, V<sub>GE</sub>=-7.5/15 V, R<sub>G</sub>=10 Ω

| 参数分类 | 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :--- | :---: | :---: | :---: |
| **IGBT 特性** | 开通延迟时间 (Turn-on delay time) | t<sub>d(on)</sub> | 125 | ns |
| | 上升时间 (Rise time) | t<sub>r</sub> | 59 | ns |
| | 关断延迟时间 (Turn-off delay time) | t<sub>d(off)</sub> | 60 | ns |
| | 下降时间 (Fall time) | t<sub>f</sub> | 79 | ns |
| | 开通损耗 (Turn-on energy)* | E<sub>on</sub> | 0.33 | mJ |
| | 关断损耗 (Turn-off energy) | E<sub>off</sub> | 0.21 | mJ |
| | 总开关损耗 (Total switching energy) | E<sub>ts</sub> | 0.54 | mJ |
| **反并联二极管** | 反向恢复时间 (Reverse recovery time) | t<sub>rr</sub> | 186 | ns |
| | 恢复电荷 (Recovered charge) | Q<sub>rr</sub> | 320 | nC |
| | 反向恢复峰值电流 (Peak reverse recovery current) | I<sub>RM</sub> | 3.3 | A |
| | 反向恢复损耗 (Reverse recovered energy) | E<sub>rec</sub> | - | mJ |

*\*注：开通损耗 E<sub>on</sub> 与总损耗 E<sub>ts</sub> 包含二极管反向恢复引起的额外损耗。*

### 2. T<sub>j</sub> = 150 °C 时开关特性（感性负载）
测试条件：V<sub>CC</sub>=400 V, I<sub>C</sub>=15 A, V<sub>GE</sub>=-7.5/15 V, R<sub>G</sub>=10 Ω

| 参数分类 | 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :--- | :---: | :---: | :---: |
| **IGBT 特性** | 开通延迟时间 (Turn-on delay time) | t<sub>d(on)</sub> | 32 | ns |
| | 上升时间 (Rise time) | t<sub>r</sub> | 91 | ns |
| | 关断延迟时间 (Turn-off delay time) | t<sub>d(off)</sub> | 74 | ns |
| | 下降时间 (Fall time) | t<sub>f</sub> | 135 | ns |
| | 开通损耗 (Turn-on energy)* | E<sub>on</sub> | 0.50 | mJ |
| | 关断损耗 (Turn-off energy) | E<sub>off</sub> | 0.30 | mJ |
| | 总开关损耗 (Total switching energy) | E<sub>ts</sub> | 0.80 | mJ |
| **反并联二极管** | 反向恢复时间 (Reverse recovery time) | t<sub>rr</sub> | 252 | ns |
| | 恢复电荷 (Recovered charge) | Q<sub>rr</sub> | 920 | nC |
| | 反向恢复峰值电流 (Peak reverse recovery current) | I<sub>RM</sub> | 4.8 | A |
| | 反向恢复损耗 (Reverse recovered energy) | E<sub>rec</sub> | - | mJ |

---

## 📐 封装外形尺寸 (TO220F-3 Outline Dimensions)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

| 符号 (Symbol) | 最小值 (Min.) | 最大值 (Max.) | 符号 (Symbol) | 最小值 (Min.) | 最大值 (Max.) |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **A** | 4.50 | 4.90 | **E** | 10.00 | 10.40 |
| **A1** | 2.45 | 2.75 | **e** | 2.54 | 2.54 |
| **A2** | 1.75 | 2.05 | **L** | 12.70 | 13.80 |
| **b** | 0.60 | 0.78 | **L1** | 2.80 | 3.40 |
| **b1** | 1.15 | 1.45 | **ΦP** | 3.10 | 3.30 |
| **c** | 0.40 | 0.60 | **Q** | 3.10 | 3.40 |
| **D** | 15.50 | 16.20 | | | |

*\*备注：因各封装厂的模具存在细微差异，请以实物尺寸为准。*

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Packing) | 每管数量 (pcs/tube) | 每盒管数 (tube/inner box) | 每箱盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| 管装 (Tube) | 50 | 8 | 5 | 2000 |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
