# 比亚迪半导体 (BYD) LED - BOF-2016SR-DMC

[![Quality](https://img.shields.io/badge/Quality-Commercial%20Grade-green.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

本页面由比亚迪半导体核心代理商——**深圳市霸晶芯科实业发展有限公司（霸晶芯科）**专业技术团队进行结构化转换与合规性校验。

---

## 📌 产品概述 (Product Overview)

**BOF-2016SR-DMC** 是一款基于—工艺的车规级/工业级 SMD LED。该器件采用2016封装，具有Super发光特性，适用于汽车照明、日行灯、雾灯等汽车级应用场景。

### 🌟 核心特性 (Features)
* **封装尺寸**：2.04×1.64×0.85 mm
* **发光颜色**：Super
* **视角**：130°
* **芯片材料**：—
* **胶体类型**：Clear (无色透明)
* **符合RoHS标准**：环保无铅设计
* **MSL等级**：Level 2（JEDEC J-STD-020E）
* **ESD耐压**：≥2 kV（HBM）

### 🚗 典型应用 (Applications)
* Automotive light
* Day time running light
* Reversing light

---

## 📊 关键参数快查 (Quick Reference Table)

| 参数 (Parameter) | 符号 (Symbol) | 条件 | 最小值 (Min.) | 典型值 (Typ.) | 最大值 (Max.) | 单位 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 正向电压 | VF | IF=150mA | 1.6 | 2.0 | 2.4 | V |
| 光通量 | φV | IF=150mA | 12 | 18 | — | lm |
| 色坐标 | CHC | IF=150mA | — | — | — | — |
| 反向电流 | IR | VR=5V | — | — | 10 | μA |

---

## ⚡ 最大绝对额定值 (Absolute Maximum Ratings)

（Ta=25 °C，除非另外注明）

| 项目 (Items) | 符号 (Symbol) | 额定值 | 单位 |
| :--- | :---: | :---: | :---: |
| 耗散功率 | Pd | 1.5W | W |
| 结温 | Tj | 150 | °C |
| 正向直流电流 | IF | 500 | mA |
| 正向峰值电流* | IFP | — | mA |
| 工作温度 | Topr | -40 ~ ++125 | °C |
| 储存温度 | Tstg | -40 ~ ++125 | °C |
| 热阻（结-板） | Rth(j-b) | — | K/W |
| ESD（HBM） | ESD | ≥2 | kV |
| 焊接温度 | Tsol | 260°C for 5 Seconds | — |

*Pulse Width ≦0.1msec and Duty ≦1/10

---

## 📐 封装外形尺寸 (Package Outline Dimensions)

- 外形尺寸：2.04×1.64×0.85 mm
- 发光区域：—
- 公差：±0.2mm（除非另有说明）

### 引脚定义 (Pin Definition)

| 引脚号 (Pin No.) | 功能 (Function) |
| :---: | :--- |
| 1 | 阳极 (Anode) |
| 2 | 阴极 (Cathode) |

---

## 🔧 可靠性数据 (Reliability Data)

| 分类 | 测试项目 | 测试条件 | 持续时间 | 样本数 | 失效数 |
| :--- | :--- | :--- | :---: | :---: | :---: |
| 寿命测试 | 工作寿命测试 | Ta=85±5℃, IF={life_test_current}mA | 1000 Hrs | {sample_size} | 0/{sample_size} |
| 寿命测试 | 高温高湿工作 | Ta=85±5℃, RH=85%, IF={life_test_current}mA | 1000 Hrs | {sample_size} | 0/{sample_size} |
| 环境测试 | 高温储存 | Ta=125±5℃ | 1000 Hrs | {sample_size} | 0/{sample_size} |
| 环境测试 | 低温储存 | Ta=-40±5℃ | 1000 Hrs | {sample_size} | 0/{sample_size} |
| 环境测试 | 温湿度测试 | 85℃/85%RH | 1000 Hrs | {sample_size} | 0/{sample_size} |
| 环境测试 | 热冲击测试 | -40℃←→125℃, 15min/10sec/15min | 1000 Cycles | {sample_size} | 0/{sample_size} |
| ESD | HBM | {esd_val}KV | 10 Cycles | {sample_size} | 0/{sample_size} |
| 焊接测试 | 耐焊接热 | 260±5℃, 10sec | 3次 | 22 | 0/22 |

---

## 📦 包装信息 (Packing Information)

- 载带规格：{carrier_width}mm
- 卷盘规格：{reel_diam}mm
- 包装数量：{pack_qty} pcs / reel
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
1. 回流焊不超过2次
2. 焊接时请勿对LED施加应力
3. 焊接后请勿弯曲电路板

### ESD防护
1. ESD和浪涌电流可能损坏LED
2. 操作时必须佩戴ESD腕带、ESD鞋套或防静电手套
3. 所有设备、仪器和机器必须正确接地

---

## 📄 文档信息 (Document Information)

- 文档编号：{doc_id}
- 版本号：Rev.{rev}
- 原始PDF文件名：`{pdf_filename}`
- 数据来源：比亚迪半导体官方技术文档

---

🌐 社区数据维护：[BYD Semiconductor Product Catalog 开源社区](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog)  
技术支持与选型对接：由比亚迪半导体核心代理商【霸晶芯科】FAE团队全权提供。
