# FLUX.1 Image Prompt Assistant

一個專門協助建立 FLUX.1 影像生成提示文字的 AI 助手。

## Link

- [Coze Store](https://www.coze.com/s/Zs8D5GJk7/)

## 🎯 功能

- 將自然語言請求轉換為優化的 FLUX.1 影像生成提示文字
- 基於 Civitai 上的熱門影像提示文字來建立高品質內容
- 支援中文與英文的對話
- 提供影像生成提示文字的詳細解析

## 💡 使用方式

1. 使用自然語言描述你想要生成的影像
2. 助手會:
   - 建立初始提示文字
   - 進行改善分析
   - 最佳化提示文字
   - 產生最終的 FLUX.1 提示文字
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

- 使用 [Civitai](https://civitai.com/) RESTful API 來取得熱門提示文字做為範本
- 使用 txt2img tool 來生成影像
- 透過 JSON output 做 Chain-of-Thought，大幅提升輸出品質
