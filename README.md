# SCU_TDK_Generator

> #### 專案目的：為電商商家建立 TDK 生成器，節省上架商品時花費的時間及人力成本

##
### 專題研究步驟
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

## 迷你黑客松結果呈現
> |   項目   |     說明    |   項目   |       連結        | 
> | :------: | :--------: | :--------: |   :---------:   |
> |   Ubersuggest 爬蟲    |  爬取長尾關鍵字推薦清單   |   程式碼   |   [🔗](https://github.com/peilichang/SCU_TDK_Generator/Ubersuggest_keyword.ipynb)    |
> |   Google Search SERP 爬蟲    |   爬取各關鍵字的前十頁搜尋結果    |   程式碼   |  [🔗](https://github.com/peilichang/SCU_TDK_Generator/Google_search_content.ipynb)     |
> |   CKIP 斷詞處理    |   將 Content 的內容進行斷詞    |   程式碼   |  [🔗](https://github.com/peilichang/SCU_TDK_Generator/CKIP.ipynb)     |
> |   PPT    |   專題發表時使用之簡報    |   簡報   |  [🔗](https://github.com/peilichang/SCU_TDK_Generator/111巨量資料專題實作成果簡報－TDK 生成器.pdf)|
> |   專題介紹   |   111-1 大四專題｜成果報告－TDK生成器    |   影片   |  [🔗](https://www.youtube.com/watch?v=SZv_pXkzJBU)|
