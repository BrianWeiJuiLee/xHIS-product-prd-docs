# xHIS Product PRD Docs

xHIS 產品 PRD 文件管理工作區，供 PM 團隊協作維護各模組的產品需求文件。

## 模組總覽

| 縮寫 | 模組名稱 | 資料夾 |
|------|----------|--------|
| OPD | 門診醫令 | [modules/opd](./modules/opd/) |
| ER | 急診醫令 | [modules/er](./modules/er/) |
| IPD | 住院醫令 | [modules/ipd](./modules/ipd/) |
| ERNIS | 急診護理 | [modules/ernis](./modules/ernis/) |
| IPDNIS | 住院護理 | [modules/ipdnis](./modules/ipdnis/) |
| APPT | 掛號系統 | [modules/appointment](./modules/appointment/) |
| PRICING | 批價系統 | [modules/pricing](./modules/pricing/) |
| REFERRAL | 轉診系統 | [modules/referral](./modules/referral/) |

## PRD 狀態流程

```
草稿 → 審查中 → 核准 → 開發中 → 已上線
```

## 快速開始

1. 確認負責模組，進入對應的 `modules/[module]/prds/` 資料夾
2. 複製 [PRD 模板](./_templates/prd-template.md)，依命名規則建立新檔案
3. 填寫 frontmatter 與文件內容，提交 Pull Request 進行審查

詳細規範請參閱：
- [命名規則](./_guidelines/naming-conventions.md)
- [工作流程](./_guidelines/workflow.md)
- [貢獻指南](./CONTRIBUTING.md)
