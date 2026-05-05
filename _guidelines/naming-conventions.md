# 命名規則

## PRD 檔案命名

格式：`[MODULE]-[ID]-[brief-description].md`

- **MODULE**：模組縮寫（大寫），見下表
- **ID**：三位數流水號，從 `001` 開始，每個模組獨立計算
- **brief-description**：功能簡述，使用小寫 kebab-case（英文單字以 `-` 連接）

### 範例

```
OPD-001-medication-order-flow.md
ER-001-triage-order.md
IPD-001-admission-order.md
ERNIS-001-nursing-assessment.md
IPDNIS-001-care-plan.md
APPT-001-online-booking.md
PRICING-001-fee-calculation.md
REFERRAL-001-outbound-referral.md
```

## 模組縮寫對照

| 縮寫 | 模組名稱 | 資料夾 |
|------|----------|--------|
| OPD | 門診醫令 | modules/opd |
| ER | 急診醫令 | modules/er |
| IPD | 住院醫令 | modules/ipd |
| ERNIS | 急診護理 | modules/ernis |
| IPDNIS | 住院護理 | modules/ipdnis |
| APPT | 掛號系統 | modules/appointment |
| PRICING | 批價系統 | modules/pricing |
| REFERRAL | 轉診系統 | modules/referral |

## Frontmatter `id` 欄位

與檔名前綴一致，例如檔名 `OPD-001-medication-order-flow.md` 對應 `id: OPD-001`。

## 流水號規則

- 每個模組從 `001` 獨立計算，不跨模組共用
- 已刪除或棄用的編號**不重複使用**
- 如需確認下一個可用號碼，查看該模組 `prds/` 資料夾內的現有檔案
