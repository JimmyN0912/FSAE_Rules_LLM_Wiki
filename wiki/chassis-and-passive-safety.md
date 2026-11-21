---
id: chassis-and-passive-safety
title: 車架與被動安全規範（F 節）
rule_sections: ["F"]
scope: FSAE-IC (2027 V1)
sources:
  - raw/FSAE_Rules_2027_V1.pdf
  - raw/2026_FSAEJ_LocalRule_4th_20260616.pdf
last_updated: 2026-11-21
verified: true
---

# 車架與被動安全規範（F 節）

F 節（Chassis and Structural）規範了賽車的主結構（Primary Structure），無論車隊採用鋼管車架（Tube Frame）、碳纖維單體殼（Monocoque）或複合式車架，都必須在翻覆、正撞與側撞下守住車手的生存空間 `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.1, p.31]`。

## 1. 主結構通用工藝紅線（F.5.2–F.5.5）
- **彎管半徑（F.5.2.1）**：任何彎管的中心線最小彎曲半徑不得小於管徑的 **3 倍（3 × OD）**，且彎折處不得皺褶或破裂 `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.2.1-F.5.2.2, p.31]`。
- **管端封口（F.5.3.3）**：除防滾架底端外，受規範管材的所有開口端皆須焊接封蓋或塞入金屬堵頭 `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.3.3, p.32]`。
- **主結構鎖附（F.5.4）**：必須使用可拆式螺栓與螺帽（嚴禁膠合緊固件或盲孔螺絲），屬於 [[driver-ergonomics-and-controls|關鍵緊固件（T.8.2）]]，且耳片孔邊距比 **e/D ≥ 1.5** `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.4.1-F.5.4.3, p.32]`。
- **結構膠折減（F.5.5.3）**：若主結構使用結構膠黏合，SES 計算時會強制將參考或實測膠合強度**打對折（折減 50%）** `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.5.3, p.32]`。

## 2. 防滾架與 95% 男性模型「Percy」（F.5.6）
- **主/前防滾架（Main Hoop & Front Hoop）**：車架必須同時具備主防滾架與前防滾架，並以結構管件進行**三角形斜撐（Triangulated）**接入主結構 `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.6.1-F.5.6.2, p.32]`。
- **第 95 百分位男性二維模板「Percy」（F.5.6.5）** `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.6.5, p.33]`：
  - 臀部圓直徑 **200 mm**、肩頸圓直徑 **200 mm**、頭盔圓直徑 **300 mm**。
  - 臀圓至肩圓中心距 **490 mm**；肩圓至頭圓中心距 **280 mm**。
- **模板擺放條件（F.5.6.6）**：座椅調至最後、踏板調至最前，臀圓中心距踏板最後表面 **≥ 915 mm**，頭圓距頭枕 **≤ 25 mm**；所有防滾保護連線須與車手及 Percy 頭盔保持規定安全間隙 `[src: raw/FSAE_Rules_2027_V1.pdf, F.5.6.6, p.33]`。

## 3. 正面撞擊保護：IA + AIP + 前隔板（F.8）
- **防侵入板（AIP, Anti-Intrusion Plate, F.8.2）**：安裝於前隔板前端，防止吸能緩衝器穿刺進腳部空間。可選用鋼板、**≥ 4.0 mm 實心鋁板**或符合 `F.8.3` 的複材板 `[src: raw/FSAE_Rules_2027_V1.pdf, F.8.2.1, p.45]`。
- **AIP 鎖附規範（F.8.2.3）**：若採螺栓鎖附，至少須使用 **8 顆 ≥ 8 mm（或 5/16"）關鍵緊固件**，任兩顆螺栓中心距 **≥ 50 mm**，單顆拉拔與彎曲強度達 **15 kN**；若採焊接則每段焊道長 ≥ 25 mm 且焊空比 ≥ 1:1 `[src: raw/FSAE_Rules_2027_V1.pdf, F.8.2.3, p.45]`。
- **吸能緩衝器（IA）**：安裝於 AIP 前端，可選官方標準發泡/蜂巢式 Standard IA，或自製並提交撞擊測試報告（IAD）。

## 4. 單體殼與安全帶鎖點強度（F.7 / SES）
- 若採用碳纖維單體殼或替代管材，必須提交 **SES（Structural Equivalency Spreadsheet）** 並以平面等效法（Flat Panel Calculation, `F.4.4`）搭配三明治夾心板實體測試證明等效強度 `[src: raw/FSAE_Rules_2027_V1.pdf, F.4.4, p.31]`。
- **單體殼安全帶鎖點拉力（F.7.9.1）**：腰帶與防潛帶各鎖點須承受 **≥ 15 kN**；若兩者鎖點距離小於 125 mm，則每個鎖點須承受 **≥ 30 kN** `[src: raw/FSAE_Rules_2027_V1.pdf, F.7.9.1, p.44]`。

> [!NOTE]
> **日本站（FSAEJ 2026）在地補充**：日本站允許採用 JIS `STKM11A`（最小抗拉強度 290 N/mm²）作為基準鋼材（`J2026-F-01`），並認定 DuPont Styro `DX-45` 等效於標準發泡緩衝器 `IMPAXX 700`（`J2026-F-04`）；詳見 [[fsaej-local-rules-diff]] `[src: raw/2026_FSAEJ_LocalRule_4th_20260616.pdf, pp.1-2]`。

---
**相關頁面**：[[driver-ergonomics-and-controls|座艙與煞車規範]] · [[technical-inspection-gauntlet|車檢流程]] · [[fsaej-local-rules-diff|日本站差異]]
