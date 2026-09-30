<div align="center">

![Zheng Han — 语音识别 × 端到端语音大模型](assets/header.svg)

[![Jinan University](https://img.shields.io/badge/Soochow_University-%E8%8B%8F%E5%B7%9E%E5%A4%A7%E5%AD%A6-2563eb?style=flat-square)](https://github.com/StarWorkshop)
![speech recognition](https://img.shields.io/badge/focus-speech_recognition-d97706?style=flat-square)
![end-to-end spoken LM](https://img.shields.io/badge/focus-end--to--end_spoken_LM-2563eb?style=flat-square)
![streaming-native](https://img.shields.io/badge/streaming--native-bounded_buffers-5c6b85?style=flat-square)
![offline-first](https://img.shields.io/badge/offline--first-always-5c6b85?style=flat-square)

</div>

![研究旅程：wavrail → dialogvox](assets/journey.svg)

## 项目

| 项目 | 研究方向 | 已实现内容 |
|---|---|---|
| [wavrail](https://github.com/StarWorkshop/wavrail) | 流式语音识别 | WAV I/O 与帧化、log-mel 特征、CTC 贪心/前缀束解码、transducer 式帧同步发射、强制对齐、中英文 CER/WER、分块流式管线与延迟核算、合成音频上的可训练声学模型 |
| [dialogvox](https://github.com/StarWorkshop/dialogvox) | 端到端语音对话 | RVQ 神经音频编解码、语音-文本统一 token、紧凑对话 LM 与联合损失、KV-cache 流式生成与有界缓冲、外部语音大模型适配器协议、回合级评测与可复现报告 |

两个项目都包含命令行工具、可运行示例、契约/黄金测试和 CPU 模型测试，全部离线可复现。

## 技术栈

![Python](https://img.shields.io/badge/Python-3.11%2B-3776ab?style=flat-square&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-core-013243?style=flat-square&logo=numpy&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-CPU_extra-ee4c2c?style=flat-square&logo=pytorch&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-contract_%2B_golden-0a9edc?style=flat-square)
![ruff](https://img.shields.io/badge/ruff-format_%2B_lint-d7ff64?style=flat-square)
![GitHub Actions](https://img.shields.io/badge/CI-3.11_%2F_3.12_%2F_3.13-2088ff?style=flat-square&logo=githubactions&logoColor=white)

## 活动

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/StarWorkshop/StarWorkshop/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/StarWorkshop/StarWorkshop/output/github-snake.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/StarWorkshop/StarWorkshop/output/github-snake.svg" />
</picture>

## 当前关注

- 流式识别的延迟核算：算法延迟 vs 发射延迟，分块与离线输出的等价性。
- 语音-文本统一 token 上的联合建模、KV-cache 流式解码与背压语义。
- 合成数据上的可复现训练链路：种子、锁文件与逐提交检查。
