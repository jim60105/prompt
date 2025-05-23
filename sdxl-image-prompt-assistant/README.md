# SDXL Image Prompt Assistant

一個專門協助建立 SDXL (Stable Diffusion XL) Booru 標籤格式提示文字的 AI 助手，基於 Civitai 熱門提示文字而設計。

## Link

- [Coze Store](https://www.coze.com/s/Zs85vktXp/)

## 🎯 功能

- 將自然語言請求轉換為優化的 SDXL Booru 標籤格式提示文字
- 基於 Civitai 上的熱門提示文字來建立高品質內容
- 支援中文與英文的對話
- 提供提示文字的詳細解析與建議
- 包含初始提示、批判性分析、針對性優化、最終提示及說明的完整流程
- 支援正向及負向提示詞 (Positive/Negative Prompts)

## 💡 使用方式

1. 使用自然語言描述你想要生成的影像
2. 助手會:
   - 建立初始提示文字
   - 進行改善分析
   - 最佳化提示文字
   - 產生最終的 SDXL 提示文字
   - 提供詳細的解釋

## 🛠️ 系統指令

- `[Generate images with last prompt]` - 使用最後一個提示文字生成影像
- `[Update masterpiece reference materials]` - 更新參考資料庫

## 🎨 範例問題

- "A dog flying in the sky"
- "A logo for an assistant that can explore infinite possibilities of role-playing"
- "An asian girl walking on the street in black dress" 
- "Japanese anime girl with blonde twin-tails, v finger to eyes"

## ⚙️ 技術要點

- 使用 Booru 標籤格式作為提示文字基礎，專為 SDXL 模型最佳化
- 運用 JSON 格式進行 Chain-of-Thought 推理，提升輸出品質
- 整合 Civitai 熱門提示文字做為參考範本
- 自動針對使用者請求分解為核心視覺元素：主題、外觀、服裝、動作、情緒等
- 自動處理提示詞順序與優先排序，提高生成品質
- 利用知識庫中相關標籤進行精確匹配，確保提示文字有效性
- DeepSeek-R1 作為底層模型提供高品質回應
