# 比亚迪半导体 (BYD) 工业级 IGBT PIM 模块 - BG150G12F13L4

[![Package](https://img.shields.io/badge/Package-EconoPIM%20Industrial-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Preliminary-yellow.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BG150G12F13L4** 是一款采用 1200V 平面栅场终止技术的硅基工业级 IGBT PIM（Converter Inverter Brake）模块。该模块集成三相整流桥、三相逆变 IGBT 和制动斩波 IGBT，具有低导通损耗、低开关损耗和高功率/温度循环能力，适用于辅助逆变器、伺服驱动器和电机传动等高可靠性功率变换场景。

*（注：该型号为初步数据 Preliminary Data）*

### 🌟 核心特性 (Features)
* **PIM 拓扑 (CIB)**：集成整流桥 (Converter)、三相逆变器 (Inverter)、制动斩波器 (Brake) 于一体。
* **1200V 平面栅场终止技术**：低导通和开关损耗，V<sub>CEsat</sub> 正温度系数易于并联。
* **强韧可靠性**：高功率循环和温度循环能力。
* **高集成度**：简化系统设计，节省安装空间。

### 🚗 典型应用 (Applications)
* 辅助逆变器 (Auxiliary Inverters)
* 伺服驱动器 (Servo Drives)
* 电机传动 (Motor Drives)
* 医疗应用 (Medical Applications)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 (V<sub>CES</sub>) | 额定公称电流 (I<sub>C(nom)</sub>) | 典型饱和电压 (V<sub>CE(sat)</sub>) | 最高工作结温 (T<sub>jmax</sub>) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BG150G12F13L4** | 1200 V | 150 A | 2.05 V | 175 °C | PIM (CIB) | EconoPIM 工业封装 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>vj</sub>=25 °C，除非另外注明）

### 1. IGBT 逆变部分 (IGBT, Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 集电极-发射极电压 | V<sub>CES</sub> | T<sub>vj</sub>=25 °C | 1200 | V |
| 连续集电极直流电流 | I<sub>C</sub> | T<sub>C</sub>=100 °C, T<sub>vjmax</sub>=175 °C | 150 | A |
| 栅极-发射极峰值电压 | V<sub>GES</sub> | — | ±20 | V |
| 集电极重复峰值电流 | I<sub>CRM</sub> | t<sub>p</sub>=1 ms | 300 | A |

### 2. 续流二极管部分 (Diode, Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 反向重复峰值电压 | V<sub>RRM</sub> | T<sub>vj</sub>=25 °C | 1200 | V |
| 连续正向直流电流 | I<sub>F</sub> | — | 150 | A |
| 正向重复峰值电流 | I<sub>FRM</sub> | t<sub>p</sub>=1 ms | 300 | A |
| I²t 值 | I²t | V<sub>R</sub>=0 V, t<sub>p</sub>=10 ms, T<sub>vj</sub>=125 °C | 2800 | A²s |

### 3. 整流二极管部分 (Diode, Rectifier)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 反向重复峰值电压 | V<sub>RRM</sub> | T<sub>vj</sub>=25 °C | 1600 | V |
| 最大正向均方根电流 (每芯片) | I<sub>FRMSM</sub> | T<sub>C</sub>=85 °C | 150 | A |
| 最大整流器输出均方根电流 | I<sub>RMSM</sub> | T<sub>C</sub>=85 °C | 150 | A |
| 正向浪涌电流 | I<sub>FSM</sub> | t<sub>p</sub>=10 ms, T<sub>vj</sub>=25 °C<br>t<sub>p</sub>=10 ms, T<sub>vj</sub>=150 °C | 1800<br>1600 | A |
| I²t 值 | I²t | t<sub>p</sub>=10 ms, T<sub>vj</sub>=25 °C<br>t<sub>p</sub>=10 ms, T<sub>vj</sub>=150 °C | 16000<br>13000 | A²s |

### 4. IGBT 制动-斩波器部分 (IGBT, Brake-Chopper)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 集电极-发射极电压 | V<sub>CES</sub> | T<sub>vj</sub>=25 °C | 1200 | V |
| 连续集电极直流电流 | I<sub>C</sub> | T<sub>C</sub>=100 °C, T<sub>vjmax</sub>=175 °C | 75 | A |
| 栅极-发射极峰值电压 | V<sub>GES</sub> | — | ±20 | V |
| 集电极重复峰值电流 | I<sub>CRM</sub> | t<sub>p</sub>=1 ms | 150 | A |

### 5. 制动-斩波器二极管部分 (Diode, Brake-Chopper)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 反向重复峰值电压 | V<sub>RRM</sub> | T<sub>vj</sub>=80 °C | 1200 | V |

### 6. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 最大结温 | T<sub>vjmax</sub> | — | 175 | °C |
| 工作结温 | T<sub>vjop</sub> | 开关工作条件 | -40 ~ 150 | °C |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件/说明 (Conditions) | 典型值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| **逆变 IGBT** 结-外壳热阻 | R<sub>thJC</sub> | 每个 IGBT (per IGBT) | 0.17 | K/W |
| **逆变 IGBT** 外壳-散热器热阻 | R<sub>thCH</sub> | λ<sub>Paste</sub>=1 W/(m·K) | 0.0732 | K/W |
| **逆变二极管** 结-外壳热阻 | R<sub>thJC</sub> | 每个二极管 (per diode) | 0.25 | K/W |
| **逆变二极管** 外壳-散热器热阻 | R<sub>thCH</sub> | λ<sub>Paste</sub>=1 W/(m·K) | 0.1 | K/W |
| **整流二极管** 结-外壳热阻 | R<sub>thJC</sub> | 每个二极管 (per diode) | 0.254 | K/W |
| **整流二极管** 外壳-散热器热阻 | R<sub>thCH</sub> | λ<sub>Paste</sub>=1 W/(m·K) | 0.0866 | K/W |
| **制动 IGBT** 结-外壳热阻 | R<sub>thJC</sub> | 每个 IGBT (per IGBT) | 0.3 | K/W |
| **制动 IGBT** 外壳-散热器热阻 | R<sub>thCH</sub> | λ<sub>Paste</sub>=1 W/(m·K) | 0.15 | K/W |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. IGBT 静态与动态特性 (IGBT, Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极饱和压降 | V<sub>CE(sat)</sub> | I<sub>C</sub>=150 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=25 °C<br>I<sub>C</sub>=150 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=125 °C<br>I<sub>C</sub>=150 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=150 °C | —<br>—<br>— | 2.05<br>2.41<br>2.47 | 2.40<br>—<br>— | V |
| 栅极阈值电压 | V<sub>GE(th)</sub> | V<sub>CE</sub>=V<sub>GE</sub>, I<sub>C</sub>=4 mA, T<sub>vj</sub>=25 °C | 5.0 | 5.9 | 7.0 | V |
| 栅极电荷 | Q<sub>G</sub> | V<sub>GE</sub>=-7.5 V…+15 V | — | 0.7 | — | μC |
| 内部栅极电阻 | R<sub>Gint</sub> | T<sub>vj</sub>=25 °C | — | 6 | — | Ω |
| 输入电容 | C<sub>ies</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | 6.2 | — | nF |
| 反向传输电容 | C<sub>res</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | 0.32 | — | nF |
| 集电极-发射极截止电流 | I<sub>CES</sub> | V<sub>CE</sub>=1200 V, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C | — | — | 1000 | μA |
| 栅极-发射极漏电流 | I<sub>GES</sub> | V<sub>CE</sub>=0 V, V<sub>GE</sub>=20 V, T<sub>vj</sub>=25 °C | — | — | 1000 | nA |
| 短路耐受电流 | I<sub>SC</sub> | V<sub>GE</sub>≤15 V, V<sub>CC</sub>=800 V, t<sub>p</sub>≤10 μs, T<sub>vj</sub>=150 °C | — | 600 | — | A |

#### 逆变 IGBT 开关损耗特性 (感性负载测试)
测试条件：I<sub>C</sub>=150 A, V<sub>CE</sub>=600 V, V<sub>GE</sub>=-7.5 V…+15 V, R<sub>Gon</sub>=R<sub>Goff</sub>=6.7 Ω

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 110<br>129<br>130 | —<br>—<br>— | ns |
| 上升时间 | t<sub>r</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 87<br>90<br>92 | —<br>—<br>— | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 280<br>292<br>303 | —<br>—<br>— | ns |
| 下降时间 | t<sub>f</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 209<br>216<br>225 | —<br>—<br>— | ns |
| 开通损耗能量 | E<sub>on</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 14.7<br>22.6<br>24.5 | —<br>—<br>— | mJ |
| 关断损耗能量 | E<sub>off</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 9.4<br>12.2<br>13.7 | —<br>—<br>— | mJ |

### 2. 续流二极管特性 (Diode, Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 正向电压 | V<sub>F</sub> | I<sub>F</sub>=150 A, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C<br>I<sub>F</sub>=150 A, V<sub>GE</sub>=0 V, T<sub>vj</sub>=125 °C<br>I<sub>F</sub>=150 A, V<sub>GE</sub>=0 V, T<sub>vj</sub>=150 °C | 1.70<br>—<br>— | 2.15<br>2.20<br>2.15 | 2.50<br>—<br>— | V |
| 反向恢复峰值电流 | I<sub>RM</sub> | I<sub>F</sub>=150 A, -di<sub>F</sub>/dt=800 A/μs, V<sub>R</sub>=600 V, V<sub>GE</sub>=-7.5 V, T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 64<br>87<br>89 | —<br>—<br>— | A |
| 恢复电荷 | Q<sub>r</sub> | 同上 | —<br>—<br>— | 8.6<br>18.9<br>21.3 | —<br>—<br>— | μC |
| 反向恢复损耗 | E<sub>rec</sub> | 同上 | —<br>—<br>— | 2.18<br>4.81<br>5.50 | —<br>—<br>— | mJ |

### 3. 整流二极管特性 (Diode, Rectifier)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 正向电压 | V<sub>F</sub> | I<sub>F</sub>=150 A, T<sub>vj</sub>=150 °C | — | 1.24 | — | V |
| 反向电流 | I<sub>R</sub> | V<sub>R</sub>=1600 V, T<sub>vj</sub>=25 °C<br>V<sub>R</sub>=1600 V, T<sub>vj</sub>=150 °C | —<br>— | 10<br>2 | —<br>— | μA<br>mA |

### 4. IGBT 制动-斩波器特性 (IGBT, Brake-Chopper)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极饱和压降 | V<sub>CE(sat)</sub> | I<sub>C</sub>=75 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=25 °C<br>I<sub>C</sub>=75 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=125 °C<br>I<sub>C</sub>=75 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=150 °C | —<br>—<br>— | 2.05<br>2.39<br>2.45 | 2.40<br>—<br>— | V |
| 栅极阈值电压 | V<sub>GE(th)</sub> | V<sub>CE</sub>=V<sub>GE</sub>, I<sub>C</sub>=2 mA, T<sub>vj</sub>=25 °C | 5.0 | 6.0 | 7.0 | V |
| 栅极电荷 | Q<sub>G</sub> | V<sub>GE</sub>=-7.5 V…+15 V | — | 0.25 | — | μC |
| 内部栅极电阻 | R<sub>Gint</sub> | T<sub>vj</sub>=25 °C | — | 4 | — | Ω |
| 输入电容 | C<sub>ies</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | 1.69 | — | nF |
| 反向传输电容 | C<sub>res</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | 0.13 | — | nF |
| 集电极-发射极截止电流 | I<sub>CES</sub> | V<sub>CE</sub>=1200 V, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C | — | — | 100 | μA |
| 栅极-发射极漏电流 | I<sub>GES</sub> | V<sub>CE</sub>=0 V, V<sub>GE</sub>=20 V, T<sub>vj</sub>=25 °C | — | — | 200 | nA |
| 短路耐受电流 | I<sub>SC</sub> | V<sub>GE</sub>≤15 V, V<sub>CC</sub>=800 V, t<sub>p</sub>≤10 μs, T<sub>vj</sub>=150 °C | — | 300 | — | A |

#### 制动 IGBT 开关损耗特性 (感性负载测试)
测试条件：I<sub>C</sub>=75 A, V<sub>CE</sub>=600 V, V<sub>GE</sub>=-8 V…+15 V, R<sub>Gon</sub>=R<sub>Goff</sub>=6.7 Ω

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 101<br>110<br>113 | —<br>—<br>— | ns |
| 上升时间 | t<sub>r</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 77<br>82<br>85 | —<br>—<br>— | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 222<br>266<br>278 | —<br>—<br>— | ns |
| 下降时间 | t<sub>f</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 101<br>184<br>215 | —<br>—<br>— | ns |
| 开通损耗能量 | E<sub>on</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 7.5<br>9.9<br>10.9 | —<br>—<br>— | mJ |
| 关断损耗能量 | E<sub>off</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C<br>T<sub>vj</sub>=150 °C | —<br>—<br>— | 3.3<br>5.5<br>6.2 | —<br>—<br>— | mJ |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

*模块采用 EconoPIM 工业封装，具体外形尺寸请参考官方规格书。所有公制尺寸单位均默认为：**毫米 (Millimeter)**。*

---

## 📦 安全操作与存储须知 (Safety & Storage)

* **运输与存储**：包装箱颠簸或坠落可能导致内部器件损毁，器件遇水受潮会导致失效。
* **存储条件**：存储地点温度与湿度建议分别控制在 20 ± 5 °C 和 30~60%。
* **长期存储**：存储超过一年需采取去湿措施，使用前请检查外观是否存在刮伤、灰尘或锈迹。
* **防静电措施**：安装和焊接过程中应保持设备与人体接地，避免栅极端子承受静电或过电压。

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
