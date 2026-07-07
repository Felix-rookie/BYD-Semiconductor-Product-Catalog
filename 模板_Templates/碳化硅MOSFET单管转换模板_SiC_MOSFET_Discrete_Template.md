# 比亚迪半导体 (BYD) 碳化硅 MOSFET 单管 (SiC MOSFET Discrete) 数据转换模板

> 💡 **贡献者填写指南**：
> 1. 本模板专门用于处理【功率半导体】板块下的 **碳化硅 MOSFET 单管 (SiC MOSFET Discretes)**，适用于汽车及工业级 SiC MOSFET。
> 2. SiC MOSFET 不同于 IGBT：关键参数为 **导通电阻 R<sub>DS(on)</sub>** 而非饱和压降 V<sub>CE(sat)</sub>，体二极管续流能力需重点标注。
> 3. 括号内的提示语（如 `[型号]`）在实际转换时请替换为真实数据。
> 4. 禁用 LaTeX 公式符号，一律使用 HTML 下标格式（如 `R<sub>DS(on)</sub>`, `V<sub>GS(th)</sub>`）。

---

# 比亚迪半导体 (BYD) [产品级别：如车规级/工业级] 碳化硅 (SiC) MOSFET - [产品型号]

[![Standard](https://img.shields.io/badge/Standard-[标准：如AEC--Q101/工业级]-[颜色].svg)]()
[![Technology](https://img.shields.io/badge/Technology-SiC-green.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**[产品型号]** 是一款基于第三代宽禁带 **碳化硅 (SiC) MOSFET** 技术构建的高性能功率开关器件。采用 [如：平面栅/沟槽栅 SiC MOSFET] 工艺，集成了 [如：低阻抗体二极管]，具有极低的导通电阻、超低的开关损耗及卓越的高温工作能力。本产品 [认证标准：如严格符合 AEC-Q101 车规级标准]，专为 [应用领域：如高效率电动汽车驱动系统与高频工业电源] 设计。

### 🌟 核心特性 (Features)
* **先进 SiC 技术**：[电压等级] 碳化硅 MOSFET，极低 R<sub>DS(on)</sub>
* **超低损耗**：无 IGBT 尾电流，开关损耗极低，支持超高频率工作
* **高温工作**：最高结温 T<sub>jmax</sub> = [温度] °C，高温下导通电阻变化小
* **强韧体二极管**：内置低 Q<sub>rr</sub> 体二极管，可简化电路设计
* **易于并联**：R<sub>DS(on)</sub> 具有正温度系数

### 🚗 典型应用 (Applications)
* 电动汽车主驱逆变器 (EV/HEV Traction Inverter)
* 车载充电机 (OBC) 与 DC/DC 变换器
* 高效开关电源与 PFC 电路
* 光伏逆变器与储能系统

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 漏-源极电压 (V<sub>DSS</sub>) | 漏极电流 (I<sub>D</sub>) | 典型导通电阻 (R<sub>DS(on)</sub>) | 最高结温 (T<sub>jmax</sub>) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **[产品型号]** | [电压] V | [电流] A | [电阻] mΩ | [温度] °C | [封装名称] |

---

## ⚡ 最大额定参数 (Maximum Rated Values)

（如无特殊说明，T<sub>j</sub> = 25 °C）

| 参数名称 (Parameter) | 符号 (Symbol) | 额定值 | 单位 |
| :--- | :---: | :---: | :---: |
| 漏-源极电压 | V<sub>DSS</sub> | [数值] | V |
| 连续漏极电流 (T<sub>C</sub> = 25 °C) | I<sub>D</sub> | [数值] | A |
| 连续漏极电流 (T<sub>C</sub> = 100 °C) | I<sub>D</sub> | [数值] | A |
| 脉冲漏极电流 | I<sub>DM</sub> | [数值] | A |
| 栅-源极电压 | V<sub>GS</sub> | [范围] | V |
| 总耗散功率 (T<sub>C</sub> = 25 °C) | P<sub>tot</sub> | [数值] | W |
| 最高结温 | T<sub>jmax</sub> | [数值] | °C |
| 工作结温 | T<sub>jop</sub> | [范围] | °C |
| 储存温度 | T<sub>stg</sub> | [范围] | °C |

---

## 🌡️ 热阻特性 (Thermal Resistance)

| 参数名称 (Parameter) | 符号 (Symbol) | 最大值 | 单位 |
| :--- | :---: | :---: | :---: |
| 结-管壳热阻 | R<sub>th(j-c)</sub> | [数值] | °C/W |
| 结-环境热阻 | R<sub>th(j-a)</sub> | [数值] | °C/W |

---

## 🔌 电学特性 (Electrical Characteristics)

### 1. 静态特性 (Static Characteristic, T<sub>j</sub> = 25 °C 除非特别声明)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 漏-源极击穿电压 | V<sub>(BR)DSS</sub> | V<sub>GS</sub> = 0 V, I<sub>D</sub> = [电流] mA | [数值] | - | - | V |
| 漏-源极导通电阻 | R<sub>DS(on)</sub> | V<sub>GS</sub> = [电压] V, I<sub>D</sub> = [电流] A, T<sub>j</sub> = 25 °C<br>V<sub>GS</sub> = [电压] V, I<sub>D</sub> = [电流] A, T<sub>j</sub> = 150 °C | - | [数值]<br>[数值] | [数值]<br>- | mΩ |
| 栅极阈值电压 | V<sub>GS(th)</sub> | V<sub>DS</sub> = V<sub>GS</sub>, I<sub>D</sub> = [电流] mA | [数值] | [数值] | [数值] | V |
| 栅极漏电流 | I<sub>GSS</sub> | V<sub>GS</sub> = ±[电压] V, V<sub>DS</sub> = 0 V | - | - | [数值] | nA |
| 漏极截止电流 | I<sub>DSS</sub> | V<sub>DS</sub> = [电压] V, V<sub>GS</sub> = 0 V | - | - | [数值] | μA |
| 体二极管正向电压 | V<sub>SD</sub> | V<sub>GS</sub> = 0 V, I<sub>F</sub> = [电流] A | - | [数值] | [数值] | V |

### 2. 动态特性 (Dynamic Characteristic)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 输入电容 | C<sub>iss</sub> | V<sub>DS</sub> = [电压] V, f = 1 MHz | [数值] | pF |
| 输出电容 | C<sub>oss</sub> | V<sub>DS</sub> = [电压] V, f = 1 MHz | [数值] | pF |
| 反向传输电容 | C<sub>rss</sub> | V<sub>DS</sub> = [电压] V, f = 1 MHz | [数值] | pF |
| 门极总电荷 | Q<sub>g</sub> | V<sub>GS</sub> = [范围] V | [数值] | nC |
| 门极-漏极电荷 | Q<sub>gd</sub> | - | [数值] | nC |
| 内部门极电阻 | R<sub>G(int)</sub> | f = 1 MHz | [数值] | Ω |

### 3. 开关特性 (Switching Characteristic, 感性负载)

测试条件：V<sub>DD</sub> = [电压] V, I<sub>D</sub> = [电流] A, V<sub>GS</sub> = [范围] V, R<sub>G</sub> = [数值] Ω

| 参数名称 (Parameter) | 符号 (Symbol) | T<sub>j</sub> = 25 °C | T<sub>j</sub> = 150 °C | 单位 |
| :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | t<sub>d(on)</sub> | [数值] | [数值] | ns |
| 上升时间 | t<sub>r</sub> | [数值] | [数值] | ns |
| 关断延迟时间 | t<sub>d(off)</sub> | [数值] | [数值] | ns |
| 下降时间 | t<sub>f</sub> | [数值] | [数值] | ns |
| 开通损耗 | E<sub>on</sub> | [数值] | [数值] | mJ |
| 关断损耗 | E<sub>off</sub> | [数值] | [数值] | mJ |

### 4. 体二极管特性 (Body Diode Characteristic)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 典型值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 反向恢复时间 | t<sub>rr</sub> | I<sub>F</sub> = [电流] A, T<sub>j</sub> = 25 °C | [数值] | ns |
| 反向恢复电荷 | Q<sub>rr</sub> | I<sub>F</sub> = [电流] A, T<sub>j</sub> = 25 °C | [数值] | nC |
| 反向恢复峰值电流 | I<sub>RM</sub> | - | [数值] | A |

---

## 📐 封装外形尺寸 (Package Outline Dimensions)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

*(此处根据具体封装绘制尺寸参数表)*

---

## 📦 包装物流信息 (Packing Information)

| 包装形式 (Packing) | 每管/盘数量 (pcs) | 总装箱量 (pcs/carton) |
| :---: | :---: | :---: |
| [如：管装 Tube / 编带 Reel] | [数值] | [数值] |

---

🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
