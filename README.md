[中文|[English](https://github.com/bojone/NBCE/blob/main/README_en.md)]

# Naive Bayes-based Context Extension
使用朴素贝叶斯思想来扩展LLM的Context处理长度。

现在，任何LLM都可以利用NBCE成为可以处理任意长Context的模型了（只要算力足够）！

<img src="https://raw.githubusercontent.com/bojone/NBCE/34601ad70eb1bdae50a026234b8980da275df775/NBCE2.png" width=600>

## 简介

基于朴素贝叶斯所启发的公式：

<img src="https://raw.githubusercontent.com/bojone/NBCE/main/NBCE.png" width=600>

细节请看博客：https://kexue.fm/archives/9617

Demo所用模型：https://openbuddy.ai/

目前结合7b模型和8*A800，在**50k**的context上仍能正确地做阅读理解！

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
@misc{nbce2023,
  title={Naive Bayes-based Context Extension},
  author={Jianlin Su},
  year={2023},
  howpublished={\url{https://github.com/bojone/NBCE}},
}
```
## 交流
QQ交流群：808623966，微信群请加机器人微信号spaces_ac_cn

