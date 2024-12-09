[中文|[English](https://github.com/bojone/NBCE/blob/main/README_en.md)]

# Naive Bayes-based Context Extension
使用朴素贝叶斯思想来扩展LLM的Context处理长度。

现在，任何LLM都可以利用NBCE成为可以处理任意长Context的模型了（只要算力足够）！

<img src="https://raw.githubusercontent.com/bojone/NBCE/34601ad70eb1bdae50a026234b8980da275df775/NBCE2.png" width=600>

## 简介

基于朴素贝叶斯所启发的公式：

<img src="https://raw.githubusercontent.com/bojone/NBCE/main/NBCE.png" width=600>

细节请看博客：https://kexue.fm/archives/9617

所给的Demo包含12段不同的Context，总长度为9000多字，连同8个问题一次性输入到模型中（测试模型训练长度为2048，参数量为7B，可以在[OpenBuddy](https://openbuddy.ai/)下载），模型能够逐一根据所给Context正确回答这8个问题。值得指出的是，所有的Context、问题和答案加起来，超过了1万字！另外，有朋友简单尝试了简历匹配和作文打分应用，效果也尚可，非常建议大家亲自调试一下。

**最新测试结果**：在8*A800下，7B模型可以处理**50k**的context，并能正确地做阅读理解。(没有用完所有GPU，大概消耗160G显存）

## 特点
- 即插即用
- 模型无关
- 不用微调
- 线性效率
- 实现简单
- 效果尚可
- 可解释性

## 引用

```
@inproceedings{nbce_naacl,
  author       = {Jianlin Su and
                  Murtadha Ahmed and
                  Bo Wen and
                  Luo Ao and
                  Mingren Zhu and
                  Yunfeng Liu},
  editor       = {Kevin Duh and
                  Helena G{\'{o}}mez{-}Adorno and
                  Steven Bethard},
  title        = {Naive Bayes-based Context Extension for Large Language Models},
  booktitle    = {Proceedings of the 2024 Conference of the North American Chapter of
                  the Association for Computational Linguistics: Human Language Technologies
                  (Volume 1: Long Papers), {NAACL} 2024, Mexico City, Mexico, June 16-21,
                  2024},
  pages        = {7791--7807},
  publisher    = {Association for Computational Linguistics},
  year         = {2024},
  url          = {https://doi.org/10.18653/v1/2024.naacl-long.431},
  doi          = {10.18653/V1/2024.NAACL-LONG.431},
  timestamp    = {Thu, 29 Aug 2024 17:13:57 +0200},
}
```
## 交流
QQ交流群：808623966，微信群请加机器人微信号spaces_ac_cn

