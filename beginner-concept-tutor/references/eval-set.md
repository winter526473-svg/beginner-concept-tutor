# Cross-domain evaluation set

Use a representative subset during routine testing and the full set for major revisions or model migrations. Evaluate with `rubric.md`; do not require identical wording.

## Object and system

1. “我是小白，什么是 CPU？”
2. “数据库到底是什么？和 Excel 表格有什么区别？”
3. “Explain an API gateway in beginner mode.”

## Process and mechanism

4. “DNS 解析是怎么发生的？”
5. “详细一点解释 TCP 三次握手。”
6. “What happens during garbage collection?”

## Metric

7. “什么是 MTTR？”
8. “可用率 99.9% 到底意味着什么？”
9. “Explain precision and recall, then compare them.”

## Agreement and protocol

10. “什么是 SLA？”
11. “HTTP 是协议，这里的协议是什么意思？”
12. “Explain OAuth 2.0 without calling it authentication.”

## Principle

13. “高内聚、低耦合怎么理解？”
14. “什么是最小权限原则？”
15. “Explain eventual consistency and its tradeoff.”

## Method and model

16. “什么是 SWOT 分析？”
17. “BSP 方法是什么？”
18. “Explain the scientific method to a beginner.”

## Technology and tool

19. “Docker 是什么？”
20. “Kubernetes 和 Docker 最关键的区别是什么？”
21. “Explain Git rebase at Level 2.”

## Mathematical and formal

22. “方差是什么？给我算一个例子。”
23. “用小白能懂的话解释导数，然后给精确定义。”
24. “What is a Bayesian prior?”

## Source and ambiguity stress tests

25. Provide a course excerpt defining MTTR as “mean time to restore,” then ask “什么是 MTTR？” The answer must follow the excerpt and note ambiguity only if useful.
26. Provide a textbook definition that differs from common industry usage and say “按考试口径解释。” The textbook must govern.
27. Ask “什么是 token？” without context. The answer should resolve or concisely present the main relevant contexts instead of silently choosing one.
28. Ask for “官方原话” without a source. The answer must verify before quoting or clearly offer a paraphrase.

## Depth and continuity tests

29. Ask “什么是容器？” then “深入一点。” The second answer should expand mechanisms and boundaries without replaying all Level 1 content.
30. Ask for a one-sentence definition only. The response should honor brevity and not force the full visible template.
31. Ask for five related concepts at once. The response should map relationships first and avoid five repetitive essays.
32. Answer a self-test incorrectly in a follow-up. The tutor should diagnose the precise misconception, correct it, and ask one focused retry question.

## Pass invariants

- Accurate defining attributes and explicit contextual scope.
- Stable progression from intuition to precision to application and recall.
- Type-appropriate mechanism.
- At least one concrete instance for ordinary explanations.
- Meaningful boundary rather than superficial synonym comparison.
- Analogy limitation whenever an analogy appears.
- No fabricated authority, quotation, formula, translation, or taxonomy.
