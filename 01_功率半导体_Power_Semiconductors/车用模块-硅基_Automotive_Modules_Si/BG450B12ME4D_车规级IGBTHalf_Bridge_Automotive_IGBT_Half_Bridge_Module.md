# 比亚迪半导体 (BYD) 车规级 Half-Bridge IGBT 模块 - BG450B12ME4D

[![Standard](https://img.shields.io/badge/Standard-AEC--Q101-red.svg)](https://www.aecouncil.com/)
[![Package](https://img.shields.io/badge/Package-V--DUAL1-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BG450B12ME4D** 是一款采用先进硅基 Field Stop 技术构建的 半桥 车规级功率模块，内部集成了 IGBT 与续流二极管 (FWD) 的最优匹配。产品严格符合 **AEC-Q101** 汽车级可靠性标准，专为新能源汽车电机驱动系统 (EV Traction)、车载充电机 (OBC)、DCDC 变换器及 PTC 加热等高可靠性场景设计。

### 🌟 核心特性 (Features)
* **车规认证**：严格符合 AEC-Q101 车规级标准要求
* **大功率半桥拓扑**：工业标准V-DUAL1外壳设计，内部Half-Bridge拓扑，优化电气连接
* **强韧动态特性**：具备高短路耐受能力（t<sub>sc</sub> ≥ 10 μs），RBSOA 达到额定电流 2 倍
* **低损耗设计**：优化导通损耗与开关损耗平衡，饱和电压 V<sub>CE(sat)</sub> 具有正温度系数，利于并联拓展
* **电气绝缘**：铜底板与陶瓷绝缘设计，绝缘等级 3.0 kV AC 1分钟
* **集成NTC温度传感器**：内置NTC热敏电阻，实时温度监控
* **符合RoHS标准**：环保无铅设计

### 🚗 典型应用 (Applications)
* 新能源汽车主驱电机控制器 (EV/HEV Traction Motor Drive)
* 车载充电机 (OBC - On-Board Charger)
* DC/DC 变换器及 PTC 加热器
* 电动压缩机驱动 (Electric Compressor)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 (V<sub>CES</sub>) | 额定公称电流 (I<sub>C(nom)</sub>) | 典型饱和电压 (V<sub>CE(sat)</sub>) | 最高工作结温 (T<sub>jmax</sub>) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BG450B12ME4D** | 1200 V | 450 A | 2.16 V | 175 °C | 半桥 (Half-Bridge) | V-DUAL1 |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>j</sub> = 25 °C，除非另外注明）

### 1. IGBT 逆变部分 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 集电极-发射极电压 | V<sub>CES</sub> | V<sub>GE</sub> = 0 V | 1200 | V |
| 连续直流集电极电流 | I<sub>C</sub> | T<sub>C</sub> = 80 °C | 450 | A |
| 集电极重复峰值电流 | I<sub>CRM</sub> | 脉宽受限，符合 T<sub>jmax</sub> | 900 | A |
| 总耗散功率 | P<sub>tot</sub> | T<sub>C</sub> = 25 °C，每 IGBT 晶圆 | 3950 | W |
| 栅极-发射极峰值电压 | V<sub>GES</sub> | - | ±20 | V |
| 短路耐受时间 | t<sub>sc</sub> | V<sub>GE</sub> = 15 V, T<sub>j</sub> ≤ 150 °C | 10 | μs |

### 2. 二极管部分 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 二极管连续正向直流电流 | I<sub>F</sub> | - | 450 | A |
| 二极管重复峰值正向电流 | I<sub>FRM</sub> | 脉宽受限，符合 T<sub>jmax</sub> | 900 | A |

### 3. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 绝缘测试电压 | V<sub>ISO</sub> | f = 50/60 Hz，正弦波 AC 1 分钟，引脚到散热片底板 | 3.0 | kV |
| 最大工作结温 | T<sub>jmax</sub> | 晶圆动态极限最大温度 | 175 | °C |
| 工作结温范围 | T<sub>jop</sub> | 连续正常工作温区 | -40 ~ 150 | °C |
| 存储温度范围 | T<sub>stg</sub> | - | -40 ~ 125 | °C |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件/说明 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| IGBT 结-管壳热阻 | R<sub>th(j-c)</sub> | 每个独立 IGBT 的导热热阻 | - | 0.038 | - | °C/W |
| 二极管结-管壳热阻 | R<sub>th(j-c)</sub> | 每个独立二极管的导热热阻 | - | 0.117 | - | °C/W |
| 管壳-散热片热阻 | R<sub>th(c-s)</sub> | 导热硅脂接触热阻 | - | 0.008 | - | °C/W |
| 端子螺丝扭矩 | M | 功率端子/基板安装螺钉 | 3.0 | 5.0 | 6.0 | N·m |
| 重量 | W | 模块整体重量 | - | 338 | - | g |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. IGBT 静态特性 (IGBT-Inverter, T<sub>j</sub> = 25 °C 除非特别声明)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极饱和压降 | V<sub>CE(sat)</sub> | V<sub>GE</sub> = 15 V, I<sub>C</sub> = 450 A, T<sub>j</sub> = 25 °C<br>V<sub>GE</sub> = 15 V, T<sub>j</sub> = 125 °C<br>V<sub>GE</sub> = 15 V, T<sub>j</sub> = 150 °C | -<br>-<br>- | 2.16<br>2.30<br>2.33 | —<br>-<br>- | V |
| 栅极-发射极阈值电压 | V<sub>GE(th)</sub> | I<sub>C</sub> = 16 mA, V<sub>CE</sub> = V<sub>GE</sub>, T<sub>j</sub> = 25 °C | 5.0 | 6.0 | 7.0 | V |
| 门极漏电流 | I<sub>GES</sub> | V<sub>CE</sub> = 0 V, V<sub>GE</sub> = ±20 V | - | - | 400 | nA |
| 断态集电极漏电流 | I<sub>CES</sub> | V<sub>CE</sub> = V<sub>CES</sub>, V<sub>GE</sub> = 0 V | - | - | 1 | mA |
| 门极充电电量 | Q<sub>g</sub> | V<sub>GE</sub> = ±15 V | - | 1 | - | μC |
| 内部门极电阻 | R<sub>Gint</sub> | T<sub>j</sub> = 25 °C | - | 1.3 | - | Ω |
| 输入电容 | C<sub>ies</sub> | f = 1 MHz, V<sub>CE</sub> = 25 V, V<sub>GE</sub> = 0 V | - | 15.9 | - | nF |
| 反向传输电容 | C<sub>res</sub> | f = 1 MHz, V<sub>CE</sub> = 25 V, V<sub>GE</sub> = 0 V | - | 0.7 | - | nF |

### 2. IGBT 开关特性 (IGBT-Inverter, 感性负载)

测试条件：V<sub>CC</sub> = 600 V, I<sub>C</sub> = 450 A, V<sub>GE</sub> = ±15 V, R<sub>Gon</sub> = 1.0 Ω, R<sub>Goff</sub> = 6.7 Ω

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 125 °C<br>T<sub>j</sub> = 150 °C | -<br>-<br>- | 120<br>—<br>— | -<br>-<br>- | ns |
| 上升时间 | t<sub>r</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 125 °C<br>T<sub>j</sub> = 150 °C | -<br>-<br>- | 70<br>—<br>— | -<br>-<br>- | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 125 °C<br>T<sub>j</sub> = 150 °C | -<br>-<br>- | 310<br>—<br>— | -<br>-<br>- | ns |
| 下降时间 | t<sub>f</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 125 °C<br>T<sub>j</sub> = 150 °C | -<br>-<br>- | 150<br>—<br>— | -<br>-<br>- | ns |
| 开通损耗 | E<sub>on</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 125 °C<br>T<sub>j</sub> = 150 °C | -<br>-<br>- | 30<br>40<br>45 | -<br>-<br>- | mJ |
| 关断损耗 | E<sub>off</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 125 °C<br>T<sub>j</sub> = 150 °C | -<br>-<br>- | 33<br>42<br>50 | -<br>-<br>- | mJ |
| 短路电流 | I<sub>SC</sub> | V<sub>GE</sub> ≤ 15 V, t<sub>sp</sub> ≤ 10 μs | - | 2800 | - | A |

### 3. 续流二极管特性 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 正向导通压降 | V<sub>F</sub> | I<sub>F</sub> = 450 A, V<sub>GE</sub> = 0 V, T<sub>j</sub> = 25 °C<br>I<sub>F</sub> = 450 A, T<sub>j</sub> = 150 °C | -<br>- | 2.07<br>2.2 | —<br>- | V |
| 反向恢复峰值电流 | I<sub>RM</sub> | 测试条件同开关特性 | - | 270 | - | A |
| 反向恢复电荷 | Q<sub>rr</sub> | 测试条件同开关特性 | - | 70 | - | μC |
| 反向恢复损耗 | E<sub>rec</sub> | 测试条件同开关特性 | - | 20 | - | mJ |

### 4. NTC 热敏电阻特性 (NTC-Thermistor)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 额定电阻值 | R<sub>25</sub> | Tc = 25 °C | - | 5.0 | - | kΩ |
| R<sub>100</sub> 偏差 | ΔR/R | Tc = 100 °C, R<sub>100</sub> = 493 Ω | -5 | - | 5 | % |
| 耗散功率 | P<sub>25</sub> | Tc = 25 °C | - | - | 20 | mW |
| B值 (25/50) | B<sub>25/50</sub> | - | - | 3375 | - | K |
| B值 (25/80) | B<sub>25/80</sub> | - | - | 3411 | - | K |
| B值 (25/100) | B<sub>25/100</sub> | - | - | 3433 | - | K |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

*(此处根据具体封装绘制尺寸参数表)*

---

🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。

> *注：BG450B12ME4D 采用先进硅基 Field Stop（场终止）技术，具有低导通压降和优化的开关特性。*
>
> *该产品严格符合 **AEC-Q101** 汽车级可靠性标准，专为新能源汽车电机驱动系统（EV Traction）、车载充电机（OBC）、DCDC 变换器及 PTC 加热等高可靠性场景设计。*