# 貢獻指南

## 建立新 PRD

1. 確認所屬模組與下一個可用的流水號
2. 從 `_templates/prd-template.md` 複製模板
3. 依命名規則 `[MODULE]-[ID]-[brief-description].md` 命名，存放於 `modules/[module]/prds/`
4. 填寫 frontmatter 欄位（`status` 預設為 `草稿`）
5. 撰寫文件內容後，建立 Pull Request

## Pull Request 規範

- **標題格式**：`[MODULE-ID] 功能簡述`（例：`[OPD-001] 醫令開立流程`）
- **草稿階段**：可開 Draft PR，方便早期討論
- **審查通過**：Reviewer approve 後，由作者 merge
- **狀態更新**：每次狀態變更（如「核准」→「開發中」）須更新 frontmatter 的 `status` 與 `updated` 欄位並 commit

## 狀態變更流程

| 狀態 | 負責人 | 說明 |
|------|--------|------|
| 草稿 | PRD 作者 | 初稿撰寫中 |
| 審查中 | PRD 作者 | 開 PR，指定 Reviewer |
| 核准 | Reviewer | PR approved & merged |
| 開發中 | PRD 作者 | 研發開始後更新 |
| 已上線 | PRD 作者 | 功能上線後更新 |

## 棄用文件

將文件移至 `archive/` 資料夾，並在 frontmatter 加上 `status: 已棄用`。
