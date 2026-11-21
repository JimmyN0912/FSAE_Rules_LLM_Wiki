---
id: 2027-static-sdf-scenario
title: 2027 靜態新制：Software-Defined Feature（簡報與成本共題）
rule_sections: ["S.2", "S.3"]
scope: FSAE-IC (2027 Season)
sources:
  - raw/2027_FSAE_Presentation_Concept.pdf
  - raw/2027_FSAE_Cost_Scenario.pdf
  - raw/2027_Presentation__Request_for_Proposal_-_Team_Response_Scoring_Rubric.pdf
  - raw/2027_Presentation_Virtual_&_Finals_Judging_Rubric.pdf
  - raw/Presentation_Concept_Discussion_and_Q&A_-_FAQ.final.pdf
last_updated: 2026-11-21
verified: true
---

# 2027 靜態新制：Software-Defined Feature（簡報與成本共題）

2027 賽季靜態賽事迎來一項重大變革：**商業簡報（Presentation, 75 分）** 與 **成本與製造（Cost & Manufacturing, 100 分）** 雖然維持獨立繳件、獨立評審與獨立計分，但兩者**共用同一個核心主題——「Software-Defined Feature（軟體定義車輛功能，SDF）」** `[src: raw/2027_FSAE_Presentation_Concept.pdf, p.2; raw/2027_FSAE_Cost_Scenario.pdf, p.2]`。

## 1. 什麼是 2027 共用情境（Software-Defined Feature）？
SAE International 設立了一項假想創新補助計畫（Grant），邀請車隊提案一項**主要透過軟體控制或強化、不需大規模改動硬體**即可更新或優化的單一車載功能，藉以提升 FSAE 賽車的 **安全（Safety）、效率（Efficiency）與／或性能（Performance）**，並說明如何擴展到**一般乘用車或商用車隊** `[src: raw/2027_FSAE_Presentation_Concept.pdf, p.4; raw/Presentation_Concept_Discussion_and_Q&A_-_FAQ.final.pdf, pp.5-7]`。

- **對 IC 車隊的實務重點（官方 FAQ 釐清）** `[src: raw/Presentation_Concept_Discussion_and_Q&A_-_FAQ.final.pdf, pp.6-8]`：
  - 功能必須是**車載（In-vehicle）功能**（例如轉向不足控制、煞車溫度監測、燃油效率最佳化、機油壽命監測），不能只做車廠製造輔助工具。
  - **不須在賽場實裝或現場展示**，但必須立足於車隊現有 IC 車輛架構，明確區分既有硬體與小幅升級（例如新增一顆感測器），且不可拿 EV 專屬功能硬套在 IC 車上。
  - **必須揭露 AI 使用情形**：須說明開發該功能本身是否考量或使用 AI（包含 AI 輔助寫程式須計入研發工時），且團隊須能親自解釋所有提交內容。
  - **補助金額無上限**，但必須合理且清楚列出所有實作成本；簡報只估「研發工時（Labor Hours）」，不需把工時換算成美元時薪，也不用估算未來量產擴展階段的成本。

## 2. 商業簡報三輪淘汰賽（Presentation — 75 分）
2027 商業簡報採「三輪晉級淘汰制」 `[src: raw/2027_FSAE_Presentation_Concept.pdf, pp.3, 6-8]`：

| 輪次 | 形式與規格限制 | 評分尺規（Rubric）拆解 |
| :--- | :--- | :--- |
| **Round 1：書面 RFP** | 最多 **8 頁**、字體 ≥ 12 pt（Arial 或 Times New Roman） | 滿分 **20 分**：內容 10 + 組織架構 5 + 溝通與視覺 5 `[src: raw/2027_Presentation__Request_for_Proposal_-_Team_Response_Scoring_Rubric.pdf, p.1]` |
| **Round 2：線上簡報** | MS Teams 30 分鐘時段：**簡報 ≤ 10 分鐘**（超時強制中止）+ **Q&A ≤ 5 分鐘** | 滿分 **50 分**：內容 15 + 組織 10 + 表達 10 + 媒體品質 7 + 問答 8 `[src: raw/2027_Presentation_Virtual_&_Finals_Judging_Rubric.pdf, p.1]` |
| **Round 3：決賽簡報** | 晉級隊伍於 Michigan International Speedway 現場簡報（沿用 10+5 分鐘規範，自備筆電與投影設備） | 依 50 分尺規評選前 3 名 `[src: raw/2027_FSAE_Presentation_Concept.pdf, p.8]` |

## 3. 成本情境題（Cost Scenario — 屬於 100 分成本項目之一）
成本評審包含三大塊：整車 Cost Report、賽場現場討論、以及 **2027 Cost Scenario** `[src: raw/2027_FSAE_Cost_Scenario.pdf, pp.3-5]`：
- **賽前繳件（< 25 MB 合併 PDF）**：
  1. **Document Index（DI）**：列出所有文件編號、標題與備註。
  2. **Costed BOM**：僅列出因該 SDF 功能而異動的零件，並與整車 Cost Report 一致，但**特別須納入研發（R&D）成本**（與整車 Cost Report 最大差異！）。
  3. **Feature Overview（≤ 5 頁）+ 工程圖面（≤ 5 頁）**：合計上限 10 頁（BOM 不計頁數），字體 ≥ 12 pt。
- **現場討論（約 15 分鐘）**：必須攜帶**紙本 1 頁摘要**（不得含新資訊）與完整賽前繳件紙本 `[src: raw/2027_FSAE_Cost_Scenario.pdf, p.5]`。

---
**相關頁面**：[[competition-scoring-1000pts|1,000 分計分總覽]] · [[rulebook-structure|規則書總則]] · [[glossary|術語表]]
