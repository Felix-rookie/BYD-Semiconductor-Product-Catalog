# 比亚迪半导体 (BYD) LED 灯珠数据转换模板

> 💡 **贡献者填写指南**：
> 1. 本模板专门用于处理【光电半导体】板块下的 **LED 灯珠 (Light Emitting Diodes)**。
> 2. LED 灯珠参数与功率模块差异较大，重点关注【光电参数】【色坐标/波长】【封装尺寸】等特有指标，提取 PDF 数据时切勿漏掉。
> 3. 括号内的中文/英文提示语（如 `[产品型号]`）在实际转换时，请替换为规格书（Datasheet）中的真实数据。
> 4. 当前覆盖产品系列：2016系列、2835系列、3528系列、0603系列、大灯系列（Headlight）。

---

# 比亚迪半导体 (BYD) LED - [产品型号]

[![Package](https://img.shields.io/badge/Package-[封装系列：如2016/2835/3528/0603]-blue.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**[产品型号]** 是一款基于 [芯片材料，如：InGaN/AlGaInP] 工艺的 [车规级/工业级] SMD LED。该器件采用 [封装尺寸，如：2.04×1.64×0.85mm] 封装，具有 [发光颜色] 发光特性，适用于 [典型应用场景]。

### 🌟 核心特性 (Features)
* **封装尺寸**：[长]×[宽]×[高] mm
* **发光颜色**：[颜色]
* **视角**：[角度]°
* **芯片材料**：[材料类型]
* **胶体类型**：[胶体颜色/类型]
* **符合RoHS标准**：环保无铅设计
* **MSL等级**：Level 2（JEDEC J-STD-020E）
* **ESD耐压**：≥ [ESD值] kV（HBM）

### 🚗 典型应用 (Applications)
* [应用场景1，如：汽车照明/日行灯]
* [应用场景2，如：转向灯/制动灯]
* [应用场景3，如：氛围灯/背光]

---

## 📊 关键参数快查 (Quick Reference Table)

| 参数 (Parameter) | 符号 (Symbol) | 测试条件 | 最小值 (Min.) | 典型值 (Typ.) | 最大值 (Max.) | 单位 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 正向电压 | VF | IF=[条件]mA | [VF_min] | [VF_typ] | [VF_max] | V |
| 光通量 | φV | IF=[条件]mA | [Flux_min] | [Flux_typ] | — | lm |
| 色坐标/波长 | CHC/Wd | IF=[条件]mA | [CHC_min] | [CHC_typ] | [CHC_max] | —/nm |
| 反向电流 | IR | VR=5V | — | — | [IR_max] | μA |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（Ta=25 °C，除非另外注明）

| 项目 (Items) | 符号 (Symbol) | 额定值 | 单位 |
| :--- | :---: | :---: | :---: |
| 耗散功率 | Pd | [Pd] | W |
| 结温 | Tj | [Tj_max] | °C |
| 正向直流电流 | IF | [IF_max] | mA |
| 正向峰值电流* | IFP | [IFP_max] | mA |
| 工作温度 | Topr | -40 ~ + [Topr_max] | °C |
| 储存温度 | Tstg | -40 ~ + [Tstg_max] | °C |
| 热阻（结-板） | Rth(j-b) | ≤ [Rth] | K/W |
| ESD（HBM） | ESD | ≥ [ESD] | kV |
| 焊接温度 | Tsol | 260°C for 5 Seconds | — |

*Pulse Width ≦200ms and Duty ≦1/10

---

## 📊 典型光电特性 (Typical Electrical & Optical Characteristics, Ta=25℃)

| 项目 (Items) | 符号 (Symbol) | 测试条件 | 最小值 (Min.) | 典型值 (Typ.) | 最大值 (Max.) | 单位 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 正向电压 | VF | IF=[条件1]mA | [VF1_min] | [VF1_typ] | [VF1_max] | V |
| 正向电压 | VF | IF=[条件2]mA | [VF2_min] | [VF2_typ] | [VF2_max] | V |
| 光通量 | φV | IF=[条件1]mA | [Flux1_min] | [Flux1_typ] | — | lm |
| 光通量 | φV | IF=[条件2]mA | [Flux2_min] | [Flux2_typ] | — | lm |
| 色坐标 (x/y) / 波长 | CHC/Wd | IF=[条件]mA | [CHC_min] | [CHC_typ] | [CHC_max] | — |
| 反向电流 | IR | VR=5V | — | — | [IR_max] | μA |

---

## 📐 封装外形尺寸 (Package Outline Dimensions)

- 外形尺寸：[长] × [宽] × [高] mm
- 发光区域：[发光区域尺寸] mm
- 公差：±0.2mm（除非另有说明）

### 引脚定义 (Pin Definition)

| 引脚号 (Pin No.) | 功能 (Function) |
| :---: | :--- |
| 1 | 阳极 (Anode) |
| 2 | 阴极 (Cathode) |

### 推荐焊盘布局 (Recommended Solder Pattern)

- 焊盘尺寸：[焊盘尺寸]
- 铜皮区域建议：>10×10mm（根据功率需求调整）

---

## 🔧 可靠性数据 (Reliability Data)

| 分类 | 测试项目 | 测试条件 | 持续时间 | 样本数 | 失效数 |
| :--- | :--- | :--- | :---: | :---: | :---: |
| 寿命测试 | 工作寿命测试 | Ta=85±5℃, IF=[测试电流]mA | 1000 Hrs | 11 | 0/11 |
| 寿命测试 | 高温高湿工作 | Ta=85±5℃, RH=85%, IF=[测试电流]mA | 1000 Hrs | 11 | 0/11 |
| 环境测试 | 高温储存 | Ta=125±5℃ | 1000 Hrs | 11 | 0/11 |
| 环境测试 | 低温储存 | Ta=-40±5℃ | 1000 Hrs | 11 | 0/11 |
| 环境测试 | 温湿度测试 | 85℃/85%RH | 1000 Hrs | 11 | 0/11 |
| 环境测试 | 热冲击测试 | -40℃←→125℃, 15min/10sec/15min | 1000 Cycles | 11 | 0/11 |
| ESD | HBM | 8KV | 10 Cycles | 11 | 0/11 |
| 焊接测试 | 耐焊接热 | 260±5℃, 10sec | 3次 | 22 | 0/22 |

**判定标准：**
- VF ≤ 初始值 × 1.2
- φV ≥ 初始值 × 0.85
- IR ≤ 规格上限

---

## 📦 包装信息 (Packing Information)

- 载带宽度：[载带宽度] mm
- 卷盘规格：[卷盘直径] mm
- 包装数量：[包装数量] pcs / reel
- 防潮等级：MSL Level 2（JEDEC J-STD-020E）
- 存储条件：30℃以下 / 70%RH以下，保质期12个月

---

## ⚠️ 使用注意事项 (Precautions For Use)

### 过流保护
必须使用限流电阻进行保护，否则微小电压偏移将导致大电流变化（可能烧毁）。

### 存储
1. 使用前请勿打开防潮袋
2. 存储条件：30℃以下，70%RH以下
3. 保质期：12个月
4. MSL等级：Level 2（JEDEC J-STD-020E）

### 焊接
1. 回流焊建议次数：不超过2次
2. 焊接时请勿对LED施加应力
3. 焊接后请勿弯曲电路板

### ESD防护
1. ESD和浪涌电流（EOS）可能损坏LED
2. 操作时必须佩戴ESD腕带、ESD鞋套或防静电手套
3. 所有设备、仪器和机器必须正确接地

---

## 📄 文档信息 (Document Information)

- 文档编号：[文档编号]
- 版本号：Rev.[版本号]
- 发布日期：[日期]
- 原始PDF文件名：`[原始文件名]`
- 数据来源：比亚迪半导体官方技术文档

---

*本文档由霸晶芯科技术团队整理，所有产品参数均基于比亚迪半导体官方公开技术文档。如需最新版本或选型支持，请联系霸晶芯科 FAE 团队。*
