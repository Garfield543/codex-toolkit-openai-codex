# AI 入口：codex-toolkit-openai-codex

## 專案定位

本專案整理 OpenAI Codex 教學、工具與工作流程，服務對象為需要將 AI 工具導入教學與文件工作的使用者。

## 固定規則

- 使用繁體中文回覆與撰寫文件。
- 中文使用全形標點；英文與數字兩側保留半形空白。
- Windows 操作使用 PowerShell 語法，不使用 Bash 語法。
- HTML 必須符合響應式設計，支援電腦、平板與手機閱讀。
- 程式碼說明保持簡潔，避免冗長前言。
- 涉及檔案操作時，回報實際產出位置。
- 數學符號需考慮 Word 的 OMML 與 PowerPoint 的雙層文字框需求。
- 不將 API key、Cookie、權杖或其他秘密寫入 repository、文件或工作筆記。
- 不把每日流水帳寫入 `AGENTS.md`；進度與踩坑記錄放在 Obsidian 工作筆記。

## Obsidian 專案駕駛艙

- 工作筆記：`D:\secondbrain\codex-toolkit-openai-codex\工作筆記.md`
- 工作筆記記錄：目前進度、下一步、最近更動、工具驗證結果與踩坑筆記。
- 若該 Vault 路徑無法使用，先回報阻礙，不要自行改寫到不明位置。

## GitHub

- repository：[Garfield543/codex-toolkit-openai-codex](https://github.com/Garfield543/codex-toolkit-openai-codex)
- 可見性：公開（public）。
- 預定部署：GitHub Pages，網站來源為 `docs/`，部署 workflow 位於 `.github/workflows/pages.yml`。
- 只提交本專案相關變更；提交前先檢查 `git diff`。

## 開工規則

1. 先讀取 Obsidian 工作筆記；若不存在，再讀取專案根目錄 `handoff.md`。
2. 執行 `git status --short`，確認未提交變更後再工作。
3. 可執行 `git fetch` 檢查遠端，但不主動執行 `git pull`。
4. 依工作筆記的「下一步」接續，不覆蓋使用者既有檔案。

## 收工規則

1. 更新 Obsidian 工作筆記與必要的 `handoff.md`。
2. 檢查 `git diff`，只提交本次相關檔案。
3. 若已授權且遠端可用，才執行 commit 與 push。
4. 回報 Obsidian、`AGENTS.md` 與 GitHub 的同步結果及實際檔案位置。


