<div align="right">
  简体中文 | <a href="./README_en.md">Eng</a>
</div>

<div align='center'>
  <img src="https://github.com/datawhalechina/musiclm-universe/blob/main/docs/images/MusicLM-Universe.jpg" alt="alt text" width="100%">
  <h1>musiclm-universe</h1>
  <h3>音乐生成模型原理、优化与项目实战</h3>
  <div align="center">
  <a href="https://trendshift.io/repositories/15520" target="_blank">
  </a>
  </div>
  <p><em> <strong>MusicLM-Universe：</strong>系统化讲解音乐生成语言模型（Music Language Model）的开源教程项目，兼顾理论基础、实践部署与进阶优化，助力开发者从入门到精通音乐生成技术</em></p>
  <img src="https://img.shields.io/github/stars/datawhalechina/musiclm-universe?style=flat&logo=github" alt="GitHub stars"/>
  <img src="https://img.shields.io/github/forks/datawhalechina/musiclm-universe?style=flat&logo=github" alt="GitHub forks"/>
  <img src="https://img.shields.io/github/watchers/datawhalechina/musiclm-universe?style=flat&logo=github" alt="GitHub watchers"/>
  <a href="https://github.com/datawhalechina/musiclm-universe"><img src="https://img.shields.io/badge/GitHub-Project-blue?style=flat&logo=github" alt="GitHub Project"></a>
  <a href="https://datawhalechina.github.io/musiclm-universe/"><img src="https://img.shields.io/badge/Online%20Reading-grey?style=flat&logo=gitbook" alt="Online Reading"></a>
</div>

---

## 项目介绍

随着 AI 生成技术的迭代，音乐生成语言模型（Music Language Model）已成为音频领域的研究与应用热点。本项目旨在搭建一个从基础到进阶的完整学习路径，带领学习者掌握音乐生成的核心原理、部署方法与优化思路，实现从使用模型到优化模型、融合应用的进阶。

项目聚焦 MusicLM 相关技术，覆盖数据表示、模型部署、优化框架及多模块融合，以实战为核心，配套相关代码演示，适合有基础Python编程能力、对AI音乐生成感兴趣的开发者、学生及自学者。


####  在线文档：https://datawhalechina.github.io/musiclm-universe/

本项目内容按模块逐步推进，可直接克隆仓库，结合Notebook演示与代码示例，快速上手实践。
```bash

git clone https://github.com/your-username/musiclm-universe.git
cd musiclm-universe

# 创建环境激活后
pip install -r requirements.txt

# 注册内核
python -m ipykernel install --user --name musictransformer --display-name "Python (musictransformer)"

# 可运行 Jupyter Notebook

```

#### 项目收获：

- 🔍 掌握音乐数据表示、音频Tokenizer、Music Transformer核心原理
- 🏗️ 实践主流开源音乐生成模型（MusicGen / Diffrhythm2 / ACE-Step）的部署与源码解读
- ⚙️ 了解MusicGen的SFT+DPO+Reasoning优化思路，掌握音乐生成优化框架核心逻辑
- 🛠️ 探索音乐生成与音效融合的实践方法，实现更丰富的音频输出


##  内容目录

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
| <strong>第三部分 • 进阶：音乐生成与音效融合实践：<br> **MusicSFX-Fusion** </strong>                                                     |              |
| 第七章 音乐与音效生成                           |                             | 进行中  |
| 第八章 智能混音策略学习                            |训练混音策略模型                          |  进行中  |
| 第九章 音效融合及可视化                    |Gradio 搭建前端应用                       |  进行中   |


## 各部分详细介绍

#### 第一部分：音乐生成模型完整实现流程（Notebook演示）

本部分聚焦基础实现，通过 Notebook 演示从数据到生成的完整流程，帮助建立对 MusicLM 的核心认知。

- 音乐数据表示：介绍波形、频谱、梅尔谱等音频表示方式，以及基础预处理流程。
- 音频 Tokenizer 原理：讲解如何将连续音频转为离散 token，并对比不同方法特点。
- Music Transformer 建模：基于 Transformer 构建音乐生成模型，理解其在时序建模中的应用。
- 训练与生成流程：完整演示训练与推理流程，帮助模型实现可用的音乐生成能力。

#### 第二部分：开源音乐生成模型部署实践与代码分析

本部分面向工程实践，围绕主流开源模型进行部署与源码拆解。

- MusicGen：理解其架构与生成机制，实现快速部署并分析关键模块。
- Diffrhythm2：关注轻量化与高效生成，掌握低资源环境下的使用方式。
- ACE-Step：侧重风格生成与节奏控制，对比不同模型的适用场景。

#### 第三部分：进阶：音乐生成与音效融合实践（开发中）

本部分整体围绕三个模块展开：音乐生成、环境音生成、音频合成。

模型组合：MusicGen 音乐生成 + AudioLDM 2 音效生成

音频融合优化：
- 时间对齐（长度匹配）
- 淡入淡出（提升自然度）
- 混音参数学习（自动 gain / EQ / reverb）
- 伪标签构建（无需人工标注）

目标是从生成音乐走向生成完整声音场景。

## 如何学习 

MusicLM-Universe 是一个兼顾理论与实践的项目，它的核心并不在于理解模型细节，而在于建立一套完整的音乐生成系统认知。因此，我们更推荐你以构建系统的视角来学习，而不是单纯阅读内容。 

在学习路径上，你可以从第一部分入手，通过 Notebook 逐步理解音乐是如何被表示、编码并最终生成的。这一阶段的重点不在于推导复杂公式，而在于真正理解音乐如何被模型理解，亲自运行代码、修改参数，观察生成结果的变化。 

进入第二部分时，学习重点将从原理转向工程。你会接触到真实可用的开源模型，并理解它们是如何被设计与实现的。建议在这一阶段多做对比与拆解，思考不同模型在生成质量、效率和可控性上的取舍。 

第三部分更偏向“系统构建”。在这一阶段，思考如何优化生成效果，以及如何将多个模型组合成一个完整应用。可以尝试根据自己的需求修改生成逻辑，甚至设计属于自己的优化策略。 

整个学习过程中，最重要的一点是：一定要动手实践。当你完成全部内容后，你将不仅理解 MusicLM，更具备设计和构建音乐生成系统的能力。


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
