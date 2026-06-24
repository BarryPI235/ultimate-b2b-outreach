# Ultimate B2B Outreach — WorkBuddy Agent Skill

<p align="center">
  <b>B2B 外贸客户开发全流程终极版</b><br>
  一个 Skill，覆盖从 <b>线索发现 → 联系人挖掘 → 精准触达</b> 的完整方法论
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0-blue" alt="version">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="license">
  <img src="https://img.shields.io/badge/lines-~2,400-orange" alt="lines">
  <img src="https://img.shields.io/badge/platform-WorkBuddy-purple" alt="platform">
</p>

---

## 目录

- [它能做什么](#它能做什么)
- [为什么是三合一](#为什么是三合一)
- [快速开始](#快速开始)
- [安装](#安装)
- [个性化配置](#个性化配置)
- [使用场景示例](#使用场景示例)
- [内容规模](#内容规模)
- [FAQ](#faq)
- [脱敏声明](#脱敏声明)
- [License](#license)

---

## 它能做什么

| 阶段 | 能力 | 核心产出 |
|:---:|------|------|
| 🔍 **Phase 1**<br>线索发现 | • 22 个 Google 搜索运算符（10 基础 + 12 高级）<br>• 搜索语法实战（公司背调 + 联系人开发组合拳）<br>• 17 种搜索策略（竞品反向、展会、招标、海关…）<br>• 分行业分国家搜索模板<br>• 非英语市场关键词矩阵（5 列 × 多语言）<br>• 五维量化评分矩阵 | 50+ 结构化<br>潜在客户线索 |
| ⛏️ **Phase 2**<br>联系人挖掘 | • 公司规模分叉路径（微型/中小/大企业）<br>• 官网 3 页必查（首页/联系/关于）<br>• 5 路并行搜索（Google + LinkedIn + 第三方 + 商业注册 + 人名）<br>• 4 路径人名发现（LinkedIn/注册库/口碑/招聘）<br>• MX 记录验证 + 邮箱格式推理引擎<br>• 多语言功能邮箱推理（11 种语言）<br>• 验证门禁 + 置信度体系 + 批量模式 | 每条线索 ≥10 个<br>触达方式 |
| ✉️ **Phase 3**<br>精准触达 | • 10 条定制提示词（P2-P12）<br>• **P7** 标准开发信模板（含变量体系）<br>• **P7-B** EDM 破冰策略（3 种切入模式）<br>• **P8** WhatsApp 开发话术<br>• **P9** 报价策略（含付款/交付话术）<br>• **P10** 售后跟进<br>• **P11** 跨行业组合策略<br>• **P12** 体量分层话术（小/中/大企业） | 回复率从 2%<br>提升至 15-30% |

---

## 为什么是三合一

传统方式需要三个独立 Skill 串联使用：`google-customer-dev`（搜索）→ `business-contact-miner`（挖掘）→ `client-outreach`（触达）。存在以下痛点：

| 痛点 | 三合一解决方案 |
|------|---------------|
| 跨 Skill 调用上下文丢失 | 单一 Skill，上下文贯穿全流程 |
| 需要在不同 Skill 间切换 | 一个对话完成搜索→挖掘→触达 |
| 重复的变量/配置 | 统一占位符，一次配置全局生效 |
| 安装三个 Skill 的维护成本 | 一个文件即插即用，零依赖 |

---

## 快速开始

在 WorkBuddy 中直接说：

```
"帮我在德国找 5 家 interactive flat panel 的经销商，找到他们的采购经理邮箱，然后写一封开发信"
```

Skill 会自动执行完整的 Pipeline：
1. **搜索**：用德语关键词在 `.de` 域名下组合搜索
2. **评分**：对每条线索五维打分，筛出 T1
3. **挖掘**：提取官网邮箱 + LinkedIn 决策人 + 推理邮箱
4. **触达**：基于调研数据写定制开发信

---

## 安装

```bash
# 克隆仓库
git clone https://github.com/YOUR_USERNAME/ultimate-b2b-outreach.git

# 复制到 WorkBuddy skills 目录
cp -r ultimate-b2b-outreach/ultimate-b2b-outreach ~/.workbuddy/skills/
```

或在 WorkBuddy 中通过 Skill 管理界面直接导入 `ultimate-b2b-outreach` 文件夹。

安装后重启 WorkBuddy，Skill 自动注册。在任何对话中使用触发词（如"开发客户""找客户""开发信"）即可激活。

---

## 个性化配置

安装后，在 `SKILL.md` 中全局搜索替换以下占位符，适配你的公司和产品：

| 占位符 | 替换为 | 示例 |
|--------|--------|------|
| `[Your Name]` | 你的姓名 | Barry Chen |
| `[Your Company]` | 你的公司名 | XX Technology |
| `[Company]` | 你的公司简称 | XX |
| `[company].com` | 你的域名 | XXX.com |
| `[Product Series]` | 你的产品系列名 | XX Series |
| `[Model]` | 你的产品型号 | XXX |
| `[Size]` | 你的产品尺寸 | 65"-110" |
| `[OS Name]` | 你的操作系统名 | XXX OS |
| `Brand A / Brand B / Brand C` | 你的主要竞品名 | ViewSonic / BenQ / MAXHUB |

> 💡 **提示**：用 VS Code 的「在文件中查找并替换」（`Ctrl+Shift+H`）一键批量替换。

---

## 使用场景示例

### 场景 1：开拓新市场

```
"帮我在波兰找 interactive flat panel 的进口商和经销商，
用波兰语搜索，优先找有 NIP 注册号的正式公司。"
```

### 场景 2：竞品客户转化

```
"我的竞品是 Brand A，帮我在德国找他们的客户案例，
反向挖出终端用户，评估是否可以转化。"
```

### 场景 3：EDM 死名单复活

```
"我有一个 200 人的 EDM 列表，超过 3 个月没人回复。
帮我生成一批破冰邮件，目标是触发对话而不是推销。"
```

### 场景 4：大客户专项开发

```
"这是一家中东的大型系统集成商，200+ 员工。
帮我做深度背调，找到采购总监，然后写一封匹配大企业体量的开发信。"
```

---

## 内容规模

| 模块 | 内容量 |
|------|--------|
| 总规模 | ~2,400 行 · ~100 KB |
| Part A — 线索发现 | 22 个搜索运算符 + 17 种策略 + 行业模板 + 关键词矩阵 |
| Part B — 联系人挖掘 | 4 路径发现 + 5 路搜索 + 11 语言功能邮箱推理 + 批量模式 |
| Part C — 精准触达 | 12 个提示词模板 + 3 种破冰策略 + 体量分层系统 |
| 附录 | 统一自检清单 + 多语言关键词速查 + 工具推荐 |

---

## FAQ

<details>
<summary><b>Q: 这个 Skill 需要联网吗？</b></summary>
部分功能（Google 搜索、LinkedIn、MX 记录查询）需要 AI Agent 有网络访问权限。纯方法论部分（开发信模板、评分矩阵）可离线使用。
</details>

<details>
<summary><b>Q: 支持哪些市场？</b></summary>
全球 50+ 国家/地区。覆盖欧洲（德法意西波兰捷克匈牙利…）、中东（阿联酋沙特）、东南亚、南亚、拉美、非洲。各国域名后缀、公司后缀、邮箱后缀均已内置。
</details>

<details>
<summary><b>Q: 和 ChatGPT 写开发信有什么不同？</b></summary>
本 Skill 不是简单的"帮我写一封开发信"提示词。它包含完整的上下文链路：搜索语法 → 线索评分 → 联系人验证 → 基于调研数据定制的开发信。ChatGPT 不知道你的客户是谁，本 Skill 强迫你先调研再动笔。
</details>

<details>
<summary><b>Q: 可以只用其中一部分吗？</b></summary>
可以。三个 Phase 各自独立，直接说"用 Phase 2 的方法帮我挖这个公司的联系人"即可只激活对应部分。
</details>

<details>
<summary><b>Q: 如何贡献或反馈？</b></summary>
欢迎提交 Issue 或 PR。如果你有新的搜索策略、行业模板、触达话术想加入，直接提 PR 到 Phase 对应章节。
</details>

---

## 方法论来源

本 Skill 由三个专业模块合并而成：

1. **Google 客户开发** — 搜索运算符系统 + 搜索语法实战 + 量化评分矩阵 + 分流门禁
2. **联系人挖掘器** — 邮箱推理引擎 + 决策人定位 + 验证门禁 + 批量处理
3. **开发信工具箱** — 定制开发信 + EDM 破冰（3 策略）+ WhatsApp + 报价 + 体量分层

三合一消除了跨 Skill 依赖，单文件即插即用。方法论框架和策略逻辑完整保留。

> 🔗 如果你只需要独立模块，可以从 [Releases](https://github.com/YOUR_USERNAME/ultimate-b2b-outreach/releases) 中下载拆分的独立版。

---

## 脱敏声明

本版本为公开发布版本。所有真实企业名称、品牌名、产品型号、个人信息均已替换为通用占位符（`[Your Name]`、`[Your Company]`、`Brand A/B/C` 等）。方法论框架和策略逻辑完整保留，不影响实际使用效果。

---

## License

MIT — 自由使用、修改、分发。署名感谢但不强制。

---

<p align="center">
  <sub>Made for B2B外贸人 · Powered by WorkBuddy AI Agent</sub>
</p>
