# 11/27進度紀錄

**簡筠方 Claire**
* 針對keyword對資料進行分析
* 流程:
  1.   檢視資料的基本結構與缺失情況，統計各欄NaN數量
  2.   統計 target 欄位的 0 和 1 的分布
  3.   統計 keyword 在資料中與按 target 分組中的分布，並計算每個 keyword 中屬於 target=1 的比例 target_1_ratio
  4.   將 keyword 的結果按 target_1 和 target_1_ratio 排序並繪製條形圖
  5.   將 keyword 欄位中的 %20 替換為空格並拆分成單字
  6.   將拆分後的 split_keywords 按 target_1 和 target_1_ratio 排序並繪製條形圖
  7.   計算train_data與test_data中keyword的交集與聯集，並計算出重疊率
* 困難:
  * keyword在train_data和test_data中都有資料缺失，無法進行分析
    * 我也不知道能怎麼辦
  * keyword總共有兩百多個，製成圖的話會變得很長
    * 或許可以只取前幾名，但這樣的話就看不出分布情況了?


---
**游婷安 Lulu**
* 做了什麼:

     1.將文字長度與 target 的關係分布視覺化
     2.統計前10常見的 keyword 及各自數量
     3.統計 keyword 與 target=1,target=0 的數量，輸出 target=1 前10高 keyword
     4.統計 keyword 與 target=1,target=0 的數量，輸出 target=0 前10高 keyword
     5.將前面資料做成圖表
     6.使用 sklearn 來預測 test.csv 結果
     7.計算準確性

* 困難:

    1.原先在 Colab 寫，後來改到 VS code上，發現他沒有 sklearn
    * 尚未解決
    
    2.大多都沒有學過也不知道從何開始
    * 參考Kaggle的初學者sklearn教學，以及ChatGPT輔助
    
    3.找不到更多元素和target有直接關係，導致無使預測更加準確
    * 尚未解決
---
**廖奕皓 Hao**
* 做了什麼:
    1. 先看train與test資料的一些基本資訊像是Missing Value、結構等
    2. 印出範例，了解disaster和nondisaster的差異
    3. 統計target0與1之分布比率
    4. 繪製出disaster和non-disaster的數量長條圖
    5. 繪製出前20常出現的keywords
    6. 繪製出前10常發言的人所在之地點
    7. 移除train與test中出現的URL和Punct
    8. 移除train與test中出現的stopwords
* 難處:
    一開始不知道要用114當kernel，耍白癡了一個小時...
    很常遇見no module的情況，原來pip install在終端機中沒用，要寫在程式碼裡面
    基本的功能都不會，所以要上網參考和學習加使用chatGPT
    
---
**陳芊羽 Eileen(lala)**
* 做了甚麼：
    1. 看了 [kaggle的解答程式碼](https://www.kaggle.com/code/philculliton/nlp-getting-started-tutorial/notebook) 的前半段(到使用RidgeClassifier)
    2. 看了 [十分基礎的pandas教學](https://simplelearn.tw/pandas-intro/#penci-%E7%AF%84%E4%BE%8B-12%EF%BC%9A%E8%AE%80%E5%8F%96-CSV-%E6%96%87%E4%BB%B6%E6%AA%94%E6%A1%88)
    3. 將pandas教學中的各個函式用在data上

* 難處：
    * 浪費了很多時間
        * 中間看了一些對這次目標沒有幫助的東西，像是kaggle那題程式碼的前半段，希望自己下次能改善
