# 电影感镜头卡

一个 Codex Skill，用来把零散的画面描述或已有提示词整理成一张可复制的中文镜头卡，适用于单镜头剧照和单镜头视频。

镜头卡依次填写人物锁定、光源清单、缺陷清单、调度与表演，以及可选的风格参考。你给定的人物、服装、光源、动作和台词都会保留。

## 使用方法

在 Codex 里输入 `$cinematic-shot-card`，接着用自己的话描述想要的画面。下面这段可以直接试用。

```text
用 $cinematic-shot-card 写一张剧照镜头卡。阴天下午，一位穿米色针织衫的女性坐在窗边。
左侧窗户的柔光是唯一光源。50mm，平视，中近景，背景轻微虚化。
肤色温润、高光柔和，帮我挑一条摄影机质感参考。
```

- **缺陷已定**时，Skill 会把你给出的效果归入对应类别，直接出卡。
- **缺陷拿不准**时，Skill 会根据现有布光、景深和环境给出候选，等你选定再出卡。
- **需要风格参考**时，可以指定摄影机、胶片或镜头，也可以描述想要的质感，让 Skill 挑一条写在最后。

## 在另一台电脑上使用

把仓库完整复制到 Codex 的个人 Skills 目录，文件夹命名为 `cinematic-shot-card`。以下命令适用于默认目录。

```sh
git clone https://github.com/Enghc1115/cinematic-shot-card.git ~/.codex/skills/cinematic-shot-card
```

克隆私有仓库时，需要使用有访问权限的 GitHub 账号。在 Codex 新对话中输入 `$cinematic-shot-card` 即可调用。

## 仓库文件

- 镜头卡模板和填写规则。 [SKILL.md](SKILL.md)
- 结合现有布光挑选成像效果。 [缺陷速查](references/imperfections.md)
- 12 项摄影机、胶片和镜头质感。 [风格参考速查](references/style.md)
- Codex 中显示的名称与调用示例。 [界面配置](agents/openai.yaml)
