# BYD Semiconductor Product Catalog

[![License](https://img.shields.io/badge/License-CC--BY--4.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Felix-rookie/BYD-Semiconductor-Product-Catalog/blob/main/CONTRIBUTING.md)

# 欢迎来到**比亚迪半导体产品目录开源社区**！🚀

---

## 🏢 关于我们与社区背景 (About Us & Background)

本开源社区由比亚迪半导体（BYD Semiconductor）核心代理商 —— **深圳市霸晶芯科实业发展有限公司（霸晶芯科）** 发起、搭建并进行长期维护。

### 为什么要做这个项目？ (Why This Project?)
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

- [ ] **01_功率半导体 (Power Semiconductors)** <-- 🎯 *当前主攻方向 (Current Focus)*
  - [ ] **IPM及单管-Si (IPMs & Discrete Devices - Si)**
  - [ ] **工业模块-Si (Industrial Modules - Si)**
  - [ ] **车用模块-Si (Automotive Modules - Si)**
  - [ ] **IPM及单管-SiC (IPMs & Discrete Devices - SiC)**
  - [ ] **车用模块-SiC (Automotive Modules - SiC)**
- [ ] **02_智能控制 IC (Smart Control ICs)**
  - [ ] **车规MCU (Automotive MCUs)**
  - [ ] **工业MCU (Industrial MCUs)**
  - [ ] **家电MCU (Home Appliance MCUs)**
  - [ ] **智能锁控MCU (Smart Lock MCUs)**
  - [ ] **电源IC (Power Management ICs / PMICs)**
  - [ ] **电池管理IC (Battery Management ICs / BMICs)**
- [ ] **03_智能传感器 (Smart Sensors)**
  - [ ] **电流电压传感器 (Current & Voltage Sensors)**
  - [ ] **角度位置传感器 (Angle & Position Sensors)**
  - [ ] **温度压力传感器 (Temperature & Pressure Sensors)**
  - [ ] **CMOS图像传感器 (CMOS Image Sensors)**
  - [ ] **生物识别 (Biometrics)**
- [ ] **04_光电半导体 (Optoelectronics)**
  - [ ] **智能车载 (Smart Automotive Optoelectronics)**
  - [ ] **影像模组 (Camera / Image Modules)**
  - [ ] **LED (Light Emitting Diodes)**
  - [ ] **结构件 (Structural Components)**

---

## 📂 仓库目录结构 (Repository Structure)

为了方便跨团队协作与多型号并发迁移，仓库采用**严谨的二级分类**与**模板化设计**：

```text
├── 01_Power_Semiconductors/       # 1. 功率半导体分类 (Power Semiconductors)
│   ├── IPM_Discretes_Si/          # IPM及单管-Si (IPMs & Discrete Devices - Si)
│   ├── Industrial_Modules_Si/     # 工业模块-Si (Industrial Modules - Si)
│   ├── Automotive_Modules_Si/     # 车用模块-Si (Automotive Modules - Si)
│   ├── IPM_Discretes_SiC/         # IPM及单管-SiC (IPMs & Discrete Devices - SiC)
│   └── Automotive_Modules_SiC/    # 车用模块-SiC (Automotive Modules - SiC)
├── 02_Smart_Control_ICs/          # 2. 智能控制 IC 分类 (Smart Control ICs)
│   ├── Automotive_MCU/            # 车规MCU (Automotive MCUs)
│   ├── Industrial_MCU/            # 工业MCU (Industrial MCUs)
│   ├── Home_Appliance_MCU/        # 家电MCU (Home Appliance MCUs)
│   ├── Smart_Lock_MCU/            # 智能锁控MCU (Smart Lock MCUs)
│   ├── Power_ICs/                 # 电源IC (Power Management ICs)
│   └── Battery_Management_ICs/    # 电池管理IC (Battery Management ICs)
├── 03_Smart_Sensors/              # 3. 智能传感器分类 (Smart Sensors)
│   ├── Current_Voltage_Sensors/   # 电流电压传感器 (Current & Voltage Sensors)
│   ├── Angle_Position_Sensors/    # 角度位置传感器 (Angle & Position Sensors)
│   ├── Temp_Pressure_Sensors/     # 温度压力传感器 (Temperature & Pressure Sensors)
│   ├── CMOS_Image_Sensors/        # CMOS图像传感器 (CMOS Image Sensors)
│   └── Biometrics/                # 生物识别 (Biometrics)
├── 04_Optoelectronics/            # 4. 光电半导体分类 (Optoelectronics)
│   ├── Smart_Automotive/          # 智能车载 (Smart Automotive Optoelectronics)
│   ├── Image_Modules/             # 影像模组 (Camera / Image Modules)
│   ├── LED/                       # LED (Light Emitting Diodes)
│   └── Structural_Components/     # 结构件 (Structural Components)
├── templates/                     # 统一的数据转化标准 Markdown 模板 (Standardized Markdown Templates)
│   ├── IGBT_Discrete_Template.md  # 硅基单管转换模板 (Si IGBT Discrete Template)
│   └── IPM_Module_Template.md     # IPM 智能功率模块模板 (IPM Module Template)
├── LICENSE                        # 开源协议 (CC-BY-4.0 License)
└── README.md                      # 社区主页导航 (Community Homepage)
```

---

## 🤝 如何参与贡献 (Contributing)

无论是修补了一个参数错漏，还是帮社区搬运、翻译了新的芯片型号，霸晶芯科和整个社区都无比欢迎你的加入！

### 快速开始 (Quick Start)
1. **查阅模板**：进入 `templates/` 目录，查看对应器件的标准化 Markdown 编写规范。
2. **认领型号**：在 Issue 列表中查看“型号认领区”，避免多人重复转换同一款芯片。
3. **提交 PR**：转换完成后，按照对应的分类目录提交 Pull Request，霸晶芯科的技术团队会第一时间进行 Review 并合并。

> 💡 **效率工具推荐 (Recommended Tools)**：建议使用 MinerU 或 Marker 等开源工具对原始 PDF 进行高效的表格识别，再利用大模型进行格式校验，可极大提升数据迁移效率。

---

## 👥 联系我们与技术支持 (Contact Us & Support)

作为比亚迪半导体的核心代理商，霸晶芯科拥有专业的 FAE 团队。如果你在选型、方案设计中遇到任何技术难题，欢迎通过以下渠道与我们取得联系：

* **项目负责人 (Project Maintainer)**：@Felix-rookie
* **企业官网 (Official Website)**：[深圳市霸晶芯科实业发展有限公司](http://你的官网链接地址)
* **技术支持群/微信交流圈 (Tech Support Group)**：*(欢迎提交 Issue 或留下您的联系方式，我们的技术团队会第一时间邀请您进入核心技术交流群)*
