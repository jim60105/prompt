# Automated Prompt Engineering

此工具實作了 Google DeepMind 論文中提出的 OPRO 策略，使用大型語言模型作為優化器來改進提示詞。透過反覆疊代和評估，它能自動找出最有效的提示詞組合。

## 連結

- [Coze Store](https://www.coze.com/s/Zs8DgSDKN/)
- [Blog Post](https://琳.tw/AI/automated-prompt-engineering/)

## 什麼是 Automated Prompt Engineering？

**Automated Prompt Engineering (自動化提示詞工程，簡稱 APE) 旨在自動化大型語言模型 (LLM) 提示詞的生成和優化過程。**

在傳統的 Prompt Engineering 中，開發者需要手動設計、測試和優化提示詞，這是一個耗時且常常需要反覆嘗試的過程。APE 的目的就是要簡化並加速這個過程，讓 AI 系統能夠自動找出最有效的提示詞。

**APE 的核心原理是利用不斷疊代來優化 AI**。它通過以下步驟來實現自動化：

1. 初始化：設定任務目標和初始提示詞。
2. 生成回應：使用當前提示詞讓 LLM 生成回應。
3. 評估效果：分析生成的回應，評估其品質和相關性。
4. 優化提示詞：基於評估結果，自動調整和改進提示詞。
5. 疊代：重複上述過程，直到達到滿意的結果。

在 APE 的實踐中，Optimization by PROmpting (以大型語言模型做為優化器，OPRO) 是一種很好的提示詞優化方法。OPRO 策略來自 Google DeepMind 的論文《[Large Language Models as Optimizers](https://arxiv.org/pdf/2309.03409)》，**通過 LLM 分析先前疊代的結果並識別成功模式，從而優化提示詞。**

在這篇部落格中我僅簡短的提及它的工作原理，若讀者對 APE 技術和 OPRO 流程感興趣，我強烈推薦閱讀下面這篇非常精彩的文章。這篇文章詳細講解了 APE 和 OPRO 流程，對理解本助手的運作原理非常有幫助。

> 自動提示詞工程解放LLM潛力，APE讓LLM探索更廣闊的提示詞設計空間 | T客邦
>
> ---
> [https://www.techbang.com/posts/118175-auto-prompt-engineering-guide](https://www.techbang.com/posts/118175-auto-prompt-engineering-guide)

## 提示詞

- **Basic Runner** (`0_basic.prompty`): 初始設定和基礎執行器
- **Target Generator** (`1_target.prompty`): 生成目標提示詞
- **Evaluator** (`2_evaluator.prompty`): 評估提示詞效果
- **Optimizer** (`3_optimizer.prompty`): 優化提示詞

## 相關工具

- [Simple Prompt Maker](simple-prompt-maker/): 用於產生初始提示詞
- [Scoring Criteria Maker](scoring-criteria-maker/): 用於產生評分標準
