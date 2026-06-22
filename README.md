# 🍌 GeminiBanana for ComfyUI + 白嫖💲300 教程

**GeminiBanana** 是一个基于 **Gemini API** 与 **ComfyUI** 的自定义节点（Custom Node），它可以让你在 ComfyUI 工作流中调用 Gemini 生成文字、解析图像、或进行多模态交互，从而大幅提升工作流的自动化与创意能力。

天啦噜，企鹅都开始写代码了，因为鄙人不精通代码，完全是GPT制作的垃圾代码。
所以他现在在Comfyui内叫这个名字：Gemini Flash 2.5 Gen/Edit
肯定有一些小BUG，陆续会更新。。。希望有缘人给更新
特别鸣谢Lgong先生，他的Github主页是（我还不会@人）

---

## ✨ 功能特性

- 🔮 **Gemini API 接入**：支持调用 Gemini-Pro / Gemini-Flash 等模型。
- 🖼 **多模态支持**：文字、图像输入与输出。
- ⚡ **ComfyUI 原生集成**：可在工作流中作为节点调用，支持输入/输出连接。
- 🛠 **自定义参数**：支持温度（temperature）、最大长度（max_tokens）、Top-P 等参数配置。
- 📦 **易于扩展**：可以根据需要二次开发，扩展成更复杂的工作流组件。

---

## 📦 安装方法

1. 进入你的 ComfyUI `custom_nodes` 文件夹：
   ```bash
   cd ComfyUI/custom_nodes
2. 克隆本仓库：

   ```bash
   git clone https://github.com/yourname/ComfyUI-GeminiBanana.git
   ```

3. 安装依赖：

   ```bash
   pip install -r requirements.txt
   ```

4. 重启 ComfyUI，搜索节点列表中的 **Gemini Flash 2.5 Gen/Edit**。

---

## 🚀 使用示例

1. 在 ComfyUI 中添加 **Gemini Flash 2.5 Gen/Edit** 节点。
2. 输入：

   * **文本输入**：Prompt，例如 `"帮我写一首关于企鹅的诗"。`
   * **图像输入**（可选最多10张）：上传图片，作为 Gemini 的多模态上下文。
3. 输出：

   * 文本结果会显示在节点输出中。
   * 图像结果会保存到 ComfyUI 的输出目录。

---

## ⚙️ 节点参数说明
Banana遵照最后一个图的尺寸出图

当前节点支持两个模型：

* `Nano Banana Pro`
  * model id: `gemini-3-pro-image`
  * image size: `1K` / `2K` / `4K`
  * aspect ratio: `1:1` `2:3` `3:2` `3:4` `4:3` `4:5` `5:4` `9:16` `16:9` `21:9`
* `Nano Banana 2`
  * model id: `gemini-3.1-flash-image-preview`
  * image size: `0.5K` / `1K` / `2K` / `4K`
  * aspect ratio: 在 `Nano Banana Pro` 的基础上，额外支持 `1:4` `4:1` `1:8` `8:1`

节点 UI 已新增 `model` 选项；`image_size` 和 `aspect_ratio` 会显示并集，实际请求时会按所选模型做校验。

---


## 🤝 致谢

* [ComfyUI](https://github.com/comfyanonymous/ComfyUI) 社区提供的优秀框架
* [Google Gemini](https://deepmind.google/technologies/gemini/) 提供的多模态大模型
* 本项目由 **GeminiBanana** 团队/作者开发与维护
* 致谢企鹅和原项目 https://github.com/PenguinTeo/Comfyui-GeminiBanana

---

## 📜 License

MIT License. 自由使用、修改与分发，但请保留署名。

---

```
