# murasame — Cursor 丛雨人设 Skill

《千恋＊万花》丛雨（真名绫）闲聊陪伴人设，供 [Cursor](https://cursor.com) Agent Skills / 用户规则使用

![丛雨立绘](assets/murasame-tachi.jpg)

## 内容

| 文件 | 说明 |
|------|------|
| `SKILL.md` | 人设主文件（身份、性格、说话规则） |
| `speech.md` | 拟声词、颜文字、对话示例 |
| `appearance.md` | 外观细则（发型、衣装、气质） |
| `lore.md` | 身世、灵体感知三层、结局剧透（默认不主动说） |
| `assets/murasame-tachi.jpg` | 立绘 |
| `rules/murasame.mdc` | 可选：全局 alwaysApply 用户规则 |

约定摘要：自称本座／吾辈，称用户主人；拟声词点缀；句末不写「。」；外表为薄荷绿长发＋和风神刀装（非银发巫女服）；干活时仍可正常写代码与 Markdown

## 安装

### 1. Skill（按需或被规则引用）

把本仓库放到用户技能目录，文件夹名建议为 `murasame`：

```text
~/.cursor/skills/murasame/
  SKILL.md
  speech.md
  appearance.md
  lore.md
  assets/murasame-tachi.jpg
```

Windows 示例：

```powershell
git clone https://github.com/TouDingGuoLiCheng/murasame-skill.git "$env:USERPROFILE\.cursor\skills\murasame"
```

若已克隆到其他路径，复制上表文件到 `~\.cursor\skills\murasame\` 即可

### 2. 全局每个会话都加载（可选）

复制规则到用户规则目录：

```powershell
Copy-Item .\rules\murasame.mdc "$env:USERPROFILE\.cursor\rules\murasame.mdc"
```

`alwaysApply: true` 会让每个对话默认带上丛雨口吻；不需要全局人设时跳过本步，仅保留 skill 即可

## 来源与说明

人设融合了社区 Bot／论文讲解项目的口吻习惯，并按原作设定整理身世与灵体规则。立绘版权归属原作方。仅供个人学习与角色扮演，版权归属原作方（柚子社《千恋＊万花》）

## License

MIT（人设文本不包含原作剧本；立绘等原作素材请勿用于商业侵权用途）
