# 小红书英语教学笔记

面向英语教师的小红书内容制作技能：核对真实教材，设计具体教学活动，制作具有艺术风格的整页配图，并提供可打印PDF。

## 能做什么

- 核验教材版本、单元、页码和任务，区分教材原内容、原创教学支架和自编示例。
- 默认交付笔记文案、7张配图、8页左右A4打印资料及整套ZIP；数量可按需求调整。
- 结合真实教材局部，随主题选择不同艺术方向，不固定同一种封面。
- 逐图、逐页目视检查，不编造课堂经验、学生表现或试教效果。

## 安装

在可使用技能安装器的Codex里发送以下指令。以下链接可直接使用：

```text
使用 $skill-installer，安装这个GitHub技能：
https://github.com/lission521/xiaohongshu-english-notes/tree/main/skills/xiaohongshu-english-notes
```

也可以把完整的 `skills/xiaohongshu-english-notes` 文件夹放进当前项目的 `.agents/skills/`，作为项目技能使用。不要只复制SKILL.md，保留agents、references和assets的相对结构。

安装后检查技能列表；未显示时重启Codex。

## 调用示例

```text
使用 $xiaohongshu-english-notes，帮我制作一篇新版人教七年级英语教学笔记，选合适单元，文案、配图和PDF一起完成。
```

```text
使用 $xiaohongshu-english-notes，制作八年级科普阅读课笔记。这次采用包豪斯风格，先核对真实教材。
```

```text
使用 $xiaohongshu-english-notes，只修改现有笔记的封面，保留正文与PDF。
```

## 使用环境

这是一套工作流程与质量要求，不自带模型、账号或生图额度。完整交付需要运行环境提供生图工具、文件处理能力和PDF制作/渲染能力；建议同时具有imagegen和pdf技能。工具可用性取决于使用者环境，其他代理工具需要自行适配。

## 文件结构

```text
README.md
skills/
  xiaohongshu-english-notes/
    SKILL.md
    agents/openai.yaml
    references/approved-examples.md
    assets/grade7-campus-cover.png
    assets/grade8-bees-cover.png
```

assets中的两张封面用于理解质量与视觉方向；其中的教材裁片仅对应示例单元，不能用于冒充其它教材依据。分享包不含完整教材、课堂照片、账号信息或本机路径。新任务必须重新核验目标教材。

## 上传到GitHub

1. 新建或选择一个仓库；希望所有人可访问时使用Public仓库。
2. 将本分享包解压，把README.md和skills文件夹上传到仓库中，保留结构；不要仅上传ZIP。
3. 提交文件后，复制技能文件夹的GitHub页面链接，即 `.../tree/分支名/skills/xiaohongshu-english-notes`。
4. 将该链接与上面的安装指令一同分享。若上传到了其他子目录，安装链接也相应调整。

本包是GitHub分享用的技能目录，不是已发布的插件。需要插件目录中的安装入口时，可进一步制作插件包。

## 官方参考

- 技能结构、项目发现路径、安装及插件分发：https://learn.chatgpt.com/docs/build-skills

## 后续怎样调整

如果你是本仓库维护者，可以直接让Codex读取仓库并修改，例如：

```text
帮我调整 https://github.com/lission521/xiaohongshu-english-notes 里的技能：默认改成6张图，PDF仍按教学内容安排。检查后提交到GitHub。
```

- 制作流程和内容要求：修改 `skills/xiaohongshu-english-notes/SKILL.md`。
- 技能显示名称和默认提示：修改 `skills/xiaohongshu-english-notes/agents/openai.yaml`。
- 参考案例：修改 `references/approved-examples.md`，对应图片放在 `assets/`。
- 安装和使用说明：修改本README。

已下载安装到别人电脑上的技能是独立副本；仓库更新后，使用者需要同步更新本地技能，不会自动修改他们已安装的文件。
