# 組員名單
蘇于庭 郭瀞淇 張嘉芸
# 案例主題
發電廠不同的發電方式如何影響建築不同層面
# 資料夾結構
01 Preprocess >

02 Precedent DNA > 

03 AI consultant >

Knowledge Base > 

案例資料 > P1圖面 (Drawings)/P2照片-渲染圖 (Photos-Renders)/P3概念-構造圖 (Diagrams-Details)/純文字資料
# Project overview
本專案以「發電廠不同的發電方式如何影響建築不同層面」為研究核心。基礎設施建築（如發電廠）過去多被視為純工業製程空間，本研究之重要性在於探討不同的發電機制（如火力、水力、生質能等），如何具體牽動並決定建築的基地回應、量體策略、空間規模、機能使用、材料使用，乃至於能源生產與副產物處理等多元設計層面。透過對多個發電廠案例的深度剖析，能將各別零散的廠房設計經驗，整合並轉化為具結構性的建築知識庫。此案例研究的核心價值，在於將知識庫介入至建築的「設計前期」。以不同的發電方式為前提，在尚未定案前即能提供設計者實質且具前瞻性的設計建議與策略指引。

# Workflow
<img width="394" height="205" alt="image" src="https://github.com/user-attachments/assets/8f98b92e-c403-4197-b97e-59ecc964a02d" />

## Step 01 Preprocess
這個階段可以再分為兩個階段的處理，先透過人工的圖面預標註，再透過本專案的「Preprocess小精靈」進行預處理。第一階段人工預處理的目的為均衡每張圖面的資訊均衡度，先經由 AI 推測圖面上的資訊並依照相應的顏色標註於圖面上，再由人工比對網路上案例的相關資訊核對AI標註的結果是否屬實或合理並標註於原圖上，第二階段Preprocess預處理我們分別針對圖面P1、P2、P3的分類進行三個方面分析。
- input data：案例原始圖面資料
- output data：json檔
## Step 02 Precedent DNA
完成第一階段的知識萃取後，我們會將萃取結果以及案例的純文字資訊透過本專案的「Precedent DNA小精靈」一起進行第二階段的分析處理。此階段的分析目的為回應我們一開始案例總覽的初步分析方向以及探討「不同發電方式」與建築各層面的關係。
- input data：preprocess json檔 + 案例原始純文字資訊
- outpput data：json檔
## Step 03 AI consultant（發電廠諮詢小精靈）
本專案研發之「發電廠結構小精靈」是一個具備高度自動化、動態互動能力及專業建築知識檢索的雙階段大語言模型諮詢系統。
- input data：precedent DNA json檔 作為案例知識庫來源

## Layer01基本資料
### Building
* form
  * massing strategy
  * orientation
  * environmental response
    * lighting strategy
    * ventilation strategy
* material
  * primary tectonic material
  * interior finishes
  * performance \& lifecycle
* space
  * spatial organization
    * spatial hierarchy
    * spatial sequence
  * circulation
  * spatial boundaries and connectivity
* facade
  * materiality \& texture
  * fenestration \& transparency
  * tectonic detailing
* scale
  * physical dimensions
  * human scale relationship
  * urban proportion
* program
  * functional zoning
  * spatial hierarchy
  * occupancy type
* structure \& construction
  * structure system
  * enclosure system
  * construction method
### Energy production
* generation type
* power capacity
* energy source
* output type
* byproduct management
### Event
* status
* completion
* renovation
### Site
* context:探討基地與其所在大環境之間的關聯
  * natural context:描述基地座落於何種地貌地形（如：山谷、水岸、平原、坡地）,以及該處原有的生態、植被與水文狀態為何。
  * historical context:描述這塊土地過去的用途或發展過程，周邊是否遺留歷史建築、古蹟遺址，或是保留了舊有城鎮的街道格局與空間尺度。
  * cultural context:聚焦於基地所在地區的人文社會氛圍與無形資產，描述當地的宗教信仰、傳統習俗或日常社區活動等
* landscape:描述周邊既有建物的立面質感、色彩與量體尺度，街道空間的鋪面材質與物件（如：街道家具、照明）配置，基地內外的植栽特性（樹種、植被）、水景設計，以及站在基地中向外望去的視野（View）、軸線、天際線與整體的空間氛圍等。
### Participant
* architect
* user
* client
* co-working designer
* consultant
### Sustainability
* carbon footprint
* circular economy
* ecological impact
## Layer02 複合分析
* Energy production+Site
* Energy production+Building
* Energy production+Sustainability
* Energy production+Participant
## Layer03反映在設計哪些方面
* 量體策略
* 材料回應
* 立面特徵
* 剖面特徵
* 副產物的利用
* 材料回應
* 複合program
* 動線規劃
# 其他
