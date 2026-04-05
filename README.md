<div align=center>
<img src="https://github.com/minigenepig/minigenepig/blob/main/images/111.jpg" width = "1000">
</div>

## **musiclm-universe** | 音乐生成模型原理、项目实战与优化框架

###  项目简介
**musiclm-universe** 是一个系统化讲解 **音乐生成语言模型（Music Language Model, MusicLM）** 的开源教程项目。

随着大语言模型的发展，音乐生成模型正从 MIDI 建模走向端到端纯音频生成，形成 Transformer、Diffusion、Hybrid 等多种技术路线。

本项目重新梳理了 MusicLM 的完整知识体系，我们将音乐视为一种可建模的语言，深入解析：

- 音乐数据表示
- 音频 Tokenizer 原理
- Music Transformer 建模
- 训练与生成流程实现
- 主流开源音乐生成模型（MusicGen / Diffrhythm2 / ACE-Step）部署与源码分析

通过 Notebook 实现，文档讲解和开源模型源码分析，我们希望帮助读者建立音乐大模型如何被构建的完整技术流程。

同时，本项目基于 Meta 的 MusicGen，构建了一个结合 SFT（Supervised Fine-Tuning） 与 DPO（Direct Preference Optimization） 的音乐生成优化框架，旨在提升：

- 指令遵循能力（Instruction Following）
- 音频质量与审美（Audio Quality & Aesthetics）
- 生成前规划能力（Optional: Reasoning）

该方法受到 “统一音频语言模型（UALM）” 思路启发，采用更轻量、可复现的工程路径，在中等规模数据下实现显著提升。


###  项目受众

- 对 AI 音乐生成 感兴趣的开发者
- 具备基本 LLM 基础的 AI 音乐爱好者


###  目录

| 章节                                                                                        | 分级内容                                      | 状态 |
| ------------------------------------------------------------------------------------------- | --------------------------------------------- | ---- |
| [引言：音乐生成模型基础知识](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/docs)   |                     | ✅    |
| <strong>第一部分：音乐生成模型完整实现流程 Notebook 演示</strong>                                                                                            |
| [第一章 **Music Representations** 音乐数据表示](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c1_Music_Representations.ipynb)    |     | ✅    |
| [第二章 **Audio Tokenizer**](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c2_Audio_Tokenizer_Encodec.ipynb)                             | Encodec 音频编码器            | ✅    |
| [第三章 **Music Transformer**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/notebook) | [**3.1 Model Training** 模型训练](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c3_1_MusicTransformer_Training.ipynb) <br>[**3.2 Music Generation** 音乐生成](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c3_2_MusicTransformer_Generation.ipynb)         | ✅    |
| <strong>第二部分：开源音乐生成模型部署实践与代码分析</strong>                                         |                                               |      |
| [第四章 **Transformer** 架构模型应用 **- MusicGen**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/tutorial/MusicGen)                 | [**4.1 MusicGen** 部署及使用](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/MusicGen/MusicGen_Setup_and_Usage.md) <br> [**4.2 MusicGen** 开源代码分析](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/MusicGen/MusicGen_Codebase_Analysis.md)  | ✅    | 
| [第五章 **Diffusion** 架构模型应用 **- Diffrhythm2**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/tutorial/Diffrhythm2) | [**5.1 Diffrhythm2** 部署及使用](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/Diffrhythm2/DiffRhythm2_Setup_and_Usage.md) <br> [**5.2 Diffrhythm2** 开源代码分析](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/Diffrhythm2/DiffRhythm2_Codebase_Analysis.md)   | ✅    |
| [第六章 **Transformer & Diffusion** 架构模型应用 **- ACE-Step**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/tutorial/ACE-Step)                             | [**6.1 ACE-Step** 部署及使用](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/ACE-Step/ACE-Step_Setup_and_Usage.md) <br> [**6.2 ACE-Step 1.5** 开源代码分析](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/ACE-Step/ACE-Step_Codebase_Analysis.md) | ✅    |
| <strong>第三部分 • 进阶：音乐生成优化框架实践：<br> **MusicGen（SFT）+ DPO + Reasoning** </strong>                                                     |              |
| [第七章 **SFT：** 分布对齐]                               | 高质量的文本-音频对微调 MusicGen                            | 进行中  |
| [第八章 **DPO：** 偏好优化]                              | 构建偏好对，优化模型生成                         |  进行中  |
| [第九章 **Reasoning**]                     | “生成前推理”机制，使模型具备音乐结构规划能力                      |  进行中   |
| [第十章 评估]                   | 核心指标、基准测试与评估框架                  |  进行中   |
| <strong>第四部分 • 进阶：音乐音效生成与智能混音实践：<br> **MusicSFX-Fusion** </strong>                                                     |              |
| [第十一章]                           |                             | 进行中  |
| [第十二章]                            |                          |  进行中  |
| [第十三章]                    |                       |  进行中   |
| [第十四章]                   |                   |  进行中   |


### MusicGen-DPO 音乐生成优化框架构建：MusicGen（SFT）+ DPO + Reasoning 偏好优化提升音乐生成

**项目核心方法：**

整个系统由三阶段组成：

1、SFT：分布对齐（Supervised Fine-Tuning）

使用高质量的文本-音频对（Rich Caption）对 MusicGen 进行微调，使模型适应目标数据分布。

2、DPO：偏好优化（Preference Optimization）

通过构建 (prompt, chosen, rejected) 偏好对，优化模型生成更符合文本语义（CLAP）、更符合人类审美（Aesthetic）

并引入 Adaptation 阶段（解决分布偏移）和 CE 正则（稳定训练）

3、Reasoning（可选）

引入“生成前推理”机制，使模型具备音乐结构规划能力和更强 controllability。

该方法受到 “统一音频语言模型（UALM）” 思路启发，采用更轻量、可复现的工程路径，在中等规模数据下实现显著提升。

###  核心贡献者
- 田佳铭-项目负责人
- 王泊轩-核心贡献者
- 林睿哲-核心贡献者
- 刘秋杰-核心贡献者

### 如何贡献
我们是一个开放的开源社区，欢迎任何形式的贡献！
- 报告 Bug - 发现内容或代码问题，请提交 Issue
- 提出建议 - 对项目有好想法，欢迎发起讨论
- 完善内容 - 帮助改进教程，提交你的 Pull Request
- 分享实践 - 在"社区贡献精选"中分享你的学习笔记和项目

### LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。
