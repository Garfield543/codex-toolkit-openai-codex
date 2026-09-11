# codex-toolkit-openai-codex

整理 OpenAI Codex 教學、工具與工作流程的繁體中文懶人包，提供可重複使用的操作說明、專案規範與教學資源。

## 專案目標

- 整理 Codex 的基本操作、工作流程與常見設定。
- 累積適合教學與日常工作的工具評估、使用範例與踩坑筆記。
- 透過 GitHub Pages 發布容易閱讀的公開文件入口。

## 目前結構

```text
.
├── .github/workflows/pages.yml  # GitHub Pages 部署流程
├── docs/index.html               # GitHub Pages 首頁
├── AGENTS.md                     # AI 協作入口與固定規則
├── README.md                     # 專案說明
└── .gitignore                    # 忽略規則
```

## 本機預覽

在 PowerShell 執行：

```powershell
py -m http.server 8000 --directory docs
```

接著開啟 <http://localhost:8000>。

## GitHub Pages

推送至 `main` 分支後，`.github/workflows/pages.yml` 會將 `docs/` 發布到 GitHub Pages。首次部署時，請在 GitHub repository 的 **Settings → Pages** 確認來源使用 **GitHub Actions**。

私有 repository 的 Pages 是否可用，仍取決於 GitHub 帳號或組織方案；若方案不支援，GitHub Actions 會在部署階段回報原因。

## 協作規則

請先閱讀 [AGENTS.md](AGENTS.md)。進度紀錄放在 Obsidian 專案工作筆記，不把每日流水帳寫入 `AGENTS.md`。
