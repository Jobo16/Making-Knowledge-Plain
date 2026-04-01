# 深度研究作战手册 v1（持续扩展）

> 面向目标：你提出的三件事——
> 1) 继续全网搜集并吸收前人成果；
> 2) 严格定义“什么内容有问题”；
> 3) 把处理规则和输出标准做成可规模化执行的系统。

---

## 0. 本手册与现有文档的关系

- `principles.md`：价值与方向
- `rewriting-rules-v1.md`：基础转化规则
- `quality-checklist-v1.md`：通用质检
- `benchmark-and-standards-v1.md`：外部项目总览（第一批）
- **本手册**：把“研究-判断-处理-评测-迭代”变成长期流水线

---

## 1. 深度研究框架：从“找资料”升级为“可复用知识系统”

## 1.1 研究对象分层（Layered Research Objects）

### L1. 规范与制度层（Policy/Standards）

用于定义“清楚表达”的底线和公共责任。

- Plain Writing Act（美国）
- Plain Language 政府实践（Digital.gov、GOV.UK、EU）
- ISO 24495 系列标准
- ASD-STE100（高风险技术文档）

**作用**：给项目提供“应然边界”（应该达到什么）。

### L2. 方法与流程层（Methods/Workflows）

用于定义“怎么做”：拆解、重写、分层输出、复审。

- 受控语言方法
- 内容设计（content design）
- 风险沟通检查清单（如 CDC CCI）

**作用**：给项目提供“实操步骤”（具体怎么做）。

### L3. 评测与数据层（Evaluation/Data）

用于定义“怎么判断做得好不好”。

- 文本简化数据：Newsela、ASSET
- 自动指标：SARI、FKGL、可读性指标
- 人评框架：保真/清晰/有用/可验证

**作用**：给项目提供“证据闭环”（如何证明有效）。

### L4. 场景与风险层（Domain Risk）

用于定义“在哪里要更谨慎”。

- 公共卫生
- 法律/政策解释
- 教育普及
- 金融与投资传播

**作用**：按领域配置不同强度的规则（高风险场景要更严格）。

---

## 2. “有问题内容”本体（Problematic Content Ontology）

> 从“感觉这段话不行”升级为“可标注、可统计、可训练”的问题类型系统。

## 2.1 一级类型（P1-P8）

- **P1 进入障碍**：行话密度过高、定义缺失、句法负担过重。
- **P2 证据缺口**：关键断言无出处、无时间、无范围。
- **P3 逻辑断裂**：因果偷换、条件丢失、对比关系被抹平。
- **P4 语气越界**：可能说成必然、局部说成普遍。
- **P5 信息变形**：复述时新增未证实内容或删关键约束。
- **P6 结构失真**：原文“问题→机制→结论”骨架被改坏。
- **P7 口水化/鸡汤化**：信息密度下降、判断力度被磨平。
- **P8 不可执行**：读者无法据此形成判断或行动。

## 2.2 二级标注（示例）

- P1.a 术语未定义
- P1.b 抽象名词连发
- P2.a 数据无来源
- P2.b 过期事实未注明日期
- P3.a 相关性当因果
- P3.b 条件句丢失
- P4.a 概率词消失
- P5.a 忠实层混入个人解释
- P7.a 用情绪词替代机制解释

## 2.3 严重度分级（S0-S3）

- **S0**：无明显问题
- **S1**：轻微问题（局部可修）
- **S2**：中度问题（影响理解或判断）
- **S3**：重度问题（可能误导）

建议规则：
- 出现 P2/P3/P4 任一且为 S3 -> 直接退回重写。
- 高风险领域（医疗/法律/金融）出现 S2 即需二次复核。

---

## 3. 诊断流程：先“判病”，再“开方”

## 3.1 诊断问题树（Decision Tree）

1. 这段话的核心主张是什么？（一句话写出）
2. 主张是否可定位到原文证据？（能/不能）
3. 是否包含时间、范围、条件、对象？（全/缺）
4. 是否存在逻辑跳步？（无/有）
5. 是否对普通读者可进入？（是/否）
6. 是否能导向可执行理解？（是/否）

输出：`问题类型 + 严重度 + 处理策略编号`。

## 3.2 标注模板（可复制）

```md
- 原文片段：
- 主张ID：C-001
- 问题类型：P3.a（相关性当因果）
- 严重度：S2
- 证据状态：弱（缺对照/缺机制）
- 处理策略：R-LOGIC-02
- 修复后句子：
- 复核结果：通过/退回
```

---

## 4. 处理策略库（Rulebook）

> 不同问题类型，对应不同“修复动作”，避免“一把梭口语化”。

## 4.1 R-ACC（可进入性修复）

- **R-ACC-01 术语首现定义**：术语首次出现 = 术语 + 一句话定义 + 一个现实例子。
- **R-ACC-02 名词动词化**：把“抽象名词堆”改成“主体-动作-结果”。
- **R-ACC-03 长句拆分**：每句只保留一个主判断，附属条件单独列出。

## 4.2 R-EVD（证据可见性修复）

- **R-EVD-01 来源补全**：关键事实附来源或标注“待证据”。
- **R-EVD-02 时间戳显式化**：所有时效性事实加日期。
- **R-EVD-03 事实/判断分层**：事实先写，判断后写并标注。

