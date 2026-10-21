# 安装及覆盖升级说明（v2.2）

这是对原 `social-science-writing-gate` 的**升级**，名称保持不变。文件夹已经具有 Codex 项目级 Skill 所需的结构。`references/` 是按需读取的补充指南，不会自动安装另外三个 GitHub 项目的全套 Skills。

## 推荐安装位置

项目级：

`/path/to/your/research-project/.agents/skills/social-science-writing-gate/`

推荐先备份原 Skill，再复制整个新文件夹（保留 `references/` 子目录）。示例在项目根目录终端执行，假设下载的ZIP已解压到 `~/Downloads/`：

```bash
cd '/path/to/your/research-project'
mkdir -p .agents/skills
if [ -d .agents/skills/social-science-writing-gate ]; then
  cp -a .agents/skills/social-science-writing-gate \
        ".agents/skills/social-science-writing-gate.backup.$(date +%Y%m%d-%H%M%S)"
fi
cp -R "$HOME/Downloads/social-science-writing-gate/." \
      .agents/skills/social-science-writing-gate/
```

**更稳妥办法**：先将压缩包解压到一个新目录；检查是否包含顶层 `social-science-writing-gate/SKILL.md`、三个 `references/*.md` 文件及 `REFERENCES_AND_SKILLS.md`，再复制整个文件夹。不要把压缩包内容直接散放在 `.agents/skills/` 根目录。

若你使用Codex的用户级目录，也可安装到 `~/.agents/skills/social-science-writing-gate/`，但**不建议同时维护不同版本的同名Skill**；以实际安装位置和Codex可发现的路径为准。通过ACP使用Cursor时，明确传递此项目级路径并要求Cursor读文件；不要以“Cursor能看到文件夹”推断它已经使用了Skill。

## 验证

在本机运行：

```bash
head -n 12 '.agents/skills/social-science-writing-gate/SKILL.md'
test -f '.agents/skills/social-science-writing-gate/references/economic-argument-guide.md' && echo 'Reference 1 OK'
test -f '.agents/skills/social-science-writing-gate/references/referee-and-source-checklist.md' && echo 'Reference 2 OK'
test -f '.agents/skills/social-science-writing-gate/REFERENCES_AND_SKILLS.md' && echo 'Inventory OK'
grep -n 'Mandatory claim-level mechanism citation gate' '.agents/skills/social-science-writing-gate/SKILL.md' 
```

然后在Codex对话输入：

> Read the project skill `social-science-writing-gate` and its economic interpretation requirements. Summarize the Economic Argument Matrix, the v2.1 claim-level mechanism citation rule (retained in v2.2) (normally 1–2 directly relevant studies per important judgment or 1–3 complementary studies per channel cluster), source-to-claim placement, and the separate scientific/economic/mechanism citation gates; do not enforce a mechanical citation quota. Do not modify the manuscript yet.

通过条件：它能提到经济现象、竞争机制及证据等级、现实含义、经济学解释的独立PASS/HOLD、仍保留七项Skills/JMU/两轮Anti-Defensive检查，而不是只说“写作风格良好”。

## 回退

关闭相关Codex/Cursor会话后，将备份目录内容恢复到 `.agents/skills/social-science-writing-gate/` 即可。备份属于本地文件，发布包中没有以前机器上的配置内容。

## 使用注意

- 本次只是文件包生成和供用户在Mac安装；未连接或修改本机Codex配置。
- 不会改变已有项目数据、论文或Codex–Cursor ACP配置。
- 对仅数据检索/数值审核的任务，无须强制做两遍反防御性写作。
- 严格审查经济机制不意味着强制重新计算或改变原研究结论。

## v2.2 additional verification

Ensure the agent can distinguish: (a) the paper's own Table/Figure-based findings, (b) externally supported economic mechanisms, (c) untested city-specific attribution. Ask it to explain how `MECHANISM_CITATION_HOLD` is triggered. The repository/package files have been validated here; **this does not confirm installation or actual skill discovery on your Mac**.


## v2.2 Results check

When updating from v2.1, keep the original directory and overwrite the seven existing files plus the new `references/results-economic-comparison-guide.md` after a backup. Confirm the new guide exists and that `SKILL.md` contains `Substantive Economic Magnitude and Comparison Gate`. Test by asking Codex to identify the most informative verified economic contrast in an approved Results table, calculate it with a source trail, and have Cursor independently check whether it is properly explained. The new quality sub-gate is `RESULTS_EXPOSITION: PASS/HOLD`. No existing Discussion gate is removed.