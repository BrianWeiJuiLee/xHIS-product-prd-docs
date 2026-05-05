# PRD 工作流程

## 狀態流程

```
草稿 → 審查中 → 核准 → 開發中 → 已上線
```

## 各狀態說明

### 草稿
- **觸發**：PM 開始撰寫新 PRD
- **作法**：建立新檔案，frontmatter `status: 草稿`，可開 Draft PR 讓團隊提早看見
- **完成條件**：文件內容足夠完整，可供 Reviewer 審查

### 審查中
- **觸發**：作者認為草稿完成，發起正式審查
- **作法**：更新 `status: 審查中`，將 Draft PR 轉為正式 PR，指定 Reviewer
- **完成條件**：Reviewer 完成審查並 approve

### 核准
- **觸發**：PR approved & merged
- **作法**：merge 後更新 `status: 核准`、`updated` 欄位
- **完成條件**：排入開發 backlog

### 開發中
- **觸發**：研發團隊開始實作
- **作法**：更新 `status: 開發中`、`updated` 欄位
- **完成條件**：功能開發完成並通過 QA

### 已上線
- **觸發**：功能正式上線
- **作法**：更新 `status: 已上線`、`updated` 欄位，並在修改紀錄補充上線版本號

## 棄用流程

若 PRD 因故取消或被取代：
1. 更新 `status: 已棄用`
2. 將檔案移至 `archive/` 資料夾
3. 在修改紀錄說明棄用原因

## Branch 策略

| 情境 | Branch 命名 |
|------|-------------|
| 新增 PRD | `feat/[MODULE-ID]-brief-description` |
| 更新既有 PRD | `update/[MODULE-ID]-brief-description` |
| 棄用文件 | `archive/[MODULE-ID]` |
