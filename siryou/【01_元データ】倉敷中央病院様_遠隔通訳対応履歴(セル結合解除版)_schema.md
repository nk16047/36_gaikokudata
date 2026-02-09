# Schema Report

Generated: 2026/02/09 11:18:22

## 【01_元データ】倉敷中央病院様_遠隔通訳対応履歴(セル結合解除版).xlsx
- File: `【01_元データ】倉敷中央病院様_遠隔通訳対応履歴(セル結合解除版).xlsx`
- Format: XLSX
- Header row: 1
- Data rows: 7
- Columns: 15

| No | Column | Type | MaxLen | Nullable | Unique | Formula |
|---:|:-------|:-----|-------:|:---------|-------:|:--------|
| 1 | 番号 | Number | 1 | No | 7 | No
| 2 | 入電日 | Date | 10 | No | 7 | No
| 3 | 入電時間 | Number | 17 | No | 7 | No
| 4 | 切電時間 | Number | 17 | No | 7 | No
| 5 | 対応時間 | Number | 20 | No | 7 | Yes (7件) `=CEILING((VALUE(TEXT(D2-C2,"h:mm:ss"))),"0:1:0")`
| 6 | 同一患者対応時間合計 | Number | 20 | No | 7 | Yes (7件) `=SUM(E2)`
| 7 | 通訳 方式 | String | 5 | No | 2 | No
| 8 | 担当科 | String | 5 | No | 6 | No
| 9 | 病院担当者名 | String | 6 | No | 7 | No
| 10 | 患者様氏名 | String | 14 | No | 6 | No
| 11 | 対応言語 | String | 7 | No | 4 | No
| 12 | 対応者 | String | 3 | No | 5 | No
| 13 | 通訳内容 | String | 238 | No | 7 | No
| 14 | 料金 | Number | 4 | No | 2 | No
| 15 | 備考 | Unknown | 0 | Yes | 0 | No

