# BYD Semiconductor Product Catalog (比亚迪半导体产品目录开源社区)

[![License](https://img.shields.io/badge/License-CC--BY--4.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog/blob/main/CONTRIBUTING.md)

# 欢迎来到**比亚迪半导体产品目录开源社区**！🚀

---

## 🏢 关于我们与社区背景

本开源社区由比亚迪半导体（BYD Semiconductor）核心代理商 —— **深圳市霸晶芯科实业发展有限公司（霸晶芯科）** 发起、搭建并进行长期维护。

### 为什么要做这个项目？
传统的 PDF 规格书（Datasheet）在工程师选型、参数对比以及版本控制上存在天然的检索隔阂。我们致力于通过**数字化、开源化**的方式，将比亚迪半导体的产品手册转化为结构清晰、对开发者友好的 **Markdown 格式**。
* **对于工程师**：可以实现秒级参数检索、一键对比、无缝集成到团队的内部知识库或 Wiki 中。
* **对于原厂与生态**：依托代理商的技术桥梁，联合原厂 FAE 与社区核心开发者，共同打造一个最懂工程师的半导体产品数据与技术交流生态。

---

## 📢 权威性与合规声明 (Disclaimer)

1. **渠道正规，数据保障**：本仓库内所有产品参数、引脚定义及规格说明，均基于比亚迪半导体官方公开披露的最新技术文档，并由霸晶芯科专业技术团队进行合规性与准确性校验。
2. **知识产权**：本仓库所涉及的比亚迪半导体相关品牌标识、商标及原始文档版权均归原厂所有。
3. **安全与合规**：本社区严格遵守信息安全规范，仅对**已公开披露**的产品规格进行结构化整理，绝不涉及、不收集、不传播任何未公开的商业机密或核心专利技术。

---

## 🗺️ 产品线路线图 (Roadmap)

我们计划逐步建立覆盖比亚迪半导体全系列的产品目录体系。当前阶段，我们优先攻坚**功率半导体**：

- [ ] **01_功率半导体 (Power Semiconductors)** <-- 🎯 *当前主攻方向*
  - [ ] IGBT 单管 (IGBT Discretes)
  - [ ] IGBT 模块 (IGBT Modules)
  - [ ] SiC 器件 (SiC Devices)
- [ ] **02_智能控制 IC (Smart Control ICs)**
  - [ ] 车规级 MCU
  - [ ] 工业/消费级 MCU
- [ ] **03_智能传感器 (Smart Sensors)**
  - [ ] 电流传感器
  - [ ] CMOS 图像传感器
- [ ] **04_光电半导体 & 功率驱动 (Optoelectronic & Drivers)**

---

## 📂 仓库目录结构

```text
├── 01_Power_Semiconductors/       # 功率半导体
│   ├── IGBT_Discretes/            # 👈 起步方向：IGBT单管
│   │   ├── BG40N120A.md           # 示例：具体型号产品页面
│   │   └── README.md              # 该分类下的子索引
│   └── SiC_MOSFETs/
├── 02_Smart_Control_ICs/          # 智能控制IC
├── templates/                     # 统一的数据转化 Markdown 模板
│   └── IGBT_Discrete_Template.md  # IGBT单管转换模板
├── README.md
└── LICENSE                        # 采用 CC-BY-4.0 开源协议
