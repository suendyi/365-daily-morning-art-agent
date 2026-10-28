# ChatGPT 导入指南

本指南介绍如何在 ChatGPT 中使用「365天晨间艺术系统 Agent」。推荐先创建一个 ChatGPT Project（项目），把 Agent 指令放在项目指令中，把模块说明和使用方法作为项目资料。项目指令和来源会供该项目中的对话复用。

## 推荐方式：创建 ChatGPT Project

### 1. 获取项目文件

打开并复制 [Agent 指令](https://github.com/suendyi/365-daily-morning-art-agent/blob/main/docs/AGENT_INSTRUCTIONS.md)全文。建议同时保存以下参考资料：

- [模块说明](https://github.com/suendyi/365-daily-morning-art-agent/blob/main/docs/MODULE.md)
- [使用方法](https://github.com/suendyi/365-daily-morning-art-agent/blob/main/docs/USAGE.md)

### 2. 新建项目并添加指令

1. 登录 ChatGPT，在侧边栏选择 **New project / 新建项目**。
2. 输入项目名称，例如「365天晨间艺术系统」。
3. 打开项目菜单中的 **Project settings / 项目设置**，将完整 Agent 指令粘贴到项目指令栏并保存。
4. 在项目内新开对话开始使用。项目指令会应用于该项目中的对话。

### 3. 添加参考资料

在项目的 **Sources / 来源** 区域上传 `MODULE.md` 和 `USAGE.md`，或粘贴它们的内容。若界面提供添加来源/文件按钮，也可将这些 Markdown 文件拖入或选择上传。ChatGPT 项目不会自动读取你电脑上的文件夹，因此请上传或连接希望它使用的资料。

建议把 Agent 的行为规则放在项目指令，把解释性材料放在来源文件中。若想简化导入，可先只放项目指令，再按需要补充模块说明和使用方法。

### 4. 检查是否导入成功

在项目中新开一条对话，先输入：

> 请先复述本项目的日期核验、双语文案、图像交付和质量检查规则，不要生成作品。

核对回答是否符合指令；之后再输入：

> 创作今天的晨间艺术作品。先核对马来西亚当地日期；若无法可靠核实，请说明原因并暂停正式生成。

网页搜索、图像生成及文件上传等功能会因账户、工作区设置、平台和当前功能可用性而异。若没有图像生成功能，应明确说明，并只提供文案或图像提示词。

## 可选方式：配置自定义 GPT（若账户和工作区允许）

若你的 ChatGPT 界面仍提供创建或编辑 GPT 的权限：

1. 打开 GPTs 区域并选择 **Create / 创建**，或进入已有 GPT 的编辑页。
2. 在 **Instructions / 指令** 中粘贴 `AGENT_INSTRUCTIONS.md` 的全文。
3. 将 `MODULE.md` 和 `USAGE.md` 上传到 **Knowledge / 知识**。
4. 按账户可用性启用网页搜索、图像生成等能力，并在预览区按上面的检查提示试运行。
5. 保存后按界面可用的分享选项决定访问范围。

自定义 GPT 的创建、编辑和发布受账户方案、工作区权限及 OpenAI 当前产品安排影响；如果看不到创建入口，请使用上面的 Project 方式。指令定义行为，Knowledge 文件提供参考资料，两者用途不同。

## 定时任务说明

将资料导入 ChatGPT 不会自动建立定时任务。原设置中的每天 07:30（马来西亚时间，MYT/UTC+8）安排需要在目标 ChatGPT 账户或平台单独创建，并确认任务状态、图像生成能力和结果通知方式。若你的账户提供 Scheduled Tasks，可在 ChatGPT 中单独设置；功能范围会因账户和工作区而异。

## 官方资料

- [ChatGPT Projects：项目、指令与来源](https://learn.chatgpt.com/docs/projects)
- [OpenAI：ChatGPT 使用指南](https://learn.chatgpt.com/docs/use-chatgpt)
- 自定义 GPT 的当前可用性与创建流程可能调整，请查看 OpenAI Help Center 的 [创建和编辑 GPT](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)。
