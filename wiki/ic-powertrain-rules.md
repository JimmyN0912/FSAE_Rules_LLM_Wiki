---
id: ic-powertrain-rules
title: IC 內燃機動力、限流閥、排氣與斷電系統（IC 節）
rule_sections: ["IC"]
scope: FSAE-IC (2027 V1)
sources:
  - raw/FSAE_Rules_2027_V1.pdf
  - raw/2026_FSAEJ_LocalRule_4th_20260616.pdf
last_updated: 2026-11-21
verified: true
---

# IC 內燃機動力、限流閥、排氣與斷電系統（IC 節）

IC 節（Internal Combustion Engine Vehicles）是內燃機組的核心技術邊界，從引擎排氣量、標誌性的 20 mm 進氣限流閥，到排氣位置、噪音上限與斷電迴路都有極精確的數值規定 `[src: raw/FSAE_Rules_2027_V1.pdf, pp.81-91]`。

## 1. 引擎與動力架構限制（IC.1）
- **引擎型式（IC.1.1.1）**：必須為**四行程活塞引擎**，總排氣量 **≤ 710 cc** `[src: raw/FSAE_Rules_2027_V1.pdf, IC.1.1.1, p.81]`。
- **禁止油電混合（IC.1.1.2）**：禁止使用儲能驅動馬達的混合動力系統（Hybrid） `[src: raw/FSAE_Rules_2027_V1.pdf, IC.1.1.2, p.81]`。
- **進氣與油路包覆（IC.1.2 / IC.2.2）**：整個進氣與燃油系統須位於輪胎包絡面（Tire Surface Envelope）內；凡距地低於 **350 mm** 的進氣零件，必須受側面/後方防撞結構保護 `[src: raw/FSAE_Rules_2027_V1.pdf, IC.1.2, IC.2.2.2, p.81]`。
- **進氣歧管固定（IC.2.3）**：須以支架與機械緊固件鎖附於引擎本體，**嚴禁僅用管束（Hose clamps）、束帶或保險絲固定**，且螺絲須具備防鬆機構（T.8.3） `[src: raw/FSAE_Rules_2027_V1.pdf, IC.2.3, p.81]`。

## 2. 招牌規則：單一圓形進氣限流閥（IC.2.4–IC.2.5）
所有進入引擎的空氣都必須通過一個不可移動、不可變形的單一圓形限流閥 `[src: raw/FSAE_Rules_2027_V1.pdf, IC.2.4.3-IC.2.4.5, p.82]`：

| 燃油類別 | 限流閥最大直徑 | 備註 |
| :--- | :---: | :--- |
| **汽油（Gasoline）** | **20.0 mm** | 全球 FSAE 標準汽油上限 `[src: raw/FSAE_Rules_2027_V1.pdf, IC.2.4.3.a, p.82]` |
| **E85（85% 乙醇）** | **19.0 mm** | 較小口徑以平衡乙醇含氧與降溫優勢 `[src: raw/FSAE_Rules_2027_V1.pdf, IC.2.4.3.b, p.82]` |

- **增壓系統順序（IC.2.4.2.b）**：若使用渦輪或機械增壓，順序強制為：**限流閥（Restrictor）→ 壓縮機（Compressor）→ 節氣門（Throttle Body）→ 引擎**；增壓車禁止使用化油器（`IC.3.1.1.b`），且中冷器必須位於節氣門下游（`IC.2.5.1`） `[src: raw/FSAE_Rules_2027_V1.pdf, IC.2.4-IC.3.1, p.82]`。
- **集氣箱與管路限制（IC.2.5.3–IC.2.5.4）**：節氣門上游不得設置集氣箱（Plenum），且限流閥至節氣門之間進氣道截面積上限為 **2,825 mm²** `[src: raw/FSAE_Rules_2027_V1.pdf, IC.2.5.3-IC.2.5.4, p.82]`。
- **曲軸箱通氣管（IC.2.6）**：若回接至進氣系統，必須接在**限流閥上游** `[src: raw/FSAE_Rules_2027_V1.pdf, IC.2.6, p.82]`。

## 3. 高壓直噴與排氣系統（IC.6–IC.7）
- **高壓燃油系統（≥ 10 Bar / DI, IC.6.2）**：高壓油管須為不鏽鋼硬管或 Aeroquip FC807 PTFE 編織管，不得使用彈性體密封圈，且每隔 **100 mm** 須以機械緊固件剛性固定於引擎結構上 `[src: raw/FSAE_Rules_2027_V1.pdf, IC.6.2.1-IC.6.2.2, p.89]`。
- **排氣出口位置（IC.7.2.2）**：不得超過後軸中心線後方 **45 cm**，且離地高度不得超過 **60 cm** `[src: raw/FSAE_Rules_2027_V1.pdf, IC.7.2.2, p.90]`。
- **禁止包覆隔熱布（IC.7.2.4）**：排氣歧管與排氣系統外側**禁止纏繞纖維／吸油性材質（如 Header Wrap）**，避免吸附漏油引發火災 `[src: raw/FSAE_Rules_2027_V1.pdf, IC.7.2.4, p.90]`。
- **噪音上限（IC.7.5 / IN.12.5）**：怠速 **≤ 103 dBC**、拉轉測試 **≤ 110 dBC**（詳見 [[technical-inspection-gauntlet]]） `[src: raw/FSAE_Rules_2027_V1.pdf, IC.7.5, p.90; IN.12.5, p.121]`。

## 4. 啟動、低壓電氣與斷電迴路（IC.8–IC.9）
- **車載啟動馬達（IC.8.1）**：車輛隨時都必須能靠**車載啟動馬達**自行發動（包含耐久賽換車手後） `[src: raw/FSAE_Rules_2027_V1.pdf, IC.8.1, p.90]`。
- **斷電迴路（Shutdown Circuit, IC.9.1）**：由**外部主斷電開關（Primary Master Switch）**、**座艙主開關（Cockpit Main Switch）** 與 **[[driver-ergonomics-and-controls|煞車超行程開關（BOTS）]]** 組成，任一觸發皆須立即熄火 `[src: raw/FSAE_Rules_2027_V1.pdf, IC.9.1.1, p.90; IN.12.7, p.121]`。

> [!NOTE]
> **日本站（FSAEJ 2026）在地差異**：日本站僅提供 **RON 100 無鉛汽油**（`J2026-IC-02`，不提供 E85）；油箱須具備免電動泵浦排空機構（`J2026-IC-04`）；且 IC 車輛主斷電開關**必須為紅色，座艙內其他任何開關皆不得為紅色**（`J2026-IC-05`） `[src: raw/2026_FSAEJ_LocalRule_4th_20260616.pdf, p.7]`。

---
**相關頁面**：[[technical-inspection-gauntlet|噪音與開關測試（IN.12）]] · [[fsaej-local-rules-diff|日本站差異]] · [[glossary|術語表]]
