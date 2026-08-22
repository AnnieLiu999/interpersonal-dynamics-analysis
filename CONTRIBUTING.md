# 贡献指南 · Contributing

感谢你对本 Skill 感兴趣！欢迎通过 Issue 与 Pull Request 参与改进。

## 行为准则（Code of Conduct）

- 友善、就事论事，不针对个人。
- 不在任何讨论或提交中引入真实人物的隐私信息（姓名、聊天原文、精确地点等）。

## 如何贡献

1. **提 Issue**：发现方法论错误、报告模板 bug、表述不清，直接开 Issue 并描述复现步骤。
2. **提 Pull Request**：
   - Fork 本仓库后新建分支（建议 `feat/...`、`fix/...`）；
   - 改动尽量集中在 `SKILL.md` 或 `references/`；
   - 提交信息用祈使句，如 `fix: 修正双轴模型描述`、`feat: 增加澄清提问模板`；
   - PR 说明「改了什么 / 为什么」。

## 本地测试

将本仓库放入 WorkBuddy 的 skills 目录即可触发：

```bash
# 用户级
~/.workbuddy/skills/interpersonal-dynamics-analysis/

# 或项目级
{workspace}/.workbuddy/skills/interpersonal-dynamics-analysis/
```

放入后，在对话中表达分析意图（如"帮我分析这段聊天"），验证触发与 HTML 报告产出。

## Skill 结构约定

- **`SKILL.md`**：保持 YAML frontmatter（`name` / `description` / `agent_created`），正文为方法论与触发规则。
- **`references/`**：分析清单、报告模板等辅助文件；模板使用 `{{占位符}}` 表示生成报告时由 Skill 填充。
- 新增参考文件时，请在 `SKILL.md` 与 README 的「目录结构」中同步说明。

## 隐私红线（重要）

本 Skill 处理高度敏感的私人关系素材，**任何提交都不得包含**：

- 真实人名、昵称、聊天对话原文；
- 精确地点、机构名、可定位的独特事件；
- 绝对路径、个人邮箱、token / 密钥。

示例与占位符一律使用**虚构数据**。这一条是硬性要求，违反的 PR 将不会被合并。

## 许可

贡献即表示你同意以 [MIT License](LICENSE) 发布你的改动。
