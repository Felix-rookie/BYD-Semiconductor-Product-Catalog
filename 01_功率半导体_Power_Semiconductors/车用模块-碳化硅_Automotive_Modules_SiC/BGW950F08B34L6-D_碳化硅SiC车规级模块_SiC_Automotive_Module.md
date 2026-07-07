# 比亚迪半导体 (BYD) 车规级碳化硅 (SiC) 半桥模块 - BGW950F08B34L6-D

[![Standard](https://img.shields.io/badge/Standard-AEC--Q101-red.svg)](https://www.aecouncil.com/)
[![Technology](https://img.shields.io/badge/Technology-SiC-green.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BGW950F08B34L6-D** 是一款基于第三代宽禁带 **碳化硅 (SiC) MOSFET** 技术构建的高性能车规级功率模块。采用先进的 SiC MOSFET 工艺，具有极低的导通电阻、超低的开关损耗及卓越的高温工作能力。产品严格符合 **AEC-Q101** 标准，专为纯电/混动车主驱逆变器 (EV/HEV Traction Inverter) 设计，可显著提升系统效率与功率密度。

### 🌟 核心特性 (Features)
* **车规认证**：严格符合 AEC-Q101 车规级标准
* **先进 SiC 技术**：采用第三代 SiC MOSFET 技术，极低导通电阻 R<sub>DS(on)</sub>
* **超低开关损耗**：无 IGBT 尾电流，开关损耗极低，支持高频化设计
* **高温工作**：最高结温 T<sub>jmax</sub> = 175 °C，优异的散热能力
* **强韧体二极管**：内置 SiC 体二极管，反向恢复特性优异（反向恢复电荷 Q<sub>rr</sub> 极低）

### 🚗 典型应用 (Applications)
* 纯电/混动车主驱逆变器 (EV/HEV Main Traction Inverter)
* 车载充电机 (OBC) 及 DC/DC 变换器
* 电动压缩机与电加热 (PTC) 驱动系统

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 漏-源极电压 (V<sub>DSS</sub>) | 漏极额定电流 (I<sub>D</sub>) | 典型导通电阻 (R<sub>DS(on)</sub>) | 最高工作结温 (T<sub>jmax</sub>) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **BGW950F08B34L6-D** | 750 V | 950 A | 1.20 mΩ | 175 °C | 全桥模块 (Full Bridge) | 标准模块封装 (PinFin Base Plate) |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：T<sub>j</sub> = 25 °C，除非另外注明）

### 1. SiC MOSFET 功率部分 (SiC MOSFET Power Part)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 漏-源极电压 | V<sub>DSS</sub> | V<sub>GS</sub> = 0 V | 750 | V |
| 连续漏极电流 | I<sub>D</sub> | T<sub>C</sub> = 65 °C | 950 | A |
| 脉冲漏极电流 | I<sub>DM</sub> | 脉宽受限，符合 T<sub>jmax</sub> | 1900 | A |
| 总耗散功率 | P<sub>tot</sub> | T<sub>C</sub> = 25 °C | 1149 | W |
| 栅-源极电压 | V<sub>GS</sub> | - | ±20 | V |

### 2. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 绝缘测试电压 | V<sub>ISO</sub> | 50/60 Hz，AC 1 分钟，引脚到散热片 | 3.8 | kV |
| 最大工作结温 | T<sub>jmax</sub> | SiC MOSFET 晶圆极限温度 | 175 | °C |
| 工作结温范围 | T<sub>jop</sub> | - | -40 ~ 175 | °C |
| 存储温度范围 | T<sub>stg</sub> | - | -40 ~ 125 | °C |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 结-管壳热阻（每 SiC MOSFET） | R<sub>th(j-c)</sub> | - | 0.0957 | °C/W |
| 管壳-散热片热阻 | R<sub>th(c-s)</sub> | 导热硅脂接触 | 参考规格书 | °C/W |
| 端子螺丝扭矩 | M | 功率端子安装螺钉 | 3 ~ 6 | N·m |
| 重量 | W | - | 710 | g |
| 外形尺寸 | L × W × H | - | 154.5×126.5×32 | mm |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. SiC MOSFET 静态特性 (T<sub>j</sub> = 25 °C 除非特别声明)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 漏-源极击穿电压 | V<sub>(BR)DSS</sub> | V<sub>GS</sub> = 0 V, I<sub>D</sub> = 1 mA | 750 | - | - | V |
| 漏-源极导通电阻 | R<sub>DS(on)</sub> | V<sub>GS</sub> = 15 V, I<sub>D</sub> = 450 A, T<sub>j</sub> = 25 °C<br>V<sub>GS</sub> = 15 V, T<sub>j</sub> = 150 °C | - | 1.20<br>1.30 | —<br>- | mΩ |
| 栅极阈值电压 | V<sub>GS(th)</sub> | V<sub>DS</sub> = V<sub>GS</sub>, I<sub>D</sub> = [电流] mA | 4.9 | 5.8 | 6.5 | V |
| 栅极漏电流 | I<sub>GSS</sub> | V<sub>GS</sub> = ±20 V | - | - | 400 | nA |
| 漏极截止电流 | I<sub>DSS</sub> | V<sub>DS</sub> = V<sub>DSS</sub>, V<sub>GS</sub> = 0 V | - | - | 1 (mA) | μA |
| 体二极管正向电压 | V<sub>SD</sub> | V<sub>GS</sub> = 0 V, I<sub>F</sub> = [电流] A | - | 1.40 | — | V |
| 门极总电荷 | Q<sub>g</sub> | V<sub>GS</sub> = [-5 ~ 18] V | - | 1.84 | - | μC |
| 内部门极电阻 | R<sub>Gint</sub> | - | - | 0.8 | - | Ω |
| 输入电容 | C<sub>iss</sub> | V<sub>DS</sub> = [电压] V, f = 1 MHz | - | 39.6 | - | nF |
| 输出电容 | C<sub>oss</sub> | V<sub>DS</sub> = [电压] V, f = 1 MHz | - | 1.45 | - | nF |
| 反向传输电容 | C<sub>rss</sub> | V<sub>DS</sub> = [电压] V, f = 1 MHz | - | 0.19 | - | nF |

### 2. SiC MOSFET 开关特性 (感性负载)

测试条件：V<sub>DD</sub> = 450 V, I<sub>D</sub> = 450 A, V<sub>GS</sub> = -8/+15, R<sub>G(on)</sub> = 2.5 Ω, R<sub>G(off)</sub> = 13.5 Ω

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 255<br>265 | ns |
| 上升时间 | t<sub>r</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 77<br>83 | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 1035<br>1127 | ns |
| 下降时间 | t<sub>f</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 56<br>83 | ns |
| 开通损耗 | E<sub>on</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 19.0<br>31.5 | mJ |
| 关断损耗 | E<sub>off</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 24.0<br>31.0 | mJ |

### 3. 体二极管续流特性 (Body Diode Reverse Recovery)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 反向恢复电荷 | Q<sub>rr</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 参考规格书 | μC |
| 反向恢复时间 | t<sub>rr</sub> | T<sub>j</sub> = 25 °C<br>T<sub>j</sub> = 150 °C | 参考规格书 | ns |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

*(此处根据具体封装绘制尺寸参数表)*

---

🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
