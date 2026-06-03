# 第 0 周第 1 天学习包：基线采集日

日期：2026-06-04

## 今日定位

今天不是正式学习 LLM 内容，而是建立“学习起点证据”。核心目标是让后续 8 周的学习变化可以被记录、被验证、被展示。

## 今日学习资料

### 视频课程

- 课程：Sebastian Raschka, *Build an LLM from Scratch*
- 第 1 节：Build an LLM from Scratch 1: Set up your code environment
- 链接：https://www.youtube.com/watch?v=yAcWnfsZhzo&list=PLTKMiZHVd_2IIEsoJrWACkIxLRdfMlw11

今天只需要确认课程入口和标题，不要在完成前测前正式观看课程内容。

### 官方代码仓库

- 仓库：rasbt/LLMs-from-scratch
- 链接：https://github.com/rasbt/LLMs-from-scratch
- 说明：官方仓库描述为“Implement a ChatGPT-like LLM in PyTorch from scratch, step by step”。

今天只需要确认仓库入口和目录结构，不要在完成前测前阅读具体代码。

## 今日必须完成的 5 件事

1. 独立完成前测：`01_baseline/pre_test.md`
2. 填写学习习惯基线：`01_baseline/learning_habit_baseline.md`
3. 填写基线代码解释：`01_baseline/baseline_code_explanation.md`
4. 完成初始知识图谱：`07_knowledge_maps/week0_initial_map.md`
5. 更新每日监督记录：`06_evidence_tables/daily_supervision_log.md`

## 建议时间安排

| 时间 | 任务 | 文件 |
|---|---|---|
| 10 分钟 | 打开课程和代码仓库，只确认入口，不深入学习 | 本文件 |
| 70 分钟 | 独立完成前测，不使用 AI | `01_baseline/pre_test.md` |
| 20 分钟 | 让 AI 评分与追问，记录盲区 | `01_baseline/pre_test.md` |
| 30 分钟 | 写学习习惯基线 | `01_baseline/learning_habit_baseline.md` |
| 25 分钟 | 修订初始知识图谱 | `07_knowledge_maps/week0_initial_map.md` |
| 20 分钟 | 完成基线代码解释 | `01_baseline/baseline_code_explanation.md` |
| 10 分钟 | 更新监督记录并提交 GitHub | `06_evidence_tables/daily_supervision_log.md` |

## 前测规则

- 先独立作答。
- 不看课程内容。
- 不搜索答案。
- 不问 AI 标准答案。
- 不追求高分，要真实暴露起点。
- 独立完成后，再让 AI 评分和追问。

## 今日可使用的 AI 提示词

### 前测评分

```text
我正在做 LLM from Scratch 学习项目的第 0 周前测。下面是我独立完成的答案。
请你只做评分和诊断，不要替我重写标准答案。
请按以下格式输出：
1. 总分估计
2. 每类题的薄弱点
3. 5 个最需要优先补的概念
4. 3 个追问问题
5. 不要直接给完整答案
```

### 学习习惯反思

```text
下面是我填写的学习习惯基线。请帮我识别其中最可能影响复杂技术学习的 3 个习惯问题。
不要替我写最终反思，只给我追问和改进方向。
```

### 初始知识图谱追问

```text
下面是我在正式学习前画的 LLM from Scratch 初始知识图谱。
请你指出图中缺失、混淆或连接不清楚的地方。
不要直接给完整知识图谱，只提出诊断性问题。
```

## 今日结束前自检

| 检查项 | 完成情况 |
|---|---|
| 前测已先独立完成 | 未完成 |
| AI 评分记录已写入前测文件 | 未完成 |
| 学习习惯基线已填写 | 未完成 |
| 初始知识图谱已更新 | 未完成 |
| 基线代码解释已完成 | 未完成 |
| 每日监督记录已更新 | 未完成 |
| 已提交并 push 到 GitHub | 未完成 |

## 今日向监督线程汇报格式

完成后在当前 Codex 线程发：

```text
第0周第1天完成汇报：
1. 前测完成：是/否，估计得分：
2. 最大盲区：
3. 今天 AI 介入次数：
4. 今天最重要的学习证据文件：
5. 是否已 push 到 GitHub：
6. 明天需要监督我重点做：
```

## 今日 Git 提交建议

```powershell
git status
git add 01_baseline 06_evidence_tables 07_knowledge_maps 02_learning_journey
git commit -m "Complete week 0 day 1 baseline evidence"
git push
```

