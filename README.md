# 语音信息处理课程作业

本仓库用于保存语音信息处理课程的实验作业。目前已上传 Lab1 和 Lab2，后续实验会继续按 `02_labs/` 目录结构补充。

## 当前内容

```text
.
├── README.md
├── .gitignore
└── 02_labs/
    ├── lab1_signal_features/
    │   ├── exp1_2026.ipynb
    │   ├── exp1_2026.pdf
    │   └── LJ001-0011.wav
    └── lab2_poetry_lstm/
        └── lab2.ipynb
```

## Lab1：语音信号特征提取

Lab1 主要围绕语音信号的基础特征提取展开，内容包括：

- 使用 `librosa` 读取音频、绘制波形和频谱图。
- 使用 `torchaudio` 计算 Mel 频谱图。
- 手动实现传统语音特征提取流程：
  - 预加重
  - 分帧
  - 加窗
  - STFT 幅度谱和功率谱
  - Mel 滤波器组
  - FBank
  - MFCC
- 对比 Hamming 窗和 Hann 窗对幅度谱的影响。
- 使用 Wav2Vec2 预训练模型提取深度音频特征，完成加分项。

## 文件说明

- `02_labs/lab1_signal_features/exp1_2026.ipynb`  
  Lab1 主实验 notebook，包含代码、图像输出和实验分析。

- `02_labs/lab1_signal_features/exp1_2026.pdf`  
  Lab1 实验指导文件。

- `02_labs/lab1_signal_features/LJ001-0011.wav`  
  实验使用的示例音频文件。

## 运行环境

推荐使用 Conda 环境。实验中使用的主要 Python 包包括：

```text
numpy
pandas
matplotlib
librosa
torch
torchaudio
scipy
```

本地实验环境为：

```text
conda environment: speech_env
python: 3.x
torch: 2.4.1+cpu
torchaudio: 2.4.1+cpu
```

如果需要重新创建环境，可以参考：

```bash
conda create -n speech_env python=3.8
conda activate speech_env
pip install numpy pandas matplotlib librosa scipy torch torchaudio
```

## 运行方式

进入 Lab1 目录：

```bash
cd 02_labs/lab1_signal_features
```

然后使用 Jupyter Notebook 或 VS Code 打开：

```text
exp1_2026.ipynb
```

建议按 notebook 顺序从上到下运行。Wav2Vec2 加分项第一次运行时会下载预训练模型权重，需要保持网络连接。

## Lab1 输出说明

Notebook 中包含以下主要输出：

- 原始音频波形图。
- `librosa` 频谱图和 Mel 频谱图。
- `torchaudio` Mel 频谱图。
- 预加重后波形图。
- 分帧、加窗、STFT 后的幅度谱图。
- Hamming 窗与 Hann 窗的幅度谱对比图。
- FBank 特征图。
- MFCC 特征图。
- Wav2Vec2 深度音频特征图。

## Lab2：古诗生成

Lab2 以字符级循环神经网络为基础，围绕古诗生成任务展开，内容包括：

- 使用唐诗 JSON 数据完成清洗、构建词典和序列填充。
- 将预处理后的诗歌样本保存为定长训练数据。
- 手动实现多层 LSTM，并完成训练与验证。
- 绘制训练集与验证集的 loss 曲线。
- 基于训练后的模型生成藏头诗与续写古诗。
- 使用 OpenAI 兼容接口调用大语言模型，完成诗歌生成对比实验。

## 后续计划

后续实验会继续放在 `02_labs/` 下，例如：

```text
02_labs/lab3_*/
```

每个实验会尽量保留主 notebook、实验说明和必要的小型数据文件。大型模型权重、缓存文件、压缩包和临时输出不会直接提交到仓库。
