# 比亚迪半导体 (BYD) 工业级 IGBT维也纳三电平模块 - BG30T07N10H5

[![Package](https://img.shields.io/badge/Package-miniPACK™2-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Preliminary-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BG30T07N10H5** 是一款由比亚迪半导体设计开发的 mini 封装维也纳三电平模块。该产品具有封装小、集成度高等优点，模块集成温度检测，可快速响应及温度实时输出，适用于空调等变频家电应用。

### 🌟 核心特性 (Features)
* **维也纳三电平拓扑**：mini 封装维也纳三电平模块，额定 V<sub>CE</sub>=650 V、I<sub>C</sub>=30 A。
* **高度集成**：集成温度检测功能，可快速响应并实时温度输出。
* **低热阻**：采用 DBC 陶瓷覆铜板，低热阻设计。
* **高速开关**：采用第五代 IGBT 芯片技术，适合高频应用。

### 🚗 典型应用 (Applications)
* 空调等变频家电 (Home Appliances like Air Condition)
* 维也纳三电平PFC (Vienna 3-Level PFC)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 (V<sub>CES</sub>) | 额定公称电流 (I<sub>C(nom)</sub>) | 典型饱和电压 (V<sub>CE(sat)</sub>) | 最高工作结温 (T<sub>jmax</sub>) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BG30T07N10H5** | 650 V | 30 A | 1.9 V | 175 °C | 维也纳三电平 (Vienna-Three-Level) | miniPACK™2 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>vj</sub>=25 °C，除非另外注明）

### 1. IGBT 逆变部分 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 集电极-发射极电压 | V<sub>CES</sub> | T<sub>vj</sub>=25 °C, V<sub>GE</sub>=0 V | 650 | V |
| 连续集电极直流电流 | I<sub>C</sub> | T<sub>C</sub>=80 °C, T<sub>vj</sub>=175 °C | 30 | A |
| 栅极-发射极电压 | V<sub>GES</sub> | T<sub>vj</sub>=25 °C | ±20 | V |
| 集电极重复峰值电流 | I<sub>CRM</sub> | t<sub>p</sub>=1 ms, T<sub>vj</sub>=25 °C | 60 | A |
| 总耗散功率 | P<sub>tot</sub> | T<sub>C</sub>=25 °C, T<sub>vj</sub>=175 °C | — | W |

### 2. 续流二极管部分 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 反向重复峰值电压 | V<sub>RRM</sub> | T<sub>vj</sub>=25 °C | 650 | V |
| 连续正向直流电流 | I<sub>F</sub> | T<sub>C</sub>=25 °C | 30 | A |
| 正向重复峰值电流 | I<sub>FRM</sub> | t<sub>p</sub>=1 ms, T<sub>vj</sub>=25 °C | 120 | A |
| I²t-值 | I²t | V<sub>R</sub>=0 V, t<sub>p</sub>=10 ms, T<sub>vj</sub>=125 °C | None | A²s |

### 3. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 最大结温 | T<sub>vjmax</sub> | - | — | — | 175 | °C |
| 工作结温 | T<sub>vjop</sub> | 开关工作条件 | -40 | — | 150 | °C |
| 存储温度 | T<sub>stg</sub> | - | -40 | — | 125 | °C |
| 绝缘测试电压 | V<sub>isol</sub> | f=50 Hz, t=1 min | 2.5 | — | — | kV |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件/说明 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| IGBT 结-外壳热阻 | R<sub>th(j-c)</sub> | 每个独立 IGBT (per IGBT) | — | 0.617 | — | K/W |
| 二极管 结-外壳热阻 | R<sub>th(j-c)</sub> | 每个独立二极管 (per diode) | — | 0.665 | — | K/W |
| 管壳-散热片热阻 | R<sub>th(c-s)</sub> | 每模块应用导热硅脂后 (per module) | — | — | — | K/W |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. IGBT 静态与动态特性 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极饱和压降 | V<sub>CE(sat)</sub> | I<sub>C</sub>=30 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=25 °C<br>I<sub>C</sub>=30 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=150 °C | -<br>- | 1.9<br>2.0 | —<br>- | V |
| 栅极阈值电压 | V<sub>GE(th)</sub> | V<sub>CE</sub>=V<sub>GE</sub>, I<sub>C</sub>=1 mA, T<sub>vj</sub>=25 °C | 5.0 | 5.8 | 7.0 | V |
| 栅极电荷 | Q<sub>G</sub> | V<sub>GE</sub>=-15 V … +15 V | — | 12 | — | μC |
| 内部栅极电阻 | R<sub>gint</sub> | T<sub>vj</sub>=25 °C | — | 12 | — | Ω |
| 输入电容 | C<sub>ies</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | 1.69 | — | nF |
| 反向传输电容 | C<sub>res</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | 0.13 | — | nF |
| 集电极-发射极截止电流 | I<sub>CES</sub> | V<sub>CE</sub>=650 V, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C | — | — | — | mA |
| 栅极-发射极漏电流 | I<sub>GES</sub> | V<sub>CE</sub>=0 V, V<sub>GE</sub>=20 V, T<sub>vj</sub>=25 °C | — | — | — | nA |

### 2. IGBT 开关损耗特性 (IGBT-Inverter, 感性负载测试)

测试条件：I<sub>C</sub>=30 A, V<sub>CE</sub>=325 V, V<sub>GE</sub>=-15 V … +15 V, R<sub>G</sub>=— Ω

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | 24<br>20.9 | -<br>- | ns |
| 上升时间 | t<sub>r</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | 8<br>9 | -<br>- | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | 96<br>138 | -<br>- | ns |
| 下降时间 | t<sub>f</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | 38<br>38 | -<br>- | ns |
| 开通损耗能量 | E<sub>on</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | 0.41<br>0.74 | -<br>- | mJ |
| 关断损耗能量 | E<sub>off</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | 0.33<br>0.53 | -<br>- | mJ |

### 3. 续流二极管特性 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 正向电压 | V<sub>F</sub> | I<sub>F</sub>=30 A, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C<br>I<sub>F</sub>=30 A, V<sub>GE</sub>=0 V, T<sub>vj</sub>=150 °C | -<br>- | 1.2<br>1.3 | —<br>- | V |
| 恢复电荷 | Q<sub>rr</sub> | I<sub>F</sub>=30 A, V<sub>R</sub>=325 V, -di<sub>F</sub>/dt=— A/μs, T<sub>vj</sub>=125 °C | — | 1.7 | — | μC |
| 反向恢复损耗 | E<sub>rec</sub> | I<sub>F</sub>=30 A, V<sub>R</sub>=325 V, -di<sub>F</sub>/dt=— A/μs, T<sub>vj</sub>=125 °C | — | 0.32 | — | mJ |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**。

---

## 📦 安全操作与存储须知 (Safety & Storage)

* **运输与存储**：包装箱颠簸或坠落可能导致内部器件毁毁，器件遇水受潮会导致失效。
* **存储条件**：存储地点温度与湿度建议分别控制在 20 ± 5 °C 和 30~60%。
* **长期存储**：存储超过一年需采取去湿措施，使用前请检查外观是否存在刮伤、灰尘或锈迹。
* **防静电措施**：安装和焊接过程中应保持设备与人体接地，避免栅极端子承受静电或过电压。

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
