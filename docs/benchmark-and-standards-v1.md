# 对标项目与方法沉淀 v1

> 目标：把“前人已经做过的事”系统收进本项目，形成可执行的判断与处理标准。

## 1) 全网可借鉴的“同类/近邻”项目地图

### A. 公共治理与公共沟通（Plain Language）

1. **美国《Plain Writing Act of 2010》**  
   价值：把“清晰表达”上升到制度层面，要求政府对公众文件使用可理解表达。  
   启发：我们的项目可以明确“不是写作偏好，而是可理解性的公共责任”。

2. **Digital.gov Plain Language（美国联邦数字服务实践）**  
   价值：给出可操作定义：面向目标受众、第一次接触就能理解并行动。  
   启发：可直接作为本项目“可进入性”判据之一。

3. **GOV.UK Content Design / Writing for GOV.UK**  
   价值：把“plain English”落到细粒度规则（词、句、结构、链接、更新说明等）。  
   启发：我们可借鉴其“禁用模糊词、先说用户要做什么”的执行风格。

4. **European Commission: Clear writing for Europe**  
   价值：跨语言、跨机构推进“反官腔/反行话”写作。  
   启发：证明该方向不仅适用于英语，也适用于多语场景。

### B. 专业文档可控写作（Controlled Language）

5. **ASD-STE100 Simplified Technical English（STE）**  
   价值：通过规则+受控词汇减少歧义，服务高风险行业（航空/工程等）。  
   启发：本项目可借鉴“允许术语，但术语必须可控、可解释、可追溯”。

6. **ISO 24495 Plain Language 系列标准**  
   价值：把 plain language 进一步标准化（含组织实施层面）。  
   启发：本项目可从“个人写作技巧”升级到“流程标准+质量审计”。

### C. 可读性改写与文本简化研究

7. **Newsela Corpus（教育分级改写）**  
   价值：同一主题多难度版本，支持“降门槛但不改主题”的实践。  
   启发：可用于构建本项目示例库（同一原文，多档重写）。

8. **ASSET 数据集（多变换简化评测）**  
   价值：强调简化不是只换词，还包括拆句、压缩、重组等多种变换。  
   启发：我们应把“处理动作”显式化，而不是只做词汇替换。

9. **Simple English Wikipedia**  
   价值：长期运行的公共知识简化实践，强调常用词、可进入性。  
   启发：适合作为“知识白话”的长期社区化参照样本。

### D. 高风险信息判断（信息质量/误导）

10. **UNESCO MIL（Media and Information Literacy）框架**  
    价值：强调受众的验证能力、来源识别和批判性判断。  
    启发：本项目在“复述”之外，需增加“来源与证据可见性”层。

11. **CDC Clear Communication Index（公共卫生沟通）**  
    价值：把“清楚”拆成可打分条目，尤其适用于高风险内容。  
    启发：我们可以复制这种“条目化质控”的思路做项目评分表。

---

## 2) 如何定义“一段内容有问题”

建议将“问题内容”定义为：**在理解成本、信息真实性、逻辑完整性、行动可用性四个维度上存在显著缺陷的表达**。

### 2.1 四维判定（任一维度触发即可标记）

1. **可理解性问题（Understandability）**
   - 行话/抽象词堆叠，读者无法在首次阅读建立问题图景。
   - 句子过长且主谓不清，读者不知道“谁在做什么”。
   - 定义缺失：关键术语未解释。

2. **可验证性问题（Verifiability）**
   - 关键事实无来源、无数据、无时间范围。
   - 用“研究表明”“专家认为”但不给出处。
   - 混淆事实与判断。

3. **逻辑结构问题（Reasoning Integrity）**
   - 因果偷换：相关性当因果。
   - 条件丢失：把“在某条件下成立”改成“普遍成立”。
   - 结论超出证据边界。

4. **可执行性问题（Actionability）**
   - 读完后不知道该做什么/不该做什么。
   - 指令缺对象、缺步骤、缺约束（时间、范围、前提）。

### 2.2 红旗信号（快速筛查）

