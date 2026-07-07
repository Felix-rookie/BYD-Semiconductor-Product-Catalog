# 比亚迪半导体 (BYD) 工业级 IGBT 单管 - BGN80V65HD

[![Standard](https://img.shields.io/badge/Standard-Industrial-green.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BGN80V65HD** 是一款基于先进 TrenchFS 技术（Trench Field-Stop Technology）构建的高性能、高可靠性 IGBT 单管，内部集成了软快恢复反并联二极管。本产品为工业级标准，专为 UPS、焊机及光伏逆变器应用设计。

### 🌟 核心特性 (Features)
* **尖端技术**：650V Trench 场终止技术 (Trench Field-Stop Technology)
* **损耗表现**：低的导通损耗和开关损耗 (Low conduction and switching losses)
* **低栅极电荷**：低栅极电荷量 (Low gate charge)
* **高温工作**：最高工作结温可达 175 °C (Maximum operating temperature of 175 °C)

### 🚗 典型应用 (Applications)
* 不间断电源 (UPS)
* 焊机 (Welding)
* 光伏逆变器 (Solar Inverter)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 (V<sub>CE</sub>) | 集电极电流 (I<sub>C</sub>) | 典型饱和电压 (V<sub>CE(sat)</sub>) | 最高结温 (T<sub>jmax</sub>) | 印丝标记 (Marking) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BGN80V65HD** | 650 V | 80 A | 1.7 V | 175 °C | 80V65HD | TO-247 |

---

## ⚡ 最大额定参数 (Maximum Rated Values)

下表规定了器件工作或测试时绝不可超过的极限参数（如无特殊说明，T<sub>j</sub> ≥ 25 °C）：

| 参数名称 (Parameter) | 符号 (Symbol) | 额定值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| 集电极-发射极电压 | V<sub>CE</sub> | 650 | V |
| 连续集电极电流 (T<sub>C</sub> = 25 °C) | I<sub>C</sub> | 160 | A |
| 连续集电极电流 (T<sub>C</sub> = 100 °C) | I<sub>C</sub> | 80 | A |
| 集电极脉冲电流 (脉宽受 T<sub>jmax</sub> 限制) | I<sub>Cpuls</sub> | 320 | A |
| 二极管正向直流电流 (T<sub>C</sub> = 25 °C) | I<sub>F</sub> | 160 | A |
| 二极管正向直流电流 (T<sub>C</sub> = 100 °C) | I<sub>F</sub> | 80 | A |
| 二极管脉冲电流 | I<sub>Fpuls</sub> | 320 | A |
| 栅极-发射极电压 | V<sub>GE</sub> | ± 20 | V |
| 总耗散功率 (T<sub>C</sub> = 25 °C) | P<sub>tot</sub> | 395 | W |
| 最高结温 | T<sub>jmax</sub> | 175 | °C |
| 工作结温 | T<sub>jop</sub> | -40 ... +175 | °C |
| 储存温度 | T<sub>stg</sub> | -55 ... +150 | °C |
| 焊接温度 (距管壳 1.6mm 处限时 10s) | T<sub>st</sub> | 260 | °C |
| 锁装力矩 (M3 螺丝) | M<sub>d</sub> | 0.6 | Nm |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| IGBT 结-管壳热阻 | R<sub>th(j-c)</sub> | 0.38 | °C/W |
| 二极管结-管壳热阻 | R<sub>th(j-c)</sub> | 0.45 | °C/W |
| 结-环境热阻 | R<sub>th(j-a)</sub> | 40 | °C/W |

---

## 🔌 电学特性 (Electrical Characteristics)

### 1. 静态特性 (Static Characteristic, T<sub>j</sub> = 25 °C 除非特别声明)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极击穿电压 | V<sub>(BR)CES</sub> | V<sub>GE</sub>=0 V, I<sub>C</sub>=0.5 mA | 650 | - | - | V |
| 集电极-发射极饱和电压 | V<sub>CE(sat)</sub> | V<sub>GE</sub>=15 V, I<sub>C</sub>=80 A, T<sub>j</sub>=25 °C<br>V<sub>GE</sub>=15 V, I<sub>C</sub>=80 A, T<sub>j</sub>=150 °C | - | 1.7<br>2.0 | 2.1<br>- | V |
| 二极管正向导通电压 | V<sub>F</sub> | V<sub>GE</sub>=0 V, I<sub>F</sub>=80 A, T<sub>j</sub>=25 °C<br>V<sub>GE</sub>=0 V, I<sub>F</sub>=80 A, T<sub>j</sub>=150 °C | - | 1.7<br>1.4 | 2.1<br>- | V |
| 栅极-发射极阈值电压 | V<sub>GE(th)</sub> | I<sub>C</sub>=1 mA, V<sub>CE</sub>=V<sub>GE</sub> | 2.0 | 2.8 | 4.0 | V |
| 集电极-发射极截止电流 | I<sub>CES</sub> | V<sub>CE</sub>=650 V, V<sub>GE</sub>=0 V | - | - | 100 | μA |
| 栅极-发射极漏电流 | I<sub>GES</sub> | V<sub>CE</sub>=0 V, V<sub>GE</sub>=±20 V | -200 | - | 200 | nA |

### 2. 动态特性 (Dynamic Characteristic)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :---: | :--- | :---: | :---: |
| 输入电容 | C<sub>ies</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz | 5777 | pF |
| 输出电容 | C<sub>oes</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz | 271 | pF |
| 反向传输电容 | C<sub>res</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz | 10 | pF |
| 门极总电量 | Q<sub>G</sub> | V<sub>CC</sub>=400 V, I<sub>C</sub>=80 A, V<sub>GE</sub>=15 V | 240 | nC |

---

## 🔄 开关特性 (Switching Characteristics)

### 1. T<sub>j</sub> = 25 °C 时开关特性（感性负载）
测试条件：V<sub>CC</sub>=400 V, I<sub>C</sub>=80 A, V<sub>GE</sub>=-7.5/15 V, R<sub>G</sub>=8 Ω

| 参数分类 | 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :--- | :---: | :---: | :---: |
| **IGBT 特性** | 开通延迟时间 (Turn-on delay time) | t<sub>d(on)</sub> | 3.5 | ns |
| | 上升时间 (Rise time) | t<sub>r</sub> | 95 | ns |
| | 关断延迟时间 (Turn-off delay time) | t<sub>d(off)</sub> | 104 | ns |
| | 下降时间 (Fall time) | t<sub>f</sub> | 79 | ns |
| | 开通损耗 (Turn-on energy)* | E<sub>on</sub> | 2.98 | mJ |
| | 关断损耗 (Turn-off energy) | E<sub>off</sub> | 1.95 | mJ |
| | 总开关损耗 (Total switching energy) | E<sub>ts</sub> | 4.93 | mJ |
| **反并联二极管** | 反向恢复时间 (Reverse recovery time) | t<sub>rr</sub> | 123 | ns |
| | 恢复电荷 (Recovered charge) | Q<sub>rr</sub> | 1.8 | μC |
| | 反向恢复峰值电流 (Peak reverse recovery current) | I<sub>RM</sub> | 21.6 | A |
| | 反向恢复损耗 (Reverse recovered energy) | E<sub>rec</sub> | 0.54 | mJ |

*\*注：开通损耗 E<sub>on</sub> 与总损耗 E<sub>ts</sub> 包含二极管反向恢复引起的额外损耗。*

### 2. T<sub>j</sub> = 150 °C 时开关特性（感性负载）
测试条件：V<sub>CC</sub>=400 V, I<sub>C</sub>=80 A, V<sub>GE</sub>=-7.5/15 V, R<sub>G</sub>=8 Ω

| 参数分类 | 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :--- | :---: | :---: | :---: |
| **IGBT 特性** | 开通延迟时间 (Turn-on delay time) | t<sub>d(on)</sub> | 4.0 | ns |
| | 上升时间 (Rise time) | t<sub>r</sub> | 93 | ns |
| | 关断延迟时间 (Turn-off delay time) | t<sub>d(off)</sub> | 122 | ns |
| | 下降时间 (Fall time) | t<sub>f</sub> | 83 | ns |
| | 开通损耗 (Turn-on energy)* | E<sub>on</sub> | 4.72 | mJ |
| | 关断损耗 (Turn-off energy) | E<sub>off</sub> | 2.35 | mJ |
| | 总开关损耗 (Total switching energy) | E<sub>ts</sub> | 7.07 | mJ |
| **反并联二极管** | 反向恢复时间 (Reverse recovery time) | t<sub>rr</sub> | 217 | ns |
| | 恢复电荷 (Recovered charge) | Q<sub>rr</sub> | 6.4 | μC |
| | 反向恢复峰值电流 (Peak reverse recovery current) | I<sub>RM</sub> | 47.6 | A |
| | 反向恢复损耗 (Reverse recovered energy) | E<sub>rec</sub> | 1.75 | mJ |

---

## 📐 封装外形尺寸 (TO-247 Outline Dimensions)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

| 符号 (Symbol) | 最小值 (Min.) | 最大值 (Max.) | 符号 (Symbol) | 最小值 (Min.) | 最大值 (Max.) |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **A** | 4.70 | 5.30 | **E1** | 13.60 | 14.10 |
| **A1** | 2.20 | 2.60 | **e** | 5.40 | 5.50 |
| **A2** | 1.80 | 2.20 | **L** | 19.80 | 20.30 |
| **b** | 1.00 | 1.35 | **L1** | 3.80 | 4.40 |
| **b1** | 1.80 | 2.20 | **ΦP** | 3.60 | 3.70 |
| **b2** | 2.60 | 3.25 | **Q** | 5.60 | 5.80 |
| **c** | 0.50 | 0.70 | **S** | 6.10 | 6.30 |
| **D** | 20.80 | 21.20 | **θ** | 5° | 11° |
| **E** | 15.60 | 16.00 | | | |

*\*备注：因各封装厂的模具存在细微差异，请以实物尺寸为准。*

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Packing) | 每管数量 (pcs/tube) | 每盒管数 (tube/inner box) | 每箱盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| 管装 (Tube) | 30 | 12 | 6 | 2160 |

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
