# BYD IGBT 单管 (Si IGBT Discrete) Markdown File Generation Summary

**Generated:** 2026-07-07
**Output directory:** `/home/codex/.openclaw/workspace/igbt_output/`
**Template:** 硅基单管转换模板_IGBT_Discrete_Template.md
**Reference (style):** BGNE40Q120SD-A_硅基IGBT单管_Si_IGBT_Discrete.md

---

## Generated Files (13 total)

| # | File Name | Model | Package | Grade | VCES | IC |
|:-:|:---|:---|:---:|:---:|:---:|:---:|
| 1 | `BGF15T65SD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGF15T65SD | TO220F-3 | Industrial | 650V | 15A |
| 2 | `BGF15T65SD-I_硅基IGBT单管_Si_IGBT_Discrete.md` | BGF15T65SD-I | TO220F-3 | Industrial | 650V | 15A |
| 3 | `BGM160T65SD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGM160T65SD | TO247Plus | Automotive (AEC-Q101) | 650V | 160A |
| 4 | `BGM160T75SD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGM160T75SD | TO247Plus | Automotive (AEC-Q101) | 750V | 160A |
| 5 | `BGM50Q120SD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGM50Q120SD | TO247Plus | Automotive (AEC-Q101) | 1200V | 50A |
| 6 | `BGN20T65SD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN20T65SD | TO247-3 | Industrial | 650V | 20A |
| 7 | `BGN30T65HD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN30T65HD | TO247-3 | Industrial | 650V | 30A |
| 8 | `BGN30T65SD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN30T65SD | TO247-3 | Industrial | 650V | 30A |
| 9 | `BGN40Q120K_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN40Q120K | TO247-3 | Automotive (AEC-Q101) | 1200V | 40A |
| 10 | `BGN40Q120SD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN40Q120SD | TO247-3 | Automotive (AEC-Q101) | 1200V | 40A |
| 11 | `BGN40T65HD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN40T65HD | TO247-3 | Industrial | 650V | 40A |
| 12 | `BGN60T65HD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN60T65HD | TO247-3 | Industrial | 650V | 60A |
| 13 | `BGN80V65HD_硅基IGBT单管_Si_IGBT_Discrete.md` | BGN80V65HD | TO-247 | Industrial | 650V | 80A |

---

## Special Handling Notes

### BGN40Q120K (No anti-parallel diode)
- Topology marked as "IGBT" (not "IGBT+FRD")
- No VF row in static characteristics
- No diode switching section (switching table only has IGBT rows)
- No IF/IFpuls rows in max ratings
- No Rth(j-c) for diode (marked as "-")
- Features mention "单管拓扑" and "无内置反并联二极管"

### BGM Series (TO247Plus package)
- BGM160T65SD, BGM160T75SD, BGM50Q120SD use TO247Plus
- Package dimensions use the TO247Plus-specific table format
- BGM160T65SD and BGM160T75SD share similar dimensions table
- All automotive grade with AEC-Q101 badge

### BGF Series (TO220F-3 package)
- BGF15T65SD and BGF15T65SD-I use TO220F-3
- Different pinout from TO247 devices
- Lower Ptot (37.5W) and higher Rth(j-a) (62.5°C/W)
- Different packing (50 pcs/tube, 2000 pcs/carton)

### BGN80V65HD (TrenchFS, +175°C Tjop)
- TrenchFS technology with wider VGE(th) range (2.0-4.0V)
- Tjop: -40 to +175°C (wider than standard +150°C)
- No tsc, IC(sc), or RBSOA specified
- Package is TO-247 (not TO247-3)
- Features: "Low gate charge" and "Maximum operating temperature of 175°C"
- Cres = 10 pF (extremely low)

### BGM50Q120SD (No capacitance data)
- Cies/Coes/Cres not specified in datasheet
- Marked as "-" in the dynamic characteristics table

---

## Data Sources
All technical parameters extracted from BYD official datasheets stored in:
`/home/codex/.openclaw/workdir/比亚迪产品规格书_extracted/比亚迪半导体产品规格书/IGBT单管/`

---
