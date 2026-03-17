# MusicLM-Universe | 音乐生成大模型原理与实践教程

## 项目简介

**MusicLM-Universe** 是一个系统化讲解 **音乐生成大模型（Music Language Model, MusicLM）** 的开源教程项目。

随着大语言模型的发展，音乐生成模型正从 MIDI 建模走向端到端纯音频生成，形成 Transformer、Diffusion、Hybrid 等多种技术路线。

本项目重新梳理了 MusicLM 的完整知识体系，我们将音乐视为一种可建模的语言，深入解析：

- 音乐数据表示
- 音频 Tokenizer 原理
- Music Transformer 建模
- 训练与生成流程实现
- 主流开源音乐生成模型（MusicGen / Diffrhythm2 / ACE-Step）部署与源码分析

通过 Notebook 实现，文档讲解和开源模型源码分析，我们希望帮助读者建立音乐大模型如何被构建的完整技术流程。


## 项目受众

- 对 AI 音乐生成 感兴趣的开发者
- 具备基本 LLM 基础的 AI 音乐爱好者


## 目录

### **一、MusicLM 完整实现流程 Notebook 部分** 

[**第 1 章 Music Representations** 音乐数据表示](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c1_Music_Representations.ipynb) *@田佳铭*
  
[**第 2 章 Audio Tokenizer**](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c2_Audio_Tokenizer_Encodec.ipynb) *@田佳铭*

[**第 3 章 Music Transformer**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/notebook) *@田佳铭*

- [**3.1 Model Training** 模型训练](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c3_1_MusicTransformer_Training.ipynb)
- [**3.2 Music Generation** 音乐生成](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/notebook/c3_2_MusicTransformer_Generation.ipynb)

### **二、Music 生成基础知识文档部分**

[**第 4 章** 音乐生成大模型基础知识](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/docs) *@王泊轩* 

### **三、开源音乐生成大模型部署使用及代码分析**

[**第 5 章 Transformer** 音乐生成模型 **- MusicGen**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/tutorial/MusicGen) *@林睿哲*
  
- [**5.1 MusicGen** 部署及使用](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/MusicGen/MusicGen_Setup_and_Usage.md)
- [**5.2 MusicGen** 开源代码分析](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/MusicGen/MusicGen_Codebase_Analysis.md)
  
[**第 6 章 Diffusion** 音乐生成模型 **- Diffrhythm2**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/tutorial/Diffrhythm2) *@刘秋杰*

- [**6.1 Diffrhythm2** 部署及使用](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/Diffrhythm2/DiffRhythm2_Setup_and_Usage.md)
- [**6.2 Diffrhythm2** 开源代码分析](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/Diffrhythm2/DiffRhythm2_Codebase_Analysis.md)
  
[**第 7 章 Transformer & Diffusion** 音乐生成模型 **- ACE-Step**](https://github.com/minimum-generated-pig/musiclm-universe/tree/main/tutorial/ACE-Step) *@田佳铭*

- [**7.1 ACE-Step** 部署及使用](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/ACE-Step/ACE-Step_Setup_and_Usage.md)
- [**7.2 ACE-Step 1.5** 开源代码分析](https://github.com/minimum-generated-pig/musiclm-universe/blob/main/tutorial/ACE-Step/ACE-Step_Codebase_Analysis.md)


## 参与贡献

- 如果你发现了一些问题，可以提Issue进行反馈，如果提完没有人回复你可以联系[保姆团队](https://github.com/datawhalechina/DOPMC/blob/main/OP.md)的同学进行反馈跟进~
- 如果你想参与贡献本项目，可以提Pull request，如果提完没有人回复你可以联系[保姆团队](https://github.com/datawhalechina/DOPMC/blob/main/OP.md)的同学进行反馈跟进~
- 如果你对 Datawhale 很感兴趣并想要发起一个新的项目，请按照[Datawhale开源项目指南](https://github.com/datawhalechina/DOPMC/blob/main/GUIDE.md)进行操作即可~

## 关注我们

<div align=center>
<p>扫描下方二维码关注公众号：Datawhale</p>
<img src="https://raw.githubusercontent.com/datawhalechina/pumpkin-book/master/res/qrcode.jpeg" width = "180" height = "180">
</div>

## LICENSE

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。

*注：默认使用CC 4.0协议，也可根据自身项目情况选用其他协议*
