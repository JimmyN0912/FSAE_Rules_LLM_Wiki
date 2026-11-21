---
id: competition-scoring-1000pts
title: 1,000 分制靜態與動態計分總覽（S / D 節 + IC 設計評分拆解）
rule_sections: ["S", "D"]
scope: FSAE-IC (2027 V1 + 2026 IC Design Score Sheet)
sources:
  - raw/FSAE_Rules_2027_V1.pdf
  - raw/2026-_FSAE_IC_Design_Score_Sheet_20251008.pdf
  - raw/2027_Design_Briefing_Template.pdf
last_updated: 2026-11-21
verified: true
---

# 1,000 分制靜態與動態計分總覽（S / D 節）

依據《2027 Formula SAE Rules V1》`S.1` 與 `D.1.1`，賽事總分精確為 **1,000 分**，分為**靜態項目 325 分（32.5%）**與**動態項目 675 分（67.5%）** `[src: raw/FSAE_Rules_2027_V1.pdf, S.1, p.125; D.1.1, p.132]`。

## 1. 全賽事 1,000 分完整配分表

| 類別 | 比賽項目 | 滿分 | 佔比 | 關鍵規則與公式亮點 |
| :--- | :--- | :---: | :---: | :--- |
| **靜態（325 分）** | Engineering Design（工程設計） | **150** | 15.0% | 7 大子系統評分 + Design Briefing（≤ 56 頁） |
| | Cost & Manufacturing（成本製造） | **100** | 10.0% | Cost Report + 現場答辯 + [[2027-static-sdf-scenario|2027 成本情境題]] |
| | Presentation（商業簡報） | **75** | 7.5% | 三輪淘汰制（[[2027-static-sdf-scenario|2027 Software-Defined Feature]]） |
| **動態（675 分）** | Endurance（耐久賽） | **275** | 27.5% | ~22 km、雙車手換手、計時 250 分 + 圈數 25 分 |
| | Autocross（計時賽） | **125** | 12.5% | 平均時速 40–48 km/h，同時決定耐久賽起跑順位 |
| | Acceleration（直線加速） | **100** | 10.0% | 2 位車手共 4 趟；撞錐 +2 秒、衝出賽道 DNF |
| | Efficiency（節能油耗） | **100** | 10.0% | 於耐久賽同步量測加油至刻度線（**須完賽**） |
| | Skidpad（八字繞錐） | **75** | 7.5% | 圓心距 18.25 m、內圓徑 15.25 m；撞錐 +0.125 秒 |
| **總計** | **Overall Competition** | **1,000** | **100.0%** | `325 + 675 = 1,000` `[src: raw/FSAE_Rules_2027_V1.pdf, pp.125, 132]` |

---

## 2. 工程設計 150 分怎麼評？（IC Design Score Sheet）
新手常以為設計賽只是展示 CAD 圖，但依據官方《FSAE IC Design Score Sheet》，評審會從 **7 大子系統**（總計 150 分）與 **4 大面向（各約佔 25%）** 深度檢驗車隊的工程理解 `[src: raw/2026-_FSAE_IC_Design_Score_Sheet_20251008.pdf, pp.1-2]`：

- **7 大子系統配分（合計 150 分）**：
  - **Powertrain（IC 動力）**：30 分
  - **Chassis（車架結構）**：30 分
  - **Overall Vehicle（整車整合與目標）**：25 分
  - **Vehicle Dynamics（車輛動態與輪胎懸吊）**：25 分
  - **Aerodynamics（空力與散熱）**：15 分
  - **Driver Interface（車手介面、煞車與脫逃）**：15 分
  - **Low Voltage / Data Acquisition（低壓電系與資料擷取）**：10 分
- **4 大評核面向（各 ~25%）**：**Design（設計與理論分析）**、**Build（製造與實車一致度）**、**Refinement/Validation（實測驗證與修正）**、**Understanding（團隊是否真正懂原理）** `[src: raw/2026-_FSAE_IC_Design_Score_Sheet_20251008.pdf, p.2]`。
- **2027 Design Briefing 提交規格**：須為 PDF 檔、**< 25 MB**、總頁數 **≤ 56 頁**（無人車組 ≤ 63 頁），字體 **≥ 12 pt（建議 16+ pt）**，須包含整車目標、配分目標與重量分配圓餅圖 `[src: raw/2027_Design_Briefing_Template.pdf, pp.2, 10-11]`。

---

## 3. 動態賽道核心規則與車手人數下限（D 節）
- **至少需要 4 位車手！（D.7.1）**：規則明訂**每位車手最多只能參加 3 個動態項目**，且 Efficiency 雖與 Endurance 同時進行但**計為獨立項目**——因此車隊至少需要 **4 位合格車手** 才能跑滿全部動態項目 `[src: raw/FSAE_Rules_2027_V1.pdf, D.7.1, p.136]`。
- **維修區推車規定（D.2.1）**：在動態區以外移動賽車，必須**熄火並裝上推車桿（Push Bar）**、座艙內有車手操控方向盤與煞車，且旁有隊員步行陪同（有空力翼片須左右各 1 人），違規每次扣 **25 分** `[src: raw/FSAE_Rules_2027_V1.pdf, D.2.1, p.132]`。
- **錐筒與出界罰則（D.8–D.10）**：
  - **DOO（Cone Down or Out）**：直線加速每顆 **+2 秒**，八字繞錐每顆 **+0.125 秒**；**OC（Off Course，四輪出界或漏門）** 該趟直接 **DNF** `[src: raw/FSAE_Rules_2027_V1.pdf, D.8-D.10, pp.136-139]`。
- **耐久賽（275 分）+ 節能（100 分）= 375 分（37.5%）**：
  - 耐久賽總長約 **22 km**（平均時速 48–57 km/h、最高約 105 km/h），禁止輪對輪競速與倒車，中途強制換第二位車手且開始後禁止修車 `[src: raw/FSAE_Rules_2027_V1.pdf, D.12.1-D.12.2, p.141]`。
  - 耐久賽完賽才可獲得計時分數（最高 250 分，另有最高 25 分圈數分），且**節能賽（100 分）** 靠賽前後加滿至油箱刻度線（嚴禁搖晃車體！）計算油耗 `[src: raw/FSAE_Rules_2027_V1.pdf, D.12.13, D.13.2, p.145]`。

---
**相關頁面**：[[2027-static-sdf-scenario|2027 簡報與成本新制（SDF）]] · [[technical-inspection-gauntlet|先過車檢才能下場]] · [[fsaej-local-rules-diff|日本站耐久賽 145% 門檻]]
