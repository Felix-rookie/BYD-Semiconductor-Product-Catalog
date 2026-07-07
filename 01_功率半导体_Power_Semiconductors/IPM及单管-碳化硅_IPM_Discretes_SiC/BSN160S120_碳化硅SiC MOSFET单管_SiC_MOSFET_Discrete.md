# 比亚迪半导体 (BYD) 碳化硅 (SiC) MOSFET 单管 - BSN160S120

[![Technology](https://img.shields.io/badge/Technology-SiC_MOSFET-green.svg)]()
[![Standard](https://img.shields.io/badge/Standard-Automotive__Grade-orange.svg)]()
[![Package](https://img.shields.io/badge/Package-TO-247-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BSN160S120** 是一款专为汽车应用设计的碳化硅 (SiC) 功率 MOSFET，采用先进的工艺技术，实现极低的单位面积导通电阻。该器件适用于高频应用，具有出色的开关性能和可靠性。

### 🌟 核心特性 (Features)
* 开关速度快，寄生电容小 (High Speed Switching with Low Capacitances)
* 阻断电压高，导通电阻低 (High Blocking Voltage with Low RDS(on))
* 100% 通过雪崩测试 (100% Avalanche Tested)
* 无卤元素，符合 RoHS (Halogen Free and RoHS Compliant)

### 🚗 典型应用 (Applications)
* EV 充电 (EV Charging)
* DC-AC 逆变器 (DC-AC Inverters)
* 高压 DC/DC 变换器 (High Voltage DC/DC Converters)
* 功率因数校正模块 (Power Factor Correction Modules)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 漏极-源极电压 ($V_{DSS}$) | 漏极电流 ($I_D$) @25°C | 典型导通电阻 ($R_{DS(on)}$) | 最高结温 ($T_{jmax}$) | 印丝标记 (Marking) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BSN160S120** | 1200 V | 26 A | 160 mΩ | 175 °C | BSN160S120 | TO-247 |

---

## ⚡ 最大额定参数 (Maximum Rated Values)

下表规定了器件工作或测试时绝不可超过的极限参数（如无特殊说明，$T_j = 25^\circ\text{C}$）：

| 参数名称 (Parameter) | 符号 (Symbol) | 额定值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| 漏极-源极电压 | $V_{DSS}$ | 1200 | V |
| 连续漏极电流 ($T_C = 25^\circ\text{C}$) | $I_D$ | 26 | A |
| 连续漏极电流 ($T_C = 100^\circ\text{C}$) | $I_D$ | 17 | A |
| 脉冲漏极电流 (脉宽受 $T_{jmax}$ 限制) | $I_{D(pulse)}$ | 44 | A |
| 栅极-源极电压 (最大值) | $V_{GSmax}$ | -10/+25 | V |
| 栅极-源极电压 (推荐工作) | $V_{GS}$ | -5/+20 | V |
| 总耗散功率 ($T_C = 25^\circ\text{C}$) | $P_D$ | 132 | W |
| 最高结温 | $T_{jmax}$ | 175 | °C |
| 工作结温 | $T_{jop}$ | -55 to +175 | °C |
| 储存温度 | $T_{stg}$ | -55 to +175 | °C |
| 焊接温度 (距管壳 1.6mm 处限时 10s) | $T_{st}$ | 260 | °C |
| 锁装力矩 | $M_d$ | 1 | Nm |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Value) | 单位 (Unit) |
| :--- | :---: | :---: | :---: |
| MOSFET 结-管壳热阻 | $R_{\theta JC}$ | 1.13 | °C/W |
| 结-环境热阻 | $R_{\theta JA}$ | 40 | °C/W |

---

## 🔌 电学特性 (Electrical Characteristics)

### 1. 静态特性 (Static Characteristic, $T_j = 25^\circ\text{C}$ 除非特别声明)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 (Min.) | 典型值 (Typ.) | 最大值 (Max.) | 单位 (Unit) |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 漏极-源极击穿电压 | $V_{BR(DSS)}$ | $V_{GS}=0\text{V}, I_D=100\mu\text{A}$ | 1200 | - | - | V |
| 漏极-源极导通电阻 | $R_{DS(on)}$ | V_GS=20V, I_D=13A, $T_j=25^\circ\text{C}$<br>V_GS=20V, I_D=13A, $T_j=175^\circ\text{C}$ | -<br>- | 160<br>238 | 240<br>- | mΩ<br>mΩ |
| 栅极-源极阈值电压 | $V_{GS(th)}$ | $V_{DS}=V_{GS}, I_{DS}=10\text{mA}$ | 2.0 | 3.2 | 4.0 | V |
| 零栅极电压漏极电流 | $I_{DSS}$ | $V_{DS}=1200\text{V}, V_{GS}=0\text{V}, T_j=25^\circ\text{C}$ | - | - | 100 | $\mu\text{A}$ |
| 栅极-源极漏电流 | $I_{GSS}$ | $V_{GS}=18\text{V}, V_{DS}=0\text{V}$ | - | - | 100 | nA |
| 栅极电阻 | $R_G$ | $f=1\text{MHz}, V_{AC}=25\text{mV}$ | - | 20 | - | $\Omega$ |

### 2. 动态特性 (Dynamic Characteristic)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :---: | :--- | :---: | :---: |
| 输入电容 | $C_{iss}$ | $V_{DS}=800\text{V}, V_{GS}=0\text{V}, f=1\text{MHz}$ | 1009 | pF |
| 输出电容 | $C_{oss}$ | $V_{DS}=800\text{V}, V_{GS}=0\text{V}, f=1\text{MHz}$ | 48 | pF |
| 反向传输电容 | $C_{rss}$ | $V_{DS}=800\text{V}, V_{GS}=0\text{V}, f=1\text{MHz}$ | 13 | pF |
| 门极总电量 | $Q_G$ | $V_{DD}=800\text{V}, I_D$按规格书, $V_{GS}=-5/20\text{V}$ | 48 | nC |
| 栅-源电荷 | $Q_{gs}$ | $V_{DD}=800\text{V}, I_D$按规格书, $V_{GS}=-5/20\text{V}$ | 13 | nC |
| 栅-漏电荷 | $Q_{gd}$ | $V_{DD}=800\text{V}, I_D$按规格书, $V_{GS}=-5/20\text{V}$ | 17 | nC |

---

## 🔄 开关特性 (Switching Characteristics)

### 1. $T_j = 25^\circ\text{C}$ 时开关特性（感性负载）
测试条件：$V_{{DS}}=800$V, $V_{{GS}}=-5/20$V, $I_D=13$A, $R_{{G(ext)}}=5\Omega$, $R_L=40\Omega$

| 参数分类 | 参数名称 (Parameter) | 符号 (Symbol) | 典型值 (Typ.) | 单位 (Unit) |
| :--- | :--- | :---: | :---: | :---: |
| **MOSFET 特性** | 开通延迟时间 (Turn-on delay time) | $t_{d(on)}$ | 18 | ns |
| | 上升时间 (Rise time) | $t_r$ | 26 | ns |
| | 关断延迟时间 (Turn-off delay time) | $t_{d(off)}$ | 34 | ns |
| | 下降时间 (Fall time) | $t_f$ | 16 | ns |
| | 开通损耗 (Turn-on energy) | $E_{on}$ | 0.9 | mJ |
| | 关断损耗 (Turn-off energy) | $E_{off}$ | 0.2 | mJ |
| **体二极管** | 源极-漏极正向电压 (Source-drain forward voltage) | $V_{SD}$ | 3.4 | V |
| | 反向恢复时间 (Reverse recovery time) | $t_{rr}$ | 24 | ns |
| | 恢复电荷 (Recovered charge) | $Q_{rr}$ | 51 | nC |
| | 峰值反向恢复电流 (Peak reverse recovery current) | $I_{rrm}$ | 6 | A |

---

## 📐 封装外形尺寸 (TO-247 Outline Dimensions)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

*详细封装尺寸请参阅规格书中的 Package Outlines 章节*

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Packing) | 每管/盘数量 (pcs/tube) | 每盒管数 (tube/inner box) | 每箱盒数 (inner box/carton) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: | :---: | :---: |
| 管装 (Tube) | 30 | 12 | 6 | 2160 |

---

🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
