# Selab-Winter (CS336 Assignment 1)

This repository is for the Winter Lab CS336 Assignment 1. The project uses `uv` for dependency and environment management, and Jupyter Notebook as the primary place for experiments and notes.

## Structure
- `main.py`: entry script for exercises/experiments (extend as needed)
- `notebooks/`: experiments and notes
- `pyproject.toml`: project metadata and dependencies
- `uv.lock`: dependency lockfile

## Requirements
- Python >= 3.12
- `uv`
- Jupyter

## Quick Start
1. Install dependencies (creates a virtual environment on first run):

```bash
uv sync
```

2. Launch Jupyter (Lab recommended):

```bash
uv run jupyter lab
```

Run the script if needed:

```bash
uv run python main.py
```

## Course Plan
| Topic | Goal | Start Time |
| --- | --- | --- |
| 1. Python Basics, Dev Environment, and Project Setup | Complete Python fundamentals and build a modern DL project structure based on uv | Feb 3 20:00- |
| 2. Byte Pair Encoding (BPE) and Vocabulary Training | Understand BPE statistics and generate an optimal vocab from raw corpora | Feb x 20:00- |
| 3. Tokenizer Implementation | Load trained vocab and implement text ↔ token ID conversion | Feb x 20:00- |
| 4. Transformer Implementation (1) - Core Components & Tools | Implement Linear, Embedding, RMSNorm, SwiGLU, and softmax | Feb x 20:00- |
| 5. Transformer Implementation (2) - Positional Encoding & Attention Core | Implement RoPE and the core math of scaled dot-product attention | Feb x 20:00- |
| 6. Transformer Implementation (3) - Block Composition & MHA | Build Transformer blocks and stack into a TransformerLM | Feb x 20:00- |
| 7. Training Modules (1) - Optimizer & Loss | Implement AdamW, numerically stable CrossEntropy, and Cosine LR scheduler | Feb x 20:00- |
| 8. Training Modules (2) - Trainer & Config | Implement TrainingConfig, Trainer, checkpointing and logging | Feb x 20:00- |
| 9. System Integration Test & Review | QA for all components | Feb x 20:00- |
| 10. Training Practice & AutoDL Usage | Train and monitor on a real cloud GPU | Feb x 20:00- |
| 11. Inference Implementation | Load trained weights and generate text like ChatGPT | Feb x 20:00- |

## Notes
- Times are tentative and subject to course scheduling.
- Maintain per-session experiments and conclusions in `notebooks/`.
