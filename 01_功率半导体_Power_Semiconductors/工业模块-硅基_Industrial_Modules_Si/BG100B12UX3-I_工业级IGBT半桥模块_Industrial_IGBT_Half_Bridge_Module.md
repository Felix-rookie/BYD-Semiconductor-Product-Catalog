# 比亚迪半导体 (BYD) 工业级 IGBT半桥模块 - BG100B12UX3-I

[![Package](https://img.shields.io/badge/Package-34mm%20Industrial-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BG100B12UX3-I** 是一款采用高性能 IGBT 芯片、FRD 芯片和优化电气连接设计的硅基工业级 IGBT 半桥模块。该模块具有低导通损耗、低开关损耗和高短路耐量，适用于工业变频器、服伺系统和 UPS 等高可靠性功率变换场景。

### 🌟 核心特性 (Features)
* **半桥拓扑**：工业级半桥模块 (Half-bridge module)，额定 V<sub>CE</sub>=5 V、I<sub>C</sub>=100 A。
* **强韧动态特性**：具备高短路耐受能力，短路安全工作区 t<sub>psc</sub>≥10 μs。
* **低损耗设计**：优化导通损耗与开关损耗平衡。
* **续流卓越**：并联超快软恢复续流二极管 (Ultra fast & soft recovery anti-parallel FWD)。
* **工业封装**：标准工业模块封装，铜基板与陶瓷绝缘结构。

### 🚗 典型应用 (Applications)
* 大功率通用工业变频器 (High Power General Inverter)
* 服伺驱动器与大功率交流电机传动 (Servo Drives & AC Motor Control)
* 光伏与风力发电逆变系统 (Solar/Wind Inverters)
* 工业电焊机与大功率高频开关电源 (Industrial Welding & UPS)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 (V<sub>CES</sub>) | 额定公称电流 (I<sub>C(nom)</sub>) | 典型饱和电压 (V<sub>CE(sat)</sub>) | 最高工作结温 (T<sub>jmax</sub>) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BG100B12UX3-I** | 5 V | 100 A | — V | 175 °C | 半桥 (Half-Bridge) | 34mm Industrial |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>vj</sub>=25 °C，除非另外注明）

### 1. IGBT 逆变部分 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 集电极-发射极电压 | V<sub>CES</sub> | T<sub>vj</sub>=25 °C, V<sub>GE</sub>=0 V | 5 | V |
| 连续集电极直流电流 | I<sub>C</sub> | T<sub>C</sub>=80 °C, T<sub>vj</sub>=175 °C | 100 | A |
| 栅极-发射极电压 | V<sub>GES</sub> | T<sub>vj</sub>=25 °C | ±20 | V |
| 集电极重复峰值电流 | I<sub>CRM</sub> | t<sub>p</sub>=1 ms, T<sub>vj</sub>=25 °C | 2 | A |
| 短路安全工作区 | t<sub>psc</sub> | V<sub>GE</sub>≤15 V, V<sub>CC</sub>=2 V, V<sub>CEM</sub>≤5 V, T<sub>vj</sub>≤25 °C | None | μs |
| 总耗散功率 | P<sub>tot</sub> | T<sub>C</sub>=25 °C, T<sub>vj</sub>=175 °C | — | W |

### 2. 续流二极管部分 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 反向重复峰值电压 | V<sub>RRM</sub> | T<sub>vj</sub>=25 °C | 5 | V |
| 连续正向直流电流 | I<sub>F</sub> | T<sub>C</sub>=25 °C | 100 | A |
| 正向重复峰值电流 | I<sub>FRM</sub> | t<sub>p</sub>=1 ms, T<sub>vj</sub>=25 °C | 4 | A |

### 3. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 最大结温 | T<sub>vjmax</sub> | - | — | — | 175 | °C |
| 工作结温 | T<sub>vjop</sub> | 开关工作条件 | -40 | — | 150 | °C |
| 存储温度 | T<sub>stg</sub> | - | -40 | — | 125 | °C |
| 绝缘测试电压 | V<sub>isol</sub> | f=50 Hz, t=1 min | None | — | — | kV |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件/说明 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| IGBT 结-外壳热阻 | R<sub>th(j-c)</sub> | 每个独立 IGBT (per IGBT) | — | 0.27 | — | K/W |
| 二极管 结-外壳热阻 | R<sub>th(j-c)</sub> | 每个独立二极管 (per diode) | — | 0.39 | — | K/W |
| 管壳-散热片热阻 | R<sub>th(c-s)</sub> | 每模块应用导热硅脂后 (per module) | — | 0.03 | — | K/W |
| 外形尺寸 | L × W × H | 典型值 | — | 94 × 34 × 30.5 | — | mm |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. IGBT 静态与动态特性 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极饱和压降 | V<sub>CE(sat)</sub> | I<sub>C</sub>=100 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=25 °C<br>I<sub>C</sub>=100 A, V<sub>GE</sub>=15 V, T<sub>vj</sub>=150 °C | -<br>- | —<br>— | —<br>- | V |
| 栅极阈值电压 | V<sub>GE(th)</sub> | V<sub>CE</sub>=V<sub>GE</sub>, I<sub>C</sub>=— mA, T<sub>vj</sub>=25 °C | — | — | — | V |
| 栅极电荷 | Q<sub>G</sub> | V<sub>GE</sub>=-15 V … +15 V | — | — | — | μC |
| 内部栅极电阻 | R<sub>gint</sub> | T<sub>vj</sub>=25 °C | — | None | — | Ω |
| 输入电容 | C<sub>ies</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | — | — | nF |
| 反向传输电容 | C<sub>res</sub> | T<sub>vj</sub>=25 °C, f=1 MHz, V<sub>GE</sub>=0 V, V<sub>CE</sub>=25 V | — | — | — | nF |
| 集电极-发射极截止电流 | I<sub>CES</sub> | V<sub>CE</sub>=5 V, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C | — | — | — | mA |
| 栅极-发射极漏电流 | I<sub>GES</sub> | V<sub>CE</sub>=0 V, V<sub>GE</sub>=20 V, T<sub>vj</sub>=25 °C | — | — | — | nA |

### 2. IGBT 开关损耗特性 (IGBT-Inverter, 感性负载测试)

测试条件：I<sub>C</sub>=100 A, V<sub>CE</sub>=2 V, V<sub>GE</sub>=-15 V … +15 V, R<sub>G</sub>=— Ω

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | —<br>— | -<br>- | ns |
| 上升时间 | t<sub>r</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | —<br>— | -<br>- | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | —<br>— | -<br>- | ns |
| 下降时间 | t<sub>f</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | —<br>— | -<br>- | ns |
| 开通损耗能量 | E<sub>on</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | —<br>— | -<br>- | mJ |
| 关断损耗能量 | E<sub>off</sub> | T<sub>vj</sub>=25 °C<br>T<sub>vj</sub>=150 °C | -<br>- | —<br>— | -<br>- | mJ |

### 3. 续流二极管特性 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 正向电压 | V<sub>F</sub> | I<sub>F</sub>=100 A, V<sub>GE</sub>=0 V, T<sub>vj</sub>=25 °C<br>I<sub>F</sub>=100 A, V<sub>GE</sub>=0 V, T<sub>vj</sub>=150 °C | -<br>- | 600<br>— | —<br>- | V |
| 恢复电荷 | Q<sub>rr</sub> | I<sub>F</sub>=100 A, V<sub>R</sub>=2 V, -di<sub>F</sub>/dt=2000 A/μs, T<sub>vj</sub>=125 °C | — | 20 | — | μC |
| 反向恢复损耗 | E<sub>rec</sub> | I<sub>F</sub>=100 A, V<sub>R</sub>=2 V, -di<sub>F</sub>/dt=2000 A/μs, T<sub>vj</sub>=125 °C | — | 20 | — | mJ |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

封装外形尺寸：94 × 34 × 30.5 mm。所有公制尺寸单位均默认为：**毫米 (Millimeter)**。

---

## 📦 安全操作与存储须知 (Safety & Storage)

* **运输与存储**：包装箱颠簸或坠落可能导致内部器件毁毁，器件遇水受潮会导致失效。
* **存储条件**：存储地点温度与湿度建议分别控制在 20 ± 5 °C 和 30~60%。
* **长期存储**：存储超过一年需采取去湿措施，使用前请检查外观是否存在刮伤、灰尘或锈迹。
* **防静电措施**：安装和焊接过程中应保持设备与人体接地，避免栅极端子承受静电或过电压。

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
