# 比亚迪半导体 (BYD) 碳化硅 (SiC) 车规级功率模块 - BM950F12B34U2

[![Technology](https://img.shields.io/badge/Technology-SiC_MOSFET-green.svg)]()
[![Grade](https://img.shields.io/badge/Grade-Automotive__Grade-orange.svg)]()
[![Package](https://img.shields.io/badge/Package-标准模块封装 (PinFin Base Plate)-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BM950F12B34U2** 是一款基于第三代半导体材料——碳化硅 (SiC) 的功率模块，采用先进的 SiC MOSFET 芯片，具有低损耗和高短路能力。额定漏极电流 550A，阻断电压 1200V。采用银烧结工艺、直接冷却铜 PinFin 底板和高性能氮化硅陶瓷绝缘。

### 🌟 核心特性 (Features)
* 第三代半导体材料——碳化硅 (3rd Generation SiC)
* 阻断电压 1200V
* 低导通电阻 RDS(on) (Low RDS(on))
* 低开关损耗 (Low Switching Losses)
* 低 Qg 和 Crss (Low Qg and Crss)
* 低电感设计 ≤15nH (Low Inductive Design)
* 银烧结工艺 (Ag Sintering)
* 最高工作结温 175°C (Tvj op=175°C)
* 直接冷却铜 PinFin 底板 (Direct Cooled Cu PinFin Base Plate)
* 高性能氮化硅陶瓷绝缘 (High Performance Si₃N₄ Ceramic)
* 集成 NTC 温度传感器 (Integrated NTC Temperature Sensor)

### 🚗 典型应用 (Applications)
* 汽车级应用 (Automotive Application)
* 电动车/混动车 (Hybrid and Electric Vehicle)
* 电机驱动逆变器 (Inverters for Motor Drive)
* 最高支持 750V 电压平台 (Max applied voltage platform: 750)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 漏极-源极电压 ($V_{DSS}$) | 额定公称电流 ($I_{D(nom)}$) | 典型导通电阻 ($R_{DS(on)}$) | 最高工作结温 ($T_{jmax}$) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BM950F12B34U2** | 1200 V | 950 A | 1.9 mΩ | 175 °C | 半桥模块 (Half-Bridge) | 标准模块封装 (PinFin Base Plate) |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：$T_j = 25^\circ\text{C}$，除非另外注明）

### 1. MOSFET 逆变部分 (MOSFET-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 漏极-源极电压 | $V_{DSS}$ | $V_{GS} = 0\text{V}$ | 1200 | V |
| 连续漏极直流电流 | $I_{D(nom)}$ | $T_F = 65^\circ\text{C}, T_{vjmax} = 175^\circ\text{C}$ | 950 | A |
| 脉冲漏极电流 | $I_{D(pulse)}$ | 脉宽受限，符合 $T_{jmax}$ | 1800 | A |
| 总耗散功率 | $P_{tot}$ | $T_F = 65^\circ\text{C}$ | 1180 | W |
| 栅极-源极峰值电压 (瞬态) | $V_{GS}$ | $t_p < 1\mu\text{s}$ | $\pm$见规格书 | V |
| 栅极-源极电压 (最大值) | $V_{GSmax}$ | - | -5.5/+20 | V |
| 栅极-源极电压 (推荐工作) | $V_{GSop}$ | - | -5/+18 | V |

### 2. 体二极管部分 (Body Diode)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 体二极管连续正向电流 | $I_{SD}$ | 等同于 $I_{D(nom)}$ | 950 | A |
| 体二极管脉冲正向电流 | $I_{SD(pulse)}$ | 脉宽受限，符合 $T_{jmax}$ | 1800 | A |

### 3. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 绝缘测试电压 | $V_{ISO}$ | $f=50/60\text{Hz}$，AC 1分钟，引脚到散热片底板 | — | kV |
| 最大工作结温 | $T_{jmax}$ | 晶圆动态极限最大温度 | 175 | °C |
| 工作结温范围 | $T_{jop}$ | 连续正常工作温区 | -40~175 | °C |
| 存储温度范围 | $T_{stg}$ | - | -40~125 | °C |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件/说明 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| MOSFET 结-冷却液热阻 | $R_{th(j-f)}$ | 每个 MOSFET，$\Delta V/\Delta t$ 按规格书 | - | — | - | °C/W |
| 杂散电感 | $L_{sCE}$ | 模块内部 | - | 15 | - | nH |
| 模块引线电阻 | $R_{CC'+EE'}$ | 端子到芯片，每开关 | - | — | - | mΩ |
| 端子螺丝紧固扭矩 | $M$ | 功率端子 M5 安装力矩 | — | — | — | $\text{N}\cdot\text{m}$ |
| 基板安装紧固扭矩 | $M$ | 模块到底板固定螺钉 M4 | — | — | — | $\text{N}\cdot\text{m}$ |
| 重量 | $W$ | 模块整体产品克重 | - | — | - | g |
| 外形尺寸 | $L \times W \times H$ | 典型值 | - | — | - | mm |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. MOSFET 静态与动态特性 (MOSFET-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 漏极-源极导通电阻 | $R_{DS(on)}$ | $V_{GS}=18\text{V}, I_D=I_D=420A, V_GS=18V, T_j=25^\circ\text{C}$<br>$V_{GS}=18\text{V}, I_D=I_D=420A, V_GS=18V, T_j=175^\circ\text{C}$ | -<br>- | 1.9<br>4.6 (175°C) | 3.2<br>- | mΩ<br>mΩ |
| 漏极-源极击穿电压 | $V_{BR(DSS)}$ | $V_{GS}=0\text{V}, I_D=1\text{mA}$ | 1200 | - | - | V |
| 栅极-源极阈值电压 | $V_{GS(th)}$ | $I_D=$按规格书, $V_{DS}=V_{GS}, T_j=25^\circ\text{C}$ | 2.1 | 3.2 | 5.8 | V |
| 栅极漏电流 | $I_{GSS}$ | $V_{CE}=0\text{V}, V_{GS}=20\text{V}, T_j=25^\circ\text{C}$ | - | - | 100 nA | nA |
| 断态漏极漏电流 | $I_{DSS}$ | $V_{DS}=V_{DSS}, V_{GS}=0\text{V}, T_j=25^\circ\text{C}$ | - | - | 150 μA | $\mu\text{A}$ |
| 门极充电电量-源极 | $Q_{gs}$ | $V_{DS}=850\text{V}, V_{GS}=-5~18\text{V}$ | - | 518 | - | nC |
| 门极充电电量-漏极 | $Q_{gd}$ | $V_{DS}=850\text{V}, V_{GS}=-5~18\text{V}$ | - | 280 | - | nC |
| 门极总电量 | $Q_g$ | $V_{DS}=850\text{V}, V_{GS}=-5~18\text{V}$ | - | 1330 | - | nC |
| 内部栅极电阻 | $R_{Gint}$ | $T_j=25^\circ\text{C}, f=1\text{MHz}$ | - | 1.6 | - | $\Omega$ |
| 输入电容 | $C_{iss}$ | $f=1\text{MHz}, T_j=25^\circ\text{C}, V_{DS}=850\text{V}$ | - | 28 (nF) | - | nF |
| 输出电容 | $C_{oss}$ | $f=1\text{MHz}, T_j=25^\circ\text{C}, V_{DS}=850\text{V}$ | - | 1.61 (nF) | - | nF |
| 反向传输电容 | $C_{rss}$ | $f=1\text{MHz}, T_j=25^\circ\text{C}, V_{DS}=850\text{V}$ | - | 154 (pF) | - | pF |

### 2. MOSFET 开关损耗特性 (MOSFET-Inverter, 感性负载测试)
测试条件：$V_{{DS}}=650$V, $I_{{DS}}=600$A, $V_{{G}}=-5/18$V, $R_{{Gon}}=12.4\Omega$, $R_{{Goff}}=8.25\Omega$, $L_S=30$nH

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值(Typ.) | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | $t_{d(on)}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$<br>$T_j = 175^\circ\text{C}$ | -<br>-<br>- | 159<br>122<br>113 | -<br>-<br>- | ns<br>ns<br>ns |
| 上升时间 | $t_r$ | $T_j = 25^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$<br>$T_j = 175^\circ\text{C}$ | -<br>-<br>- | 134<br>113<br>111 | -<br>-<br>- | ns<br>ns<br>ns |
| 关断延迟时间 | $t_{d(off)}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$<br>$T_j = 175^\circ\text{C}$ | -<br>-<br>- | 540<br>625<br>642 | -<br>-<br>- | ns<br>ns<br>ns |
| 下降时间 | $t_f$ | $T_j = 25^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$<br>$T_j = 175^\circ\text{C}$ | -<br>-<br>- | 81<br>89<br>92 | -<br>-<br>- | ns<br>ns<br>ns |
| 开通损耗电能 (每脉冲) | $E_{on}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$<br>$T_j = 175^\circ\text{C}$ | -<br>-<br>- | 45<br>38<br>37 | -<br>-<br>- | mJ<br>mJ<br>mJ |
| 关断损耗电能 (每脉冲) | $E_{off}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$<br>$T_j = 175^\circ\text{C}$ | -<br>-<br>- | 51<br>51<br>51 | -<br>-<br>- | mJ<br>mJ<br>mJ |

### 3. 体二极管特性 (Body Diode)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 源极-漏极正向导通压降 | $V_{SD}$ | 按规格书, $T_j=25^\circ\text{C}$<br>按规格书, $T_j=175^\circ\text{C}$ | -<br>- | —<br>— | -<br>- | V<br>V |
| 反向恢复峰值电流 | $I_{rrm}$ | $I_F$按规格书, $V_{DS}$按规格书, $T_j=175^\circ\text{C}$ | - | — | - | A |
| 反向恢复电荷 | $Q_{rr}$ | $I_F$按规格书, $V_{DS}$按规格书, $T_j=175^\circ\text{C}$ | - | — | - | nC |
| 反向恢复时间 | $t_{rr}$ | $I_F$按规格书, $V_{DS}$按规格书, $T_j=175^\circ\text{C}$ | - | — | - | ns |
| 反向恢复损耗能量 | $E_{rr}$ | $I_F$按规格书, $T_j=175^\circ\text{C}$ | - | — | - | mJ |

### 4. NTC 热敏电阻特性 (NTC-Thermistor)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 额定电阻 | $R_{25}$ | $T_C=25^\circ\text{C}$ | - | 5.0 | - | kΩ |
| B值 (25/50) | $B_{25/50}$ | $R_2=R_{25}\exp[B_{25/50}(1/T_2-1/298.15K)]$ | - | 3375 | - | K |
| B值 (25/80) | $B_{25/80}$ | $R_2=R_{25}\exp[B_{25/80}(1/T_2-1/298.15K)]$ | - | 3411 | - | K |
| B值 (25/100) | $B_{25/100}$ | $R_2=R_{25}\exp[B_{25/100}(1/T_2-1/298.15K)]$ | - | 3433 | - | K |
| R100 偏差 | $\Delta R/R$ | $T_C=100^\circ\text{C}, R_{100}=493\Omega$ | -5 | - | 5 | % |
| 耗散功率 | $P_{25}$ | $T_C=25^\circ\text{C}$ | - | - | 20.0 | mW |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

外形尺寸：— mm

*详细封装尺寸请参阅规格书中的 Package Outlines 章节*

---

🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
