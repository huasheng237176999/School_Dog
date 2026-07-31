# 學校周邊人犬衝突熱區分析展示平台

本資料包可直接上傳至 GitHub Pages 使用。

## 結構

```text
school_heat_county_recut_package_v5/
├─ index.html
├─ full_taiwan/
│  └─ png/
├─ county_final/
│  └─ png/
├─ all_png/
└─ tables/
   ├─ county_final_priority_summary.csv
   ├─ county_final_priority_class_area_long.csv
   ├─ county_final_priority_ranking.csv
   ├─ all_png_inventory.csv
   └─ county_image_match_check.csv
```

## 本版修正

- 使用縣市摘要資料作為統計卡、排名、縣市圖片的單一對應來源。
- 縣市圖片固定依 `COUNTYNAME` 對應至 `county_final/png/{縣市}_school_heat_priority_5class_within1000m.png`。
- HTML 內嵌一份由 CSV 轉換出的展示資料，避免 GitHub Pages 路徑或 CSV 讀取時序造成畫面不同步。
- CSV 仍保留於 `tables/`，供檢查與後續更新。
- 文字維持「關注／優先關注」語境。


## 本次修正說明

- 已將縣市統計、縣市排名、縣市圖片統一改用 `COUNTYNAME` 對應。
- 縣市圖片固定對應 `county_final/png/{COUNTYNAME}_school_heat_priority_5class_within1000m.png`。
- 網站前端已內嵌一份由 CSV 正規化後的資料，避免 GitHub Pages 讀取 CSV 時造成圖表不同步。
- `tables/county_image_match_check.csv` 可用於檢查每個縣市的圖片對應狀態。
