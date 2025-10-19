﻿# Hands-On Large Language Models CN(ZH)  -- 动手学大模型

这本书（Hands-On Large Language Models）原作者是 [Jay Alammar](https://www.linkedin.com/in/jalammar/)，[Maarten Grootendorst](https://www.linkedin.com/in/mgrootendorst/)。 英文好的同学强烈推荐支持原书，访问 [原书地址](https://github.com/HandsOnLLM/Hands-On-Large-Language-Models) 。


> 这是[中文版本的 hands-on LLMs](https://github.com/bbruceyuan/Hands-On-Large-Language-Models-CN)，推荐大家访问原书。
> 
> 也非常欢迎大家感兴趣可以关注公众号【[chaofa用代码打点酱油](https://mp.weixin.qq.com/s/WxLbKvW4_9g0ajQ0wGRruQ)】获得文字更新推送~ 或者加群来吹水聊天（🤣）


## 中文版有什么特点
- 对代码进行了更详细的注释，并且在**部分内容加上自己的理解**。
- 有更适合国内网络环境使用的 Notebook 版本，不需要翻墙可以使用（主要是更快）
  - 这里我也是为了免费用了 [openbayes](https://openbayes.com/console/signup?r=bbruceyuan_1o6b) 的 GPU，注册可以送 5 小时 CPU 和 3 小时 4090 GPU，如果用[我的链接注册](https://openbayes.com/console/signup?r=bbruceyuan_1o6b)，我们都能多一个小时。能薅一点牛毛是一点是一点，目标是免费录完这次教程。
  - 如果你不太喜欢 notebook 类型，更喜欢实验室这种 Linux 类型的环境，那么推荐你使用  [AIStackDC](https://aistackdc.com/phone-register?invite_code=D872A9) 算力平台，可以直接 ssh，配置好之后就是一个独立的开发机，如果使用[我的邀请链接](https://aistackdc.com/phone-register?invite_code=D872A9)，可以额外获得 2 张 1 折优惠券（5 小时）和 3 张 5 折优惠券（36 小时），这样前一百个小时基本免费吧。
- **配套的中文视频讲解**。
  - [YouTube 视频](https://www.youtube.com/watch?v=BvdAH38BCe8) 
  - [B站视频-chaofa用代码打点酱油](https://www.bilibili.com/video/BV16Am3Y4ES3/)


## 目录

建议海外用户通过 Google Colab 运行所有示例，以获得最简单的设置。Google Colab 允许您免费使用具有 16GB 显存的 T4 GPU。所有示例主要使用 Google Colab 构建和测试，因此它应该是更稳定的平台。然而，任何其他云提供商都应该可以工作。 

国内用户如果想要运行，最好还是用[中文可运行 Notebook](https://openbayes.com/console/bbruceyuan/containers/RhWOr6vTLN4)，你可以复制我的容器直接运行这些代码，[注册链接](https://openbayes.com/console/signup?r=bbruceyuan_1o6b)，这样不需要翻墙，国内网络环境访问 Google Colab 可能比较慢。


| 章节 | Google Colab | 中文 Notebook<br/>复制后可直接运行| 视频讲解 <br/> (可点击)|
|---|---|------|------|
| 第一章: 介绍大模型  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter01/Chapter%201%20-%20Introduction%20to%20Language%20Models.ipynb)   | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/bbruceyuan/containers/pfiQnfIjPo6) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV16Am3Y4ES3)](https://www.bilibili.com/video/BV16Am3Y4ES3/)<br />[![Youtube](https://img.shields.io/youtube/views/BvdAH38BCe8?style=social)](https://www.youtube.com/watch?v=BvdAH38BCe8) |
| 第二章: Tokens and Embeddings  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter02/Chapter%202%20-%20Tokens%20and%20Token%20Embeddings.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/bbruceyuan/containers/LkZZVWNf0F4) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1yRB8YwEBt)](https://www.bilibili.com/video/BV1yRB8YwEBt/)<br /> [![Youtube](https://img.shields.io/youtube/views/cC9W0Yv2p_k?style=social)](https://www.youtube.com/watch?v=cC9W0Yv2p_k)|
| 第三章: Looking Inside Transformer LLMs  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter03/Chapter%203%20-%20Looking%20Inside%20LLMs.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/bbruceyuan/containers/N8TSxf4B7ux) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1ZDqfYYEyB)](https://www.bilibili.com/video/BV1ZDqfYYEyB/)<br /> [![Youtube](https://img.shields.io/youtube/views/YbE-kQOaHoM?style=social)](https://www.youtube.com/watch?v=YbE-kQOaHoM) |  
| 第四章: Text Classification  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter04/Chapter%204%20-%20Text%20Classification.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/bbruceyuan/containers/jeIPTPLojfo) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1Zx6hYoEDe)](https://www.bilibili.com/video/BV1Zx6hYoEDe/)<br /> [![Youtube](https://img.shields.io/youtube/views/ClsD01EqnLY)](https://www.youtube.com/watch?v=ClsD01EqnLY)|
| 第五章: Text Clustering and Topic Modeling  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter05/Chapter%205%20-%20Text%20Clustering%20and%20Topic%20Modeling.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/bbruceyuan/containers/Qnc6Zlkkc5A) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1nLcVePEJV)](https://www.bilibili.com/video/BV1nLcVePEJV/)<br /> [![Youtube](https://img.shields.io/youtube/views/MFKkwIwGRcA)](https://www.youtube.com/watch?v=MFKkwIwGRcA)|
| 第六章: Prompt Engineering  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter06/Chapter%206%20-%20Prompt%20Engineering.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/signup?r=bbruceyuan_1o6b) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1btTRzMEwe)](https://www.bilibili.com/video/BV1btTRzMEwe/)<br />  [![Youtube](https://img.shields.io/youtube/views/5FzJCQEKW-o)](https://www.youtube.com/watch?v=5FzJCQEKW-o)|
| 第七章: Advanced Text Generation Techniques and Tools  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter07/Chapter%207%20-%20Advanced%20Text%20Generation%20Techniques%20and%20Tools.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/signup?r=bbruceyuan_1o6b) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1DKM8zuEWc)](https://www.bilibili.com/video/BV1DKM8zuEWc/)<br />  [![Youtube](https://img.shields.io/youtube/views/dSJ6-yOala8)](https://www.youtube.com/watch?v=dSJ6-yOala8) |  
| 第八章: Semantic Search and Retrieval-Augmented Generation  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter08/Chapter%208%20-%20Semantic%20Search.ipynb) <br /> [RAG 进化之路：传统 RAG 到工具与强化学习双轮驱动的 Agentic RAG](https://yuanchaofa.com/post/from-native-rag-to-agentic-rag.html) | [![中文可运行 Notebook](https://img.shields.io/badge/python-code%E5%B9%B3%E5%8F%B0-pink)](https://github.com/bbruceyuan/Hands-On-Large-Language-Models-CN/tree/master/chapter08) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1iLx6zRETu)](https://www.bilibili.com/video/BV1iLx6zRETu/)<br />  [![Youtube](https://img.shields.io/youtube/views/6cuiF4Lodrs)](https://www.youtube.com/watch?v=6cuiF4Lodrs)  |
| 第九章: Multimodal Large Language Models  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter09/Chapter%209%20-%20Multimodal%20Large%20Language%20Models.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/signup?r=bbruceyuan_1o6b) | 在录了~ |
| 第十章: Creating Text Embedding Models  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter10/Chapter%2010%20-%20Creating%20Text%20Embedding%20Models.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/signup?r=bbruceyuan_1o6b) | 在录了~ |
| 第十一章: Fine-tuning Representation Models for Classification  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter11/Chapter%2011%20-%20Fine-Tuning%20BERT.ipynb)  |[![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/signup?r=bbruceyuan_1o6b) | 在录了~ |
| 第 12.1 章: 大模型 SFT  | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HandsOnLLM/Hands-On-Large-Language-Models/blob/main/chapter12/Chapter%2012%20-%20Fine-tuning%20Generation%20Models.ipynb)  | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/bbruceyuan/containers/OPg9Oo99ET6) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1NM1tY3Eu5)](https://www.bilibili.com/video/BV1NM1tY3Eu5/)<br />[![Youtube](https://img.shields.io/youtube/views/ZN_tfSTTBho?style=social)](https://www.youtube.com/watch?v=ZN_tfSTTBho) |
| bonous1 - 动手实现 LoRA（非import peft） | [LoRA 原理和 PyTorch 代码实现](https://yuanchaofa.com/hands-on-code/hands-on-lora.html) | [![中文可运行 Notebook](https://img.shields.io/badge/notebook-openbayes%E5%B9%B3%E5%8F%B0-pink)](https://openbayes.com/console/bbruceyuan/containers/dqZ35wOdmzh) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1fHmkYyE2w)](https://www.bilibili.com/video/BV1fHmkYyE2w/)<br /> | 
| bonus2 从零实现 GRPO (Agent RL），用于 Agentic RAG 训练 | [RAG 进化之路：传统 RAG 到工具与强化学习双轮驱动的 Agentic RAG](https://yuanchaofa.com/post/from-native-rag-to-agentic-rag.html) |[![中文可运行 Notebook](https://img.shields.io/badge/python-code%E5%B9%B3%E5%8F%B0-pink)](https://github.com/bbruceyuan/Hands-On-Large-Language-Models-CN/tree/master/chapter08) | [![bilibili](https://img.shields.io/badge/dynamic/json?label=views&style=social&logo=bilibili&query=data.stat.view&url=https%3A%2F%2Fapi.bilibili.com%2Fx%2Fweb-interface%2Fview%3Fbvid%3DBV1yX4aznE9s)](https://www.bilibili.com/video/BV1yX4aznE9s/)<br />[![Youtube](https://img.shields.io/youtube/views/TLDj0Cob_jk?style=social)](https://www.youtube.com/watch?v=TLDj0Cob_jk) |

> [!TIP]
> You can check the [setup](.setup/) folder for a quick-start guide to install all packages locally and you can check the [conda](.setup/conda/) folder for a complete guide on how to setup your environment, including conda and PyTorch installation.
> Note that the depending on your OS, Python version, and dependencies your results might be slightly differ. However, they
> should this be similar to the examples in the book. 

## 其他资源

We attempted to put as much information into the book without it being overwhelming. However, even with a 400-page book there is still much to discover! If you are interested in similar illustrated/visual guides we created, these might be of interest to you:

| [A Visual Guide to Mamba](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mamba-and-state)             |  [A Visual Guide to Quantization](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization) | [The Illustrated Stable Diffusion](https://jalammar.github.io/illustrated-stable-diffusion/) |
:-------------------------:|:-------------------------:|:-------------------------:
![](images/mamba.png)  |  ![](images/quant.png) |  ![](images/diffusion.png)


## Citation

Please consider citing the book if you consider it useful for your research:

```
@book{hands-on-llms-book,
  author       = {Jay Alammar and Maarten Grootendorst},
  title        = {Hands-On Large Language Models},
  publisher    = {O'Reilly},
  year         = {2024},
  isbn         = {978-1098150969},
  url          = {https://www.oreilly.com/library/view/hands-on-large-language/9781098150952/},
  github       = {https://github.com/HandsOnLLM/Hands-On-Large-Language-Models}
}
```
