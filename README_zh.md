# Selab-Winter（CS336 Assignment 1）

寒假实验室交流 CS336 Assignment 1 代码仓库。项目使用 `uv` 进行依赖与环境管理，日常实验与记录主要在 Jupyter Notebook 中完成。

## 目录结构
- `main.py`：课程练习/实验入口脚本（可按需扩展）
- `notebooks/`：课程实验与记录
- `pyproject.toml`：项目元数据与依赖声明
- `uv.lock`：依赖锁定文件

## 环境要求
- Python >= 3.12
- `uv`
- Jupyter

## 快速开始
1. 安装依赖（首次会创建虚拟环境）：

```bash
uv sync
```

2. 启动 Jupyter（推荐 Lab）：

```bash
uv run jupyter lab
```

如需运行脚本：

```bash
uv run python main.py
```

## 课程计划
| 内容安排 | 目标 | 开始时间 |
| --- | --- | --- |
| 1. Python 基础、开发环境与工程基建 | 完成 Python 语法速通，构建一个基于 uv 的现代化深度学习工程结构 | 2月3日 20:00- |
| 2. Byte Pair Encoding (BPE) 原理与词表训练 | 掌握 BPE 统计算法，从原始语料中统计并生成一个最优的词表 | 2月x日 20:00- |
| 3. Tokenizer 类实现 | 加载训练好的词表，实现文本与 Token ID 的双向转换 | 2月x日 20:00- |
| 4. Transformer 的原理以及实现(1) - 核心组件与工具 | 实现 Transformer 架构所需的线性层(Linear)、嵌入层(Embedding)、归一化层(RMSNorm)、激活函数(SwiGLU)以及基础数学工具函数(softmax) | 2月x日 20:00- |
| 5. Transformer 的原理以及实现(2) - 位置编码与注意力核心 | 实现让模型感知序列顺序的旋转位置编码(RoPE)以及点积缩放注意力(Scaled Dot-Product Attention)的核心数学计算 | 2月x日 20:00- |
| 6. Transformer 的原理以及实现(3) - 核心架构组合与多头注意力封装、调整总结 | 实现标准的 Transformer Block 模块，并将多个 Block 堆叠组装成完整的 Transformer 语言模型(TransformerLM) | 2月x日 20:00- |
| 7. train 过程各模块原理以及实现(1) - 优化器与损失函数 | 实现模型训练所需的支持算法，包括解耦权重衰减的优化 (AdamW)、数值稳定的损失函数(CrossEntropy)以及学习率调度(Cosine Scheduler) | 2月x日 20:00- |
| 8. train 过程各模块原理以及实现(2) - 训练器与配置管理 | 实现高层训练逻辑，包括强类型配置管理(TrainingConfig)、训练循环控制(Trainer Class)以及断点续传与日志系统 | 2月x日 20:00- |
| 9. 系统集成测试与调整总结 | 对之前的内容进行 QA | 2月x日 20:00- |
| 10. 训练实操与 AutoDL 服务器使用 | 在真实的云端 GPU 环境下进行模型训练与监控 | 2月x日 20:00- |
| 11. Inference 推理过程实现 | 加载训练好的模型权重，实现像 ChatGPT 一样的文本生成 | 2月x日 20:00- |

## 备注
- 时间为暂定，实际以课程安排为准。
- 后续可在 `notebooks/` 中维护每次课程的实验记录与结论。
