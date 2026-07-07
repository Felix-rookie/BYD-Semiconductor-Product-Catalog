# 比亚迪半导体 (BYD) 工业级 IGBT 半桥模块 - BG200B12UY3-I

[![Package](https://img.shields.io/badge/Package-62mm%20Industrial-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BG200B12UY3-I** 是一款采用先进 IGBT 芯片、FRD 芯片和优化电气连接设计的硅基工业级 IGBT 半桥模块。该模块具有快速开关特性、高短路耐量和低电感设计，适用于高频驱动器、伺服系统和 UPS 等高可靠性功率变换场景。

### 🌟 核心特性 (Features)
* **半桥拓扑**：工业级半桥模块 (Half-bridge module)，额定 V<sub>CES</sub>=1200 V、I<sub>C</sub>=200 A。
* **高速 IGBT 技术**：快速开关特性与短尾电流，低电感设计。
* **续流卓越**：并联超快软恢复续流二极管 (Ultra fast & soft recovery anti-parallel FWD)。
* **强韧动态特性**：具备高短路耐受能力，短路安全工作区 t<sub>psc</sub>=10 μs。
* **工业封装**：106.4 × 61.4 × 31.5 mm 工业模块封装，标准螺栓安装。

### 🚗 典型应用 (Applications)
* 高频驱动器 (High Frequency Drivers)
* 交流电机控制 (AC Motor Control)
* 逆变器 (Inverters)
* 伺服系统 (Servo)
* 不间断电源 (UPS)
* 电焊机 (Electric Welding)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 (V<sub>CES</sub>) | 额定公称电流 (I<sub>C(nom)</sub>) | 典型饱和电压 (V<sub>CE(sat)</sub>) | 最高工作结温 (T<sub>jmax</sub>) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BG200B12UY3-I** | 1200 V | 200 A | 2.8 V | 150 °C | 半桥 (Half-Bridge) | 62mm 工业封装 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>vj</sub>=25 °C，除非另外注明）

### 1. IGBT 逆变部分 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 集电极-发射极电压 | V<sub>CES</sub> | V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C | 1200 | V |
| 连续集电极直流电流 | I<sub>C</sub> | T<sub>C</sub>=80 °C | 200 | A |
| 集电极重复峰值电流 | I<sub>CRM</sub> | I<sub>CRM</sub>=2×I<sub>C</sub>, t<sub>p</sub>=1 ms | 400 | A |
| 栅极-发射极电压 | V<sub>GES</sub> | — | ±20 | V |
| 总耗散功率 | P<sub>tot</sub> | 每开关 (per IGBT), T<sub>C</sub>=25 °C | 1041 | W |
| 短路安全工作区 | t<sub>psc</sub> | V<sub>CC</sub>=600 V, V<sub>GE</sub>≤15 V, V<sub>CES</sub>≤1200 V, T<sub>vj</sub>≤125 °C | 10 | μs |

### 2. 续流二极管部分 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 二极管连续正向直流电流 | I<sub>F</sub> | T<sub>C</sub>=80 °C | 200 | A |
| 二极管重复峰值正向电流 | I<sub>FRM</sub> | I<sub>FRM</sub>=2×I<sub>F</sub>, t<sub>p</sub>=1 ms | 400 | A |

### 3. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 绝缘测试电压 | V<sub>isol</sub> | f=50 Hz, t=1 min, 正弦波交流 | AC 2500 | V |
| 最大结温 | T<sub>vjmax</sub> | — | 150 | °C |
| 工作结温 | T<sub>vj op</sub> | — | -40 ~ 125 | °C |
| 存储温度 | T<sub>stg</sub> | — | -40 ~ 125 | °C |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件/说明 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| IGBT 结-外壳热阻 | R<sub>th(j-c)</sub> | 每个 IGBT (per IGBT) | — | 0.12 | — | K/W |
| 二极管结-外壳热阻 | R<sub>th(j-c)</sub> | 每个二极管 (per diode) | — | 0.2 | — | K/W |
| 外壳-散热片热阻 | R<sub>th(c-s)</sub> | 每个模块 (per module) | — | 0.03 | — | K/W |
| 外形尺寸 | L × W × H | — | — | 106.4 × 61.4 × 31.5 | — | mm |
| 爬电距离 | d<sub>s</sub> | 端子到端子 (Terminal to terminal) | — | 14 | — | mm |
| 爬电距离 | d<sub>s</sub> | 端子到底板 (Terminal to base) | — | 24 | — | mm |
| 空气间隙 | d<sub>a</sub> | 端子到端子 (Terminal to terminal) | 6.0 | — | — | mm |
| 空气间隙 | d<sub>a</sub> | 端子到底板 (Terminal to base) | — | 28.3 | — | mm |
| 重量 | m | — | — | 320 | — | g |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. IGBT 静态与动态特性 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极饱和压降 | V<sub>CE(sat)</sub> | I<sub>C</sub>=200 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=25 °C<br>I<sub>C</sub>=200 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=125 °C | —<br>— | 2.8<br>3.5 | —<br>— | V |
| 栅极阈值电压 | V<sub>GE(th)</sub> | V<sub>CE</sub>=V<sub>GE</sub>, I<sub>C</sub>=3 mA, T<sub>vj</sub>=25 °C | 5.0 | 5.8 | 6.5 | V |
| 集电极-发射极截止电流 | I<sub>CES</sub> | V<sub>CE</sub>=1200 V, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C | —<br>— | —<br>— | 1<br>10 | mA |
| 栅极-发射极漏电流 | I<sub>GES</sub> | V<sub>CE</sub>=0 V, V<sub>GE</sub>=±20 V, T<sub>vj</sub>=25 °C | -400 | — | 400 | nA |
| 栅极电荷 | Q<sub>g</sub> | V<sub>CE</sub>=600 V, I<sub>C</sub>=200 A, V<sub>GE</sub>=0 V…+15 V | — | 1.28 | — | μC |
| 栅极-发射极电荷 | Q<sub>ge</sub> | — | — | 0.22 | — | μC |
| 栅极-集电极电荷 | Q<sub>gc</sub> | — | — | 0.80 | — | μC |
| 内部栅极电阻 | R<sub>Gint</sub> | T<sub>vj</sub>=25 °C | — | 1.5 | — | Ω |
| 输入电容 | C<sub>ies</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz, T<sub>vj</sub>=25 °C | — | 12.8 | — | nF |
| 输出电容 | C<sub>oes</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz, T<sub>vj</sub>=25 °C | — | 7.5 | — | nF |
| 反向传输电容 | C<sub>res</sub> | V<sub>CE</sub>=25 V, V<sub>GE</sub>=0 V, f=1 MHz, T<sub>vj</sub>=25 °C | — | 9.3 | — | nF |

### 2. IGBT 开关损耗特性 (IGBT-Inverter, 感性负载测试)
测试条件：V<sub>CC</sub>=600 V, I<sub>C</sub>=200 A, V<sub>GE</sub>=±15 V, R<sub>Gon</sub>=R<sub>Goff</sub>=3.3 Ω, L<sub>σ</sub>=80 nH, 感性负载 (Inductive load)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C | —<br>— | 224<br>210 | —<br>— | ns |
| 上升时间 | t<sub>r</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C | —<br>— | 91<br>84 | —<br>— | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C | —<br>— | 400<br>460 | —<br>— | ns |
| 下降时间 | t<sub>f</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C | —<br>— | 140<br>200 | —<br>— | ns |
| 开通损耗能量 | E<sub>on</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C | —<br>— | 13.9<br>17.8 | —<br>— | mJ |
| 关断损耗能量 | E<sub>off</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=125 °C | —<br>— | 10.9<br>15.8 | —<br>— | mJ |

### 3. 续流二极管特性 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 正向电压 | V<sub>F</sub> | I<sub>F</sub>=200 A, T<sub>vj</sub>=25 °C<br>I<sub>F</sub>=200 A, T<sub>vj</sub>=125 °C | —<br>— | 1.8<br>1.8 | —<br>— | V |
| 反向恢复峰值电流 | I<sub>RR</sub> | I<sub>F</sub>=200 A, V<sub>R</sub>=600 V, di<sub>F</sub>/dt=1100 A/μs, T<sub>vj</sub>=125 °C | — | 160 | — | A |
| 恢复电荷 | Q<sub>rr</sub> | I<sub>F</sub>=200 A, V<sub>R</sub>=600 V, di<sub>F</sub>/dt=1100 A/μs, T<sub>vj</sub>=125 °C | — | 28.4 | — | μC |
| 反向恢复时间 | t<sub>rr</sub> | I<sub>F</sub>=200 A, V<sub>R</sub>=600 V, di<sub>F</sub>/dt=1100 A/μs, T<sub>vj</sub>=125 °C | — | 370 | — | ns |
| 反向恢复损耗 | E<sub>rec</sub> | I<sub>F</sub>=200 A, V<sub>R</sub>=600 V, di<sub>F</sub>/dt=1100 A/μs, T<sub>vj</sub>=125 °C | — | 10.5 | — | mJ |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

封装外形尺寸：106.4 × 61.4 × 31.5 mm。所有公制尺寸单位均默认为：**毫米 (Millimeter)**。

---

## 📦 安全操作与存储须知 (Safety & Storage)

* **运输与存储**：包装箱颠簸或坠落可能导致内部器件损毁，器件遇水受潮会导致失效。
* **存储条件**：存储地点温度与湿度建议分别控制在 20 ± 5 °C 和 30~60%。
* **长期存储**：存储超过一年需采取去湿措施，使用前请检查外观是否存在刮伤、灰尘或锈迹。
* **防静电措施**：安装和焊接过程中应保持设备与人体接地，避免栅极端子承受静电或过电压。

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
