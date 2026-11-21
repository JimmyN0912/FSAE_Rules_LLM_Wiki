# LLM Wiki Execution & Maintenance Log

> 真實記錄本專案從「先討論、後生成」到「原始檔錯誤攔截、重建 9 份官方 PDF 知識庫、自動化 Lint 驗證、以及 HTML 簡報編譯」的完整歷程。

---

## [2026-11-21 20:48] Phase 0 — 先討論、後生成（Scope Alignment）
- 與使用者討論後定案：
  - 主題：**Formula SAE 規則書知識庫（聚焦 IC 內燃機組）**，繁體中文。
  - 架構：Agent-driven LLM Wiki（`SCHEMA.md` + `raw/` + `wiki/` + 檢查迴圈 + 執行日誌）。
  - 交付：教學型單檔 HTML 簡報（專注新手教學，末頁附流程精簡版）+ 獨立 `REPORT.md`。

## [2026-11-21 20:51] Incident #1（關鍵錯誤攔截）— `raw/` 層汙染與假原始檔問題
- **發生錯誤**：初版執行時未取得真實官方 PDF，直接將網路搜尋彙整的二手摘要寫入 `raw/01-*.md ~ 06-*.md`。
- **造成的實際偏差**：
  1. 規則章節代碼過時（誤寫為 `A` / `DR`，漏掉 `VE`；2027 官方實為 `AD` / `PS` / `VE`）。
  2. 網路二手來源配分表算術錯誤（動態加總僅 625 分而非 675 分）。
  3. 完全漏掉 2027 年重大新制（簡報與成本共題 **Software-Defined Feature**）與日本站在地差異。
- **修正行動（Shift-Left 升級）**：
  - 使用者即時喊停，提供 **9 份真實官方 PDF** 置入 `raw/`。
  - 清空所有二手 `.md` 與舊版 `wiki/`，並在 `SCHEMA.md` 的 Loop A 最前端新增 **A0 原始檔完整性閘門（Primary Source Integrity Gate）** 與 **A1 版本/分站標記節點**。

## [2026-11-21 21:00] Loop A（v2）— 9 份真實官方 PDF 抽取與版本差異檢查（A0 → A1）
- 使用 `pypdf` 於臨時區（scratch）抽取全部 9 份 PDF 文字（合計 244 頁、492,000+ 字元），保持 `raw/` 完全不可變。
- **發現跨年度／跨分站衝突（於 A1 提前標記隔離）**：
  - 2027 全球規則允許汽油（20.0 mm）或 E85（19.0 mm），但 2026 日本站（`J2026-IC-02`）僅提供 RON 100 無鉛汽油。
  - 2027 全球設計簡報模板字體下限為 12 pt（建議 16+ pt），但 2026 日本站（`J2026-S-20`）嚴格規定 16 pt 下限，違者不予閱讀。

## [2026-11-21 21:04] Loop A（v2）— 編譯 8 頁知識庫（A2）
- 依 9 份官方 PDF 編譯並交叉連結 8 篇繁體中文知識頁 + `index.md`：
  - `rulebook-structure.md`、`chassis-and-passive-safety.md`、`driver-ergonomics-and-controls.md`、`ic-powertrain-rules.md`、`technical-inspection-gauntlet.md`、`competition-scoring-1000pts.md`、`2027-static-sdf-scenario.md`、`fsaej-local-rules-diff.md`、`glossary.md`。
- 下一步：執行 **A3 自動化 Wiki Lint 檢查**。

## [2026-11-21 21:05] Loop A（v2）— 自動化 Wiki Lint 驗證通過（A3 → A4）
- 執行 Python 自動化 Lint 腳本，檢查結果：
  - `raw/` 僅含 9 份真實官方 PDF（0 非法二手檔），且 **9/9 份 PDF 皆有被 Wiki 頁面引用**。
  - `wiki/` 共 9 篇知識頁（修正了 `index.md` 原先誤寫為 8 頁的 metadata 筆誤），**0 斷鏈、0 孤兒頁、0 缺 frontmatter、0 缺行內引用**。
  - 關鍵算術全數通過：`325 + 675 = 1,000`、`25+25+15+30+30+15+10 = 150`、`10+5+5 = 20`、`15+10+10+7+8 = 50`。

## [2026-11-21 21:08] Loop B — 教學型 HTML 簡報編譯與 QA 通過（B1 → B7）
- 依據 `wiki/index.md` 學習路徑與 9 頁知識庫編譯單檔離線簡報：`presentation/fsae-rulebook-101.html`（共 12 頁，含鍵盤導覽、側欄目錄、Percy SVG 示意圖、IC 車檢四關卡互動切換器、1,000 分互動配分圖）。
- **B6 自動化實測通過**：12 頁完整、0 外部 CDN 依賴、17 項關鍵規則數值全數吻合 Wiki、`node --check` JS 語法檢查 `rc=0`。
- 完成撰寫 `REPORT.md`（涵蓋步驟三 Loop/Graph 設計與步驟四真實反思）。
