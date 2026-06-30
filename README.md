# 組員名單

蘇于庭 郭瀞淇 張嘉芸

# 案例主題

發電廠不同的發電方式如何影響建築不同層面

# Project overview

本專案以「發電廠不同的發電方式如何影響建築不同層面」為研究核心。基礎設施建築（如發電廠）過去多被視為純工業製程空間，本研究之重要性在於探討不同的發電機制（如火力、水力、生質能等），如何具體牽動並決定建築的基地回應、量體策略、空間規模、機能使用、材料使用，乃至於能源生產與副產物處理等多元設計層面。透過對多個發電廠案例的深度剖析，能將各別零散的廠房設計經驗，整合並轉化為具結構性的建築知識庫。此案例研究的核心價值，在於將知識庫介入至建築的「設計前期」。以不同的發電方式為前提，在尚未定案前即能提供設計者實質且具前瞻性的設計建議與策略指引。

# Workflow

<img alt="image" src="https://github.com/user-attachments/assets/8f98b92e-c403-4197-b97e-59ecc964a02d" />

## Step 01 Preprocess

這個階段可以再分為兩個階段的處理，先透過人工的圖面預標註，再透過本專案的「Preprocess Gem」進行預處理。第一階段人工預處理的目的為均衡每張圖面的資訊均衡度，先經由 AI 推測圖面上的資訊並依照相應的顏色標註於圖面上，再由人工比對網路上案例的相關資訊核對AI標註的結果是否屬實或合理並標註於原圖上，第二階段Preprocess預處理我們分別針對圖面P1、P2、P3的分類進行三個方面分析。

- input data : 案例原始圖面資料 `preprocess_input data`
- output data : `preprocess_output data`           

## Step 02 Precedent DNA

完成第一階段的知識萃取後，我們會將萃取結果以及案例的純文字資訊透過本專案的「Precedent DNA Gem」一起進行第二階段的分析處理。此階段的分析目的為回應我們一開始案例總覽的初步分析方向以及探討「不同發電方式」與建築各層面的關係。

- input data：`preprocess_output data` + 案例原始純文字資訊
- outpput data：`DNA_01-23.json`
  
## Step 03 AI consultant Gem（發電廠諮詢）

本專案研發之「AI consultant Gem（發電廠諮詢）」是一個具備高度自動化、動態互動能力及專業建築知識檢索的雙階段大語言模型諮詢系統，採雙階段的「多輪引導與知識庫比對」機制釐清使用者的設計需求，並比對知識庫內的案例給予適合的案例推薦與設計手法總整理。
- input data：`DNA_01-23.json` 作為案例知識庫來源

# 資料夾結構

`01 Preprocess` >

- `preprocess_input data`
- `preprocess_output data`
- `preprocess_prompt.md`
- `圖面預標註_prompt.md`

`02 Precedent DNA` > 

- `precedent DNA_input data`
- `precedent DNA_output data`
- `Precedent DNA_prompt.md`
- `輸出結果json格式.json`

`03 AI consultant` >

- `AI consultant_prompt.md`
- `發電廠諮詢小精靈(KB Tester)`

`Knowledge Base` >

- `DNA_01-23.json`

`案例資料` >

- `00 案例P1、P2、P3分類`
- `Case01-23原始圖片及文字資料`
