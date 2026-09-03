# College Resume Coach

面向大学生的 Codex 简历教练 Skill。它可以通过结构化访谈梳理真实经历，也可以根据已有简历和岗位 JD 生成针对性的中文简历。

## 主要能力

- 从零访谈并整理个人经历，交付可编辑的经历梳理文档
- 根据真实材料生成简历文字版，保留人工确认节点
- 根据岗位 JD 拆解要求、映射证据并生成定制简历
- 生成单文件、可编辑、可打印的 A4 HTML 简历
- 支持本地上传照片，不向网络传输图片
- 支持调整正文字号、行间距、段间距、加粗和斜体
- 在交付 HTML 前检查 A4 适配、溢出、遮挡、断页和页底留白

## 核心原则

本 Skill 只使用用户主动提供的事实。它可以重组和专业化表达，但不会虚构经历、职责、数字、奖项、证书或技能。缺失信息会明确标记为待补充。

## 安装

将仓库克隆到 Codex 的个人 Skills 目录：

```powershell
git clone https://github.com/sanjin666-eng/college-resume-coach.git "$env:USERPROFILE\.codex\skills\college-resume-coach"
```

如果目标目录已经存在，请先备份或更换目录名称，不要直接覆盖正在使用的版本。

## 使用示例

在 Codex 中调用：

```text
$college-resume-coach 帮我从零制作一份中文简历。
```

或者同时提供初版简历与完整岗位 JD：

```text
$college-resume-coach 请根据这份 JD 定制我的简历，所有内容必须基于我提供的真实经历。
```

## 工作流

1. 经历访谈与梳理
2. 简历文字版确认
3. 可编辑 A4 HTML 排版

岗位定制是独立入口：先输出 JD 匹配分析和定制文字版，用户确认后再生成 HTML。

## 目录结构

```text
college-resume-coach/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── html-resume.md
    ├── interview.md
    ├── jd-tailoring.md
    └── text-resume.md
```

## 隐私提示

请勿把真实简历、手机号、邮箱、证件照或其他个人资料提交到公开仓库。建议只提交 Skill 规则和完全虚构、彻底脱敏的示例。

## 许可证

本项目采用 [MIT License](LICENSE)。