- 抽象名词密度高、动作动词密度低。
- 高频模糊词："某种"、"很多"、"显著"、"优化"、"赋能"（无量化支持）。
- 引用“权威”但缺原始链接。
- 情绪强度高于证据强度。

---

## 3) 处理规则：从“问题内容”到“合格输出”

## 3.1 七步处理流程（可直接落地）

1. **定位任务类型**：复述 / 解释 / 评价（先分层，避免混写）。
2. **抽取原子主张**：把原文拆成“谁-做什么-基于什么-得出什么”。
3. **证据对齐**：每条主张标注证据级别（原文明示/推断/无依据）。
4. **逻辑修复**：补齐条件、范围、不确定性；禁止擅自强化结论。
5. **语言去障碍**：术语→现象，名词→动作，长句→可验证短句。
6. **输出分层**：
   - A 忠实复述（仅原文可支持）
   - B 辅助解释（例子/类比，明确是解释）
   - C 个人判断（单独区块）
7. **质控回归**：用第 4 节标准打分，未达标则回到第 3~5 步。

### 3.2 允许与禁止

**允许**
- 为理解补充最小必要背景（且显式标注“解释层”）。
- 术语保留，但必须首现定义+现实对应。

**禁止**
- 在“忠实复述层”新增原文没有依据的新观点。
- 把“可能/部分/条件成立”改写为“必然/普遍/绝对成立”。
- 为了顺口删除关键限制条件。

---

## 4) 输出应符合的标准（验收标准 v1）

建议采用“硬门槛 + 评分项”。

### 4.1 硬门槛（必须全部满足）

1. **可回指**：关键句能回指到原文依据。  
2. **不越界**：复述不超出原文证据边界。  
3. **不失真**：核心问题、逻辑关系、语气边界未被改坏。  
4. **可进入**：非圈内读者可在首次阅读后说出“它在解释什么问题”。

### 4.2 评分项（每项 0-2 分，总分 10）

- **保真度**（0-2）：是否保持原问题与关键关系。
- **清晰度**（0-2）：是否主谓清楚、术语可懂。
- **证据可见性**（0-2）：关键断言是否有依据标注。
- **简洁性**（0-2）：是否无口水、无空话。
- **可用性**（0-2）：读者能否据此形成判断或行动。

**建议阈值**：
- 8-10：可发布
- 6-7：需修改
- ≤5：退回重做

---

## 5) 建议纳入本项目的新增工作包

1. **基准样例库**：同一原文，产出“忠实复述/辅助解释/批判拆解”三版。  
2. **问题内容标注集**：给每段标注问题类型（理解/验证/逻辑/执行）。  
3. **术语处置字典**：术语 -> 定义 -> 现实场景 -> 允许替代表达。  
4. **评分模板**：把 4.2 做成可复用 markdown 检查单。

---

## 6) 外部参考链接（第一批）

- U.S. Congress — Plain Writing Act of 2010: https://www.congress.gov/bill/111th-congress/house-bill/946/text
- Digital.gov — Plain language: https://digital.gov/topics/plain-language
- GOV.UK — Writing for GOV.UK: https://www.gov.uk/guidance/content-design/writing-for-gov-uk
- European Commission — Clear writing for Europe: https://commission.europa.eu/about/departments-and-executive-agencies/translation/clear-writing-europe_en
- ASD-STE100 (official): https://www.asd-ste100.org/about_STE.html
- ISO 24495 (catalog): https://www.iso.org/standard/78907.html
- ISO 24495-2 legal communication: https://www.iso.org/cms/%20render/live/en/sites/isoorg/contents/data/standard/08/57/85774.html
- Newsela Corpus Access: https://newsela.com/legal/data
- ASSET paper (arXiv): https://arxiv.org/abs/2005.00481
- Simple English Wikipedia: https://simple.wikipedia.org
- UNESCO MIL article hub (example): https://www.unesco.org/en/articles/media-and-information-literacy-first-line-defence-against-disinformation
- CDC Clear Communication Index: https://www.cdc.gov/ccindex/tool/index.html

