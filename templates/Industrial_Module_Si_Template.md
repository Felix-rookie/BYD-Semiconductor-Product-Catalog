# 比亚迪半导体 (BYD) 硅基工业模块 (Industrial Module - Si) 数据转换模板

> 💡 **贡献者填写指南**：
> 1. 本模板专门用于处理【功率半导体】板块下的 **工业模块-Si (Industrial Modules - Silicon)**，通常适用于大功率标准变频器、逆变器及电焊机等模块。
> 2. 工业模块非常注重【测试条件】的严谨性，填报数据时请务必准确抄录规格书中的公称测试电流（如 $I_{C(nom)}$）以及结温状态下的损耗值。
> 3. 括号内的中文/英文提示语（如 `[型号]`）在实际转换时，请替换为规格书（Datasheet）中的真实数据。

---

# 比亚迪半导体 (BYD) 硅基工业半桥/三相模块 - [产品型号]

[![Package](https://img.shields.io/badge/Package-[封装形式：如标准工业封装/62mm]-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**[产品型号]** 是一款采用先进硅基场终止 (Field-Stop) 技术构建的工业级大功率 [逆变拓扑：如双管半桥/三相全桥] 模块。该模块具有极低的导通压降、优异的动态开关特性以及极高的强韧度，专为 [应用领域：如高可靠性大功率工业变频器、光伏逆变器及电焊机] 方案设计。

### 🌟 核心特性 (Features)
* **大功率拓扑**：工业标准外壳设计，内部优化配置 [如：IGBT半桥与快恢复二极管 FWD 最佳匹配]
* **强韧动态特性**：具备高短路耐受能力（$t_{sc} \ge 10\,\mu\text{s}$），反偏安全工作区 (RBSOA) 达到 2 倍额定电流
* **电气绝缘佳**：基板采用铜底板与陶瓷绝缘设计，绝缘等级高达 [如：2500V / 3000V] AC 1分钟
* **易于并联**：饱和导通电压 ($V_{CE(sat)}$) 具有优异的正温度系数

### 🚗 典型应用 (Applications)
* 大功率通用工业变频器 (High Power General Inverter)
* 伺服驱动器与大功率交流电机传动 (Servo Drives & AC Motor Control)
* 光伏与风力发电逆变系统 (Solar/Wind Inverters)
* 工业电焊机与大功率高频开关电源 (Industrial Welding & UPS)

---

## 📊 关键参数快查 (Quick Reference Table)

| 型号 (Type) | 集电极-发射极电压 ($V_{CES}$) | 额定公称电流 ($I_{C(nom)}$) | 典型饱和电压 ($V_{CE(sat)}$) | 最高工作结温 ($T_{jmax}$) | 内部拓扑 (Topology) | 封装形式 (Package) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **[产品型号]** | [电压] V | [电流] A | [饱和电压] V | [结温] °C | [半桥/三相全桥等] | [封装名称] |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（测试条件：$T_j = 25^\circ\text{C}$，除非另外注明）

### 1. IGBT 逆变部分 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 集电极-发射极电压 | $V_{CES}$ | $V_{GE} = 0\text{V}$ | [数值] | V |
| 连续直流集电极电流 | $I_C$ | $T_C = [数值]^\circ\text{C}$<br>$T_C = 25^\circ\text{C}$ | [数值]<br>[数值] | A |
| 额定集电极公称电流 | $I_{C(nom)}$ | 工业级标称连续工作电流 | [数值] | A |
| 集电极重复峰值电流 | $I_{CRM}$ | 脉宽受限，符合 $T_{jmax}$ | [数值] | A |
| 总耗散功率 | $P_{tot}$ | $T_C = 25^\circ\text{C}$，每个单独 IGBT 晶圆 | [数值] | W |
| 栅极-发射极峰值电压 | $V_{GES}$ | - | $\pm 20$ | V |

### 2. 续流二极管部分 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 二极管连续正向直流电流 | $I_F$ | - | [数值] | A |
| 二极管重复峰值正向电流 | $I_{FRM}$ | 脉宽受限，符合 $T_{jmax}$ | [数值] | A |

### 3. 模块整体系统 (Module System)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 额定值 | 单位 |
| :--- | :---: | :--- | :---: | :---: |
| 绝缘测试电压 | $V_{ISO}$ | $f=50/60\text{Hz}$，正弦波交流电压1分钟，引脚到散热片底板 | [数值] | V |
| 最大工作结温 | $T_{jmax}$ | 晶圆动态极限最大温度 | [数值] | °C |
| 工作结温范围 | $T_{jop}$ | 连续正常工作温区 | [范围] | °C |
| 存储温度范围 | $T_{stg}$ | - | [范围] | °C |

---

## 🌡️ 热阻与机械特性 (Thermal & Mechanical Characteristics)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件/说明 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| IGBT 结-管壳热阻 | $R_{th(j-c)}$ | 每个独立 IGBT 的导热热阻 | - | [数值] | [数值] | °C/W |
| 二极管 结-管壳热阻 | $R_{th(j-c)}$ | 每个独立二极管的导热热阻 | - | [数值] | [数值] | °C/W |
| 管壳-散热片热阻 | $R_{th(c-s)}$ | 每个模块应用导热硅脂后的接触热阻 | - | [数值] | - | °C/W |
| 端子螺丝紧固扭矩 | $M$ | 功率端子连接螺钉 M[号] 安装力矩 | [数值] | [数值] | [数值] | $\text{N}\cdot\text{m}$ |
| 基板安装紧固扭矩 | $M$ | 模块到底板固定螺钉 M[号] 安装力矩 | [数值] | [数值] | [数值] | $\text{N}\cdot\text{m}$ |
| 重量 (Weight) | $W$ | 模块整体产品克重 | - | [数值] | - | g |

---

## 🔌 电气特性 (Electrical Characteristics)

### 1. IGBT 静态与动态特性 (IGBT-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 集电极-发射极饱和压降 | $V_{CE(sat)}$ | $V_{GE}=15\text{V}, I_C=[数值]\text{A}, T_j=25^\circ\text{C}$<br>$V_{GE}=15\text{V}, I_C=[数值]\text{A}, T_j=125^\circ\text{C}$<br>$V_{GE}=15\text{V}, I_C=[数值]\text{A}, T_j=150^\circ\text{C}$ | - | [数值]<br>[数值]<br>[数值] | [数值]<br>-<br>- | V |
| 栅极-发射极阈值电压 | $V_{GE(th)}$ | $I_C=[数值]\text{mA}, V_{CE}=V_{GE}, T_j=25^\circ\text{C}$ | [数值] | [数值] | [数值] | V |
| 门极漏电流 | $I_{GES}$ | $V_{CE}=0\text{V}, V_{GE}=\pm20\text{V}, T_j=25^\circ\text{C}$ | - | - | [数值] | nA |
| 断态集电极漏电流 | $I_{CES}$ | $V_{CE}=V_{CES}, V_{GE}=0\text{V}, T_j=25^\circ\text{C}$ | - | - | [数值] | mA |
| 门极充电电量 | $Q_g$ | $V_{GE}=-15\text{V} \ldots +15\text{V}, V_{CC}=[数值]\text{V}$ | - | [数值] | - | $\mu\text{C}$ |
| 内部门极电阻 | $R_{Gint}$ | $T_j=25^\circ\text{C}$ | - | [数值] | - | $\Omega$ |
| 输入电容 | $C_{ies}$ | $f=1\text{MHz}, T_j=25^\circ\text{C}, V_{CE}=25\text{V}, V_{GE}=0\text{V}$ | - | [数值] | - | nF |
| 反向传输电容 | $C_{res}$ | $f=1\text{MHz}, T_j=25^\circ\text{C}, V_{CE}=25\text{V}, V_{GE}=0\text{V}$ | - | [数值] | - | nF |
| 短路耐受电流数据 | $I_{SC}$ | $V_{GE} \le 15\text{V}, V_{CC}=[数值]\text{V}, t_{sp} \le 10\,\mu\text{s}, T_{jop}=150^\circ\text{C}$ | - | [数值] | - | A |

### 2. IGBT 开关损耗特性 (IGBT-Inverter, 感性负载测试)
测试条件：$V_{CC}=[数值]\text{V}, I_C=[数值]\text{A}, V_{GE}=\pm15\text{V}, R_{Gon}=[数值]\,\Omega, R_{Goff}=[数值]\,\Omega$

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 开通延迟时间 | $t_{d(on)}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 125^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$ | - | [数值]<br>[数值]<br>[数值] | - | ns |
| 上升时间 | $t_r$ | $T_j = 25^\circ\text{C}$<br>$T_j = 125^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$ | - | [数值]<br>[数值]<br>[数值] | - | ns |
| 关断延迟时间 | $t_{d(off)}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 125^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$ | - | [数值]<br>[数值]<br>[数值] | - | ns |
| 下降时间 | $t_f$ | $T_j = 25^\circ\text{C}$<br>$T_j = 125^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$ | - | [数值]<br>[数值]<br>[数值] | - | ns |
| 开通损耗电能 (每脉冲) | $E_{on}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 125^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$ | - | [数值]<br>[数值]<br>[数值] | - | mJ |
| 关断损耗电能 (每脉冲) | $E_{off}$ | $T_j = 25^\circ\text{C}$<br>$T_j = 125^\circ\text{C}$<br>$T_j = 150^\circ\text{C}$ | - | [数值]<br>[数值]<br>[数值] | - | mJ |

### 3. 续流二极管特性 (Diode-Inverter)

| 参数名称 (Parameter) | 符号 (Symbol) | 测试条件 (Conditions) | 最小值 | 典型值 | 最大值 | 单位 |
| :--- | :---: | :--- | :---: | :---: | :---: | :---: |
| 正向导通压降 | $V_F$ | $I_F=[数值]\text{A}, V_{GE}=0\text{V}, T_j=25^\circ\text{C}$<br>$I_F=[数值]\text{A}, V_{GE}=0\text{V}, T_j=125^\circ\text{C}$ | - | [数值]<br>[数值] | [数值]<br>- | V |
| 反向恢复峰值电流 | $I_{RM}$ | $I_F=[数值]\text{A}, -di_F/dt=[数值]\text{A}/\mu\text{s}, V_{CC}=[数值]\text{V}, T_j=125^\circ\text{C}$ | - | [数值] | - | A |
| 反向恢复电荷 | $Q_{rr}$ | $I_F=[数值]\text{A}, -di_F/dt=[数值]\text{A}/\mu\text{s}, V_{CC}=[数值]\text{V}, T_j=125^\circ\text{C}$ | - | [数值] | - | $\mu\text{C}$ |
| 反向恢复损耗能量 | $E_{rec}$ | $I_F=[数值]\text{A}, -di_F/dt=[数值]\text{A}/\mu\text{s}, V_{CC}=[数值]\text{V}, T_j=125^\circ\text{C}$ | - | [数值] | - | mJ |

---

## 📐 封装外形尺寸 (Package Outline Drawings)

所有公制尺寸单位均默认为：**毫米 (Millimeter)**

*(由于工业模块封装各异，如62mm封装、EconoPACK封装等，具体转换型号时在此处配置标准尺寸参数表)*

---
🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
