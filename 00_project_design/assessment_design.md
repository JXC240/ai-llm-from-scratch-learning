# 前后测与每周小测设计

前测和后测采用同一能力框架，题型和难度保持一致。建议满分 100 分。

## 评分建议

| 题型 | 题号 | 分值 |
|---|---|---|
| 概念解释题 | 1-15 | 60 分 |
| 代码理解题 | 16-18 | 24 分 |
| 实验分析题 | 19-20 | 16 分 |

## 概念解释题

1. 什么是 tokenization？为什么 LLM 不能直接读取自然语言文本？
2. token、character、word 三种文本切分方式有什么区别？
3. embedding 的作用是什么？
4. token embedding 和 positional embedding 有什么区别？
5. 为什么 Transformer 需要位置信息？
6. self-attention 中 Q、K、V 分别代表什么？
7. attention score 的含义是什么？
8. softmax 在 attention 中起什么作用？
9. causal mask 为什么对 GPT 重要？
10. multi-head attention 为什么比 single-head attention 更强？
11. GPT block 通常包含哪些主要结构？
12. residual connection 和 layer normalization 的作用是什么？
13. pretraining 的目标是什么？
14. next-token prediction 为什么可以训练语言模型？
15. pretraining 和 finetuning 的区别是什么？

## 代码理解题

16. 给定一个 token id 序列，说明它如何经过 embedding 层变成模型输入。
17. 解释 attention 代码中 batch size、sequence length、embedding dimension 的含义。
18. 说明 logits、targets、cross-entropy loss 在训练循环中的关系。

## 实验分析题

19. 如果 loss 一直不下降，可能有哪些原因？如何验证？
20. 如果模型生成内容重复或无意义，可以从数据、模型、训练和采样哪些方面分析？

## 每周小测规则

每周小测包含：

- 3 道概念解释题。
- 1 道代码理解题。
- 1 道迁移或实验分析题。

答题流程：

1. 先独立作答。
2. 再让 AI 评分与追问。
3. 标出 AI 发现的盲区。
4. 重写最终答案。

