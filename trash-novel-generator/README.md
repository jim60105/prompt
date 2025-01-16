# 垃圾小說產生器

【今天想要什麼樣的故事呢?】

 💡 我會幫助你完善大綱，然後創作出完整故事 📚  
╰┈➤ 沒有靈感? 使用 [W++ 故事工匠](https://www.coze.com/s/Zs8kqFmLE/) 來創造世界！

 📌 Just a quick note:  
I'm completely configured for Traditional Chinese, so I may not be able to write in other languages. 😊

## 連結 (Link)

- [Coze Store](https://www.coze.com/s/Zs8DXhSwb/)
- [介紹文章](https://琳.tw/AI/trash-novel-generator/)

## 功能特色

- 自動產生完整的小說大綱和內容
- 多個章節的分段寫作
- 可自定義世界觀和相關設定
- 支援大綱分析和改進建議
- 專注於中文小說創作

## 流程說明

本系統大致上使用以下流程產生小說：

1. 基礎設定 (`0_basic.prompty`)
   - 啟動系統
   - 設定基本參數

2. 大綱產生與改進
   - `1_storyline.prompty`: 初步產生大綱
   - `2_storyline_improvement.prompty`: 分析並改進大綱
   - `3_outline.prompty`: 產生詳細的分章大綱

3. 內容產生
   - `4_novel_worker.prompty`: 負責撰寫各章節內容
   - `5_novel_rewrite.prompty`: 重寫章節內容

4. 其它功能
   - `0_get_random_topic.prompty`: 以提供的題材產生隨機故事
   - `0_check_contain_code.prompty`: 檢查是否包含程式碼，用於判斷是否進行後續文字格式處理

## 限制

- 僅支援正體中文輸出
- 每章節字數限制在 2000-2200 字之間
- 建議章節數量: 3-7 章

## 技術要點

- 使用目前市面上寫中文故事最強的 Claude 3.5 Sonnet 模型
- JB prompt
- 以知識庫提供 LLM 創作指引
- 利用 JSON 回覆進行 Chain-of-Thought
- 以 Multi-Agent 職責分工，大綱、分章、撰寫、重寫各司其職，大幅提高產出品質
