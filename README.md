# SCU_TDK_Generator

> #### 專案目的：為電商商家建立 TDK 生成器，節省上架商品時花費的時間及人力成本

### 專案步驟
1. 運用 SEO 工具 **Ubersuggest** 獲得以「貝果」為主題之長尾關鍵字推薦清單，並將其爬取下來
2. 以長尾關鍵字為搜尋目標，爬取 Google Search SERP 前十頁搜尋結果分別的 `Title`, `Description`, `Link`, `Content`, `Page`, `Source`（Source 表示用來搜尋的 Keyword）
3. 將 Content 的內容進行 `CKIP Transformer` 斷詞處理
4. 進一步的分析文本詞彙關聯詞分析內容：
   - 關聯詞頻計算
   - TF-IDF 計算
   - 知識圖譜繪製(Gephi)
   - Word2Vec 關聯詞分類模型訓練
5. TDK 生成模型訓練：
   - Title：採用 GENIUS 模型作為 Title 的處理模組
   - Description：採用 GPT2 模型針對特定商品生成對應文本
   - Keyword：以 Keyword 分類模型結果推薦該類別 KEI 值前五名的關鍵詞
