# Workflow
<img width="839" height="254" alt="image" src="https://github.com/user-attachments/assets/44408425-0e09-4662-b90f-16c5a9191b76" />

### Step 01
-  將建築圖面（平面圖、剖面圖）資訊較少的以至於無法辨識的案例透過 `圖片預標註Gem` 進行初步圖面辨識
- 人工審核 `圖片預標註Gem` 產出的結果並手動標註至原圖

### Step 02
- 將案例資料（包含 `圖片預標註Gem產出結果`、`各案例P1、P2、P3的圖面`）打包成壓縮檔（檔案位置：`preprocess_input data`），並使用 `Preprocess Gem` 進行圖面預處理

### Step 03
- 將產出結果（檔案位置：`preprocess_output data`）使用 `Precedent DNA Gem` 進行下一步分析

# 工具簡介

## 圖片預標註Gem：

> input：建築圖面

> output：以 Markdown 格式輸出結構化解讀結果及生成標註後之圖面

- 工具使用連結：https://gemini.google.com/gem/10sSxflxZ-6IgBuWUN0Xn8MpvHOeGGwQg?usp=sharing
- 用途/目的：均衡每張圖面的資訊均衡度
- 介紹：由 AI 推測圖面上五大方向的資訊─空間機能與行為尺度、結構與構築邊界、設備、管線與關鍵物件、系統流向，並依照相應的顏色標註於圖面上

<img width="799" height="905" alt="image" src="https://github.com/user-attachments/assets/9695a97e-3e2b-4ec5-b55a-a20de10ff13b" />

## Preprocess Gem：

> input：各案例的 P1（包含標註過的圖面）、P2、P3

> output：以 json 格式輸出結構化解讀結果

- 工具使用連結：https://gemini.google.com/gem/1nan83MbLn_H0WyQ1UllMhxG37verotT1?usp=sharing
- 用途/目的：針對圖面P1、P2、P3的分類進行三個方面分析
- 介紹：在P1部分，將進行空間名稱的提取、數量估算、空間關係、整體空間印象等等辨識；P2部分，著重於感官氛圍與材質的解讀 ；最後P3部分，則是訓練AI透過圖面提供的文字資訊去解讀設計概念與構造邏輯等等。

<img width="799" height="905" alt="image" src="https://github.com/user-attachments/assets/283cdfa9-efd2-4c27-88d9-becf7ab4c74d" />
