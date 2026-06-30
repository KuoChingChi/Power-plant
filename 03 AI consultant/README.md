# Workflow
<img width="869" height="456" alt="螢幕擷取畫面 2026-06-30 235324" src="https://github.com/user-attachments/assets/4bc94d96-cb4e-45f5-80d2-fa597bf3b3ba" />

### Step 01
- 將 `Precedent DNA產出結果` 作為 `AI consultant Gem（發電廠諮詢）` 的參考知識庫

### Step 02
- 與 `AI consultant Gem（發電廠諮詢）` 進行對答，它將分析使用者的設計需求求並給予參考案例推薦與設計建議
  
# 工具簡介

## AI consultant Gem（發電廠諮詢）：

> input：`Precedent DNA產出結果` （檔案位置：`precedent DNA_output data / DNA_01-23.json`）

> output：設計總結報告

- 工具使用連結：https://gemini.google.com/gem/1MIhjq5IW0feteMW8nw9uGj8RvqG0alcK?usp=sharing 
- 用途/目的：在傳統的建築設計或學術研究流程中，使用者在面對龐大的歷史與技術案例時，往往因缺乏結構化的提問思維，導致檢索結果流於表面。為解決此痛點，本系統揚棄了傳統「一問一答」的單向檢索模式，改採雙階段的「多輪引導與知識庫比對」機制。

### 應用機制：
### 1. 第一階段：多輪引導式問卷機制（獲取使用者設計需求）
     
  系統會透過動態的多輪問卷形式與使用者互動，逐步挖掘並精準獲取使用者在四個核心維度上的具體「設計需求」。

  <img width="929" height="537" alt="image" src="https://github.com/user-attachments/assets/ad56d8ad-cfa7-44e3-9a51-fc5f80bbdb95" />

### 2. 第二階段：案例知識庫比對機制（生成設計建議）
     
  將第一階段所產出的四維度設計需求，與後台內建的「案例知識庫」進行深度的比對與交叉分析。根據比對結果，系統將提煉出具備參考價值的洞察，最終「生成設計建議總結報告」。

  <img width="934" height="559" alt="image" src="https://github.com/user-attachments/assets/b54764e9-e93d-42af-9346-ea4fef992c7c" />

### 應用示範

<img width="1080" height="908" alt="image" src="https://github.com/user-attachments/assets/9953675d-943f-4226-b822-bce3411759c9" />

<img width="1080" height="930" alt="image" src="https://github.com/user-attachments/assets/2b6caabe-1c6b-4234-bde5-2eb960d379ba" />

