# 前测 AI 诊断记录

日期：2026-06-04

## 诊断原则

本诊断只用于记录学习起点，不用于评价能力高低。前测阶段的目标是暴露真实盲区，因此“不知道”“不确定”“我猜”都是有效证据。

## 总分估计

建议记录为：**9 / 100**

这个分数不是失败，而是非常清晰的基线。它说明你当前处于“听过部分术语，但尚未建立系统理解和代码解释能力”的状态。

## 分项判断

| 类别 | 题号 | 满分 | 估计得分 | 诊断 |
|---|---|---:|---:|---|
| 概念解释题 | 1-15 | 60 | 9 | 能识别少量术语，如 Q/K/V、next-token prediction、pretraining/finetuning 的中文含义，但大多数概念还没有形成可解释结构。 |
| 代码理解题 | 16-18 | 24 | 0 | 暂时无法解释 token ids、embedding、attention shape、logits、targets、loss 的代码关系。 |
| 实验分析题 | 19-20 | 16 | 0 | 暂时无法从数据、模型、训练、采样角度分析 loss 和生成质量。 |
| 总计 | 1-20 | 100 | 9 | 适合作为第 0 周基线。 |

## 当前最大盲区

1. **文本如何进入模型**：tokenization、token id、embedding 之间的关系还不清楚。
2. **Transformer 为什么需要位置信息**：token embedding 和 positional embedding 尚未区分。
3. **attention 的计算机制**：虽然知道 Q/K/V 的英文，但还不能解释它们如何产生 attention score。
4. **causal mask 与 GPT 生成逻辑**：还不知道为什么 GPT 不能看未来 token。
5. **训练循环的关键对象**：logits、targets、cross-entropy loss 的关系还没有建立。
6. **实验诊断能力**：loss 不下降、生成重复等问题还无法拆解原因。

## 已经有的起点优势

- 你没有假装自己懂，而是诚实写了“不知道”和“我猜”，这对诊断式学习非常重要。
- 你已经知道 Q/K/V 分别是 query、key、value，这是后面学习 attention 的切入口。
- 你能猜到 next-token prediction 与预测下一个 token 有关，这是理解 pretraining 的入口。
- 你知道 pretraining 与 finetuning 是两个不同阶段，虽然目前只停留在中文翻译层面。

## AI 追问问题

这些问题不要现在查答案，等第 2-6 周学习对应主题时再回头回答。

1. 如果一句话先被 tokenizer 变成 token ids，为什么 embedding 层不能直接接收原始文字？
2. 如果 self-attention 只看 token embedding 而没有 positional embedding，模型会丢失什么信息？
3. Q、K、V 都来自同一个输入，为什么还要分成三个不同向量？
4. 如果 GPT 在训练时能看到未来 token，会发生什么问题？
5. loss 不下降时，怎样区分是数据问题、模型问题、训练循环问题还是学习率问题？

## 后续学习优先级

| 优先级 | 主题 | 对应周次 |
|---|---|---|
| 1 | tokenization -> token ids -> embedding | 第 2-3 周 |
| 2 | tensor shape 与 batch/sequence/embedding 维度 | 第 3 周 |
| 3 | Q/K/V、attention score、softmax、causal mask | 第 4 周 |
| 4 | GPT block 结构与 residual/layer norm | 第 5 周 |
| 5 | logits、targets、loss、next-token prediction | 第 6 周 |
| 6 | generation、sampling、重复输出分析 | 第 7 周 |

## 记录结论

这是一个有效的前测基线。后续 8 周的目标不是把这些题背成标准答案，而是逐步做到：

- 能用自己的话解释。
- 能联系代码输入输出。
- 能通过实验验证。
- 能识别 AI 解释中的错误或不完整之处。

