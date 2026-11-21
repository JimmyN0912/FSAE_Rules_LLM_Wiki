# Formula SAE (IC) Rulebook LLM Wiki — 全站知識索引

> **定位**：基於 **9 份真實官方 PDF（`raw/`）** 編譯而成的 **Formula SAE 內燃機組（IC）** 新手知識庫。  
> **最後更新**：2026-11-21 ｜ **已攝取官方 PDF 數**：9 份 ｜ **知識頁數**：9 頁（含術語表）

---

## 一、新手學習路徑（Learning Path）

1. **[[rulebook-structure|1. 2027 規則書架構與行政規範（GR / AD / PS）]]**  
   搞懂 FSAE「模擬新創車廠造車」的本質、12 大英文字母章節地圖，以及違反意圖（`GR.4.6`）等四條紅線總則。
2. **[[chassis-and-passive-safety|2. 車架與被動安全規範（F 節）]]**  
   掌握防滾架、95% 男性模板 Percy（`F.5.6.5`）、防侵入板 AIP（`F.8.2`）、吸能緩衝器 IA 與單體殼 SES 驗證。
3. **[[driver-ergonomics-and-controls|3. 車體幾何、座艙防護與煞車系統（V / T / VE 節）]]**  
   理解軸距 ≥ 1,525 mm、三維隔熱（傳導/對流/輻射）、防火牆、雙獨立液壓煞車（2,000 N 踏板強度）與 BOTS 開關。
4. **[[ic-powertrain-rules|4. IC 內燃機動力、限流閥與斷電系統（IC 節）]]**  
   看懂 IC 組靈魂：≤ 710 cc 四行程、20.0 mm（汽油）/ 19.0 mm（E85）進氣限流閥、禁包隔熱布、103/110 dBC 噪音上限與斷電迴路。
5. **[[technical-inspection-gauntlet|5. IC 車檢四關卡全流程（IN 節）]]**  
   集滿 4 張車檢貼紙才能下場：整車與模板機檢 → 45°/60° 傾斜測試 → 103/110 dBC 噪音與斷電開關測試 → 四輪鎖死不熄火煞車測試。
6. **[[competition-scoring-1000pts|6. 1,000 分制靜態與動態計分總覽（S / D 節 + IC 設計評分）]]**  
   拆解靜態 325 分（含 IC 設計評分表 7 大子系統 150 分）與動態 675 分（含「至少 4 位車手」規則與耐久+節能 375 分核心戰略）。
7. **[[2027-static-sdf-scenario|7. 2027 靜態新制：Software-Defined Feature（簡報 + 成本共題）]]**  
   整合 5 份 2027 官方簡報與成本文件：三輪淘汰賽制、評分尺規、AI 揭露規定與含 R&D 成本的 Costed BOM。
8. **[[fsaej-local-rules-diff|8. 2026 日本站（FSAEJ）在地規則差異速查]]**  
   統整日本站最易踩雷的覆寫條文：僅供 RON 100 汽油、紅色主斷電開關、防火牆禁鋁箔膠帶、旗號考試、145% 耐久賽門檻與 16 pt 字體紅線。
9. **[[glossary|9. 新手必備術語與縮寫對照表]]**  
   速查 AIP、BOM、BOTS、DOO、Egress、Percy、Restrictor、RFP、SDF、SES、SIS 等高頻術語。

---

## 二、已攝取之原始一手 PDF 清單（`raw/` — 共 9 份）
1. `raw/FSAE_Rules_2027_V1.pdf`（147 頁，2027 FSAE 官方規則書 V1）
2. `raw/2026_FSAEJ_LocalRule_4th_20260616.pdf`（36 頁，2026 日本站在地規則第 4 版）
3. `raw/2026-_FSAE_IC_Design_Score_Sheet_20251008.pdf`（11 頁，2026 IC 設計評分表）
4. `raw/2027_Design_Briefing_Template.pdf`（26 頁，2027 設計簡報官方模板）
5. `raw/2027_FSAE_Cost_Scenario.pdf`（5 頁，2027 成本情境題指南）
6. `raw/2027_FSAE_Presentation_Concept.pdf`（8 頁，2027 商業簡報主題指南）
7. `raw/2027_Presentation__Request_for_Proposal_-_Team_Response_Scoring_Rubric.pdf`（1 頁，Round 1 RFP 評分尺規）
8. `raw/2027_Presentation_Virtual_&_Finals_Judging_Rubric.pdf`（1 頁，Round 2/3 評分尺規）
9. `raw/Presentation_Concept_Discussion_and_Q&A_-_FAQ.final.pdf`（9 頁，2027 簡報主題官方 FAQ）

---

## 三、系統規範與日誌
- [SCHEMA.md](../SCHEMA.md) — Wiki 結構、引用規範與 Loop A / Loop B 工作流定義
- [log.md](./log.md) — 完整 Ingest、錯誤攔截、Lint 驗證與簡報編譯紀錄
