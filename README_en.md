[[中文](https://github.com/bojone/NBCE/blob/main/README.md)|English]

# Naive Bayes-based Context Extension
Using the Naive Bayes idea to extend the context handling length of LLM.

Now, any LLM can utilize NBCE to become a model capable of processing context of any length (as long as there is enough computing power)!

<img src="https://raw.githubusercontent.com/bojone/NBCE/34601ad70eb1bdae50a026234b8980da275df775/NBCE2.png" width=600>

## Introduction

Inspired by the Naive Bayes formula:

<img src="https://raw.githubusercontent.com/bojone/NBCE/main/NBCE.png" width=600>

For details, please refer to the blog: https://kexue.fm/archives/9617

Demo model used: https://openbuddy.ai/

Currently, combining a 7b model and 8*A800, it can still perform reading comprehension correctly on a **50k** context!

## Features
- Plug and play
- Model-Agnostic
- No fine-tuning required
- Linear efficiency
- Simple implementation
- Decent performance
- Interpretability

## Citation
```
@misc{nbce2023,
  title={Naive Bayes-based Context Extension},
  author={Jianlin Su},
  year={2023},
  howpublished={\url{https://github.com/bojone/NBCE}},
}
```
## Communication
QQ discussion group: 808623966, for WeChat group, please add the robot WeChat ID spaces_ac_cn

