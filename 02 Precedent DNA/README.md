# Workflow
<img width="821" height="333" alt="螢幕擷取畫面 2026-06-30 232913" src="https://github.com/user-attachments/assets/68d71d55-e760-4ccf-8ae3-bac7e1a7ab8a" />

### Step 01
- 將 `Preprocess Gem 產出結果` 以及 `案例純文字資料` 打包成壓縮檔，並使用 `Precedent DNA` 進行分析

### Step 02
- 將產出結果作為 `AI consultant Gem（發電廠諮詢` 的知識庫使用，並進行下一步應用

# 工具簡介

## Precedent DNA Gem：

> input：`Preprocess Gem 產出結果` + `案例純文字資料` 的壓縮檔（檔案位置：`precedent DNA_input data`）

> output：以 json 格式輸出結構化解讀結果（檔案位置：`precedent DNA_output data`）

- 工具使用連結：https://gemini.google.com/gem/10sSxflxZ-6IgBuWUN0Xn8MpvHOeGGwQg?usp=sharing 
- 用途/目的：回應我們一開始案例總覽的初步分析方向以及探討「不同發電方式」與建築各層面的關係
- 分析架構：這套架構分為三個層次。
    - Layer01：建築物的基本資料，此Layer之下可再分為六大領域
    - Layer02：將第一層的相對客觀的分析結果進行複合的關聯式分析
    - Layer03：郵遞二層的結果推導進到設計層面的回應。

### 分析架構圖
<img width="2662" height="1825" alt="發電廠發電方式如何影響建築各層面 (4)" src="https://github.com/user-attachments/assets/23e2f7e4-8e85-4808-9720-dc779e73c18b" />

### 發電廠建築類型Ontology

<img width="4030" height="2062" alt="發電廠發電方式如何影響建築各層面 (6)" src="https://github.com/user-attachments/assets/7bdbcfa7-8cd0-46fe-b2a6-01e35112a753" />