## 4.3 R-LOGIC（逻辑修复）

- **R-LOGIC-01 关系词显式化**：因果/条件/转折必须明确连接词。
- **R-LOGIC-02 条件补回**：恢复“在何条件下成立”。
- **R-LOGIC-03 边界回收**：把超出证据范围的结论降级为“可能/倾向”。

## 4.4 R-TONE（语气边界修复）

- **R-TONE-01 概率词保护**：原文有“可能/部分/倾向”，复述必须保留。
- **R-TONE-02 禁绝对化**：禁止把条件结论写成绝对结论。

## 4.5 R-USE（可用性修复）

- **R-USE-01 给对象**：明确这段话对谁有用。
- **R-USE-02 给动作**：明确“应该做什么/不该做什么”。
- **R-USE-03 给限制**：说明适用范围与不适用边界。

---

## 5. 输出标准 2.0：从“好不好看”到“可审计”

## 5.1 三层输出协议（强制）

- **L-A 忠实复述层**：只允许原文可支持内容。
- **L-B 辅助解释层**：允许例子/类比，但必须标注“解释”。
- **L-C 评估判断层**：允许观点，但必须给出依据。

## 5.2 审计字段（每次输出必须附）

```yaml
task_type: faithful_rewrite | explanation | critique
domain_risk: low | medium | high
source_time: YYYY-MM-DD
claims_count: N
unsupported_claims: N
problem_tags: [P1.a, P3.b]
score:
  fidelity: 0-2
  clarity: 0-2
  evidence: 0-2
  concision: 0-2
  actionability: 0-2
release_decision: publish | revise | reject
```

## 5.3 发布门槛（建议）

- **必要条件**：硬门槛全过 + unsupported_claims = 0
- **分数条件**：总分 >= 8
- **高风险加严**：domain_risk=high 时 evidence 必须 = 2

---

## 6. 评测协议：人评 + 自动评测 + 反例回放

## 6.1 人评（主）

每条输出由 2 名评审独立打分：
- 保真度
- 可进入性
- 证据可见性
- 可用性
- 边界合规性

出现分歧 >=2 分：触发第三评审。

## 6.2 自动指标（辅）

用于趋势监控，不单独决定质量：
- 可读性指标（如 FKGL 等）
- 简化相关指标（如 SARI）
- 长度压缩比、术语密度变化

> 注意：自动分高不代表保真高，必须由人评兜底。

## 6.3 反例库（Hard Cases）

建立“最容易翻车”的样例池：
- 多重条件句
- 反事实推理
- 高术语密度段落
- 强价值判断段落

每次规则更新先跑反例库，回归不过不得发布。

---

## 7. 研究生产线（你要的“不要停”版本）

## 7.1 周期节奏（建议）

- **每日**：新增 3-5 条外部案例 + 1 条高质量改写样例
- **每周**：产出 1 份专题研究（一个领域）
- **每两周**：规则与评分表小版本升级
- **每月**：发布“问题分布与质量趋势”报告

## 7.2 持续采集清单（下阶段）

1. 法律/政策 plain language 实践
2. 医疗健康风险沟通标准
3. 教育分级改写数据
4. 科技传播中的术语治理方法
5. 自动评测指标与人评一致性研究

## 7.3 产出物标准化

每次新增研究必须包含：
- 来源链接（原始页面）
- 摘要（100-200 字）
- 可借鉴点（3 条）
- 对项目规则的影响（新增/修改/不变）

---

## 8. 下一步立即可执行任务（Backlog）

- [ ] 建立 `docs/case-library/`：先放 10 个“原文-三层输出-评分”样例
- [ ] 建立 `docs/problem-ontology-v1.yaml`：把 P1-P8 机器可读化
- [ ] 建立 `docs/review-template-v1.md`：统一审计字段
- [ ] 建立 `docs/hard-cases-v1.md`：首批反例 30 条
- [ ] 建立 `docs/research-log-2026Q2.md`：持续采集日志

---

## 9. 深度参考（新增批次）

- Plain Writing Act of 2010（U.S. Congress）: https://www.congress.gov/bill/111th-congress/house-bill/946/text
- Digital.gov Plain Language: https://digital.gov/topics/plain-language
- GOV.UK Writing for GOV.UK: https://www.gov.uk/guidance/content-design/writing-for-gov-uk
- EU Clear Writing: https://commission.europa.eu/about/departments-and-executive-agencies/translation/clear-writing-europe_en
- WHO Plain Language: https://www.who.int/about/communications/understandable/plain-language
- CDC Clear Communication Index: https://www.cdc.gov/ccindex/
- ASD-STE100: https://www.asd-ste100.org/about_STE.html
- ISO 24495 overview: https://www.iso.org/standard/78907.html
- Newsela data info: https://newsela.com/legal/data
- ASSET (arXiv): https://arxiv.org/abs/2005.00481
- SARI paper (ACL Anthology): https://aclanthology.org/Q16-1029/
- The (Un)Suitability of Automatic Evaluation Metrics for Text Simplification: https://direct.mit.edu/coli/article/47/4/861/106930/

