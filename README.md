# kaparthy

A collection of forks of [karpathy (Andrej)](https://github.com/karpathy) open-source LLM and deep learning projects. Each project is kept in its own subdirectory and tracked as a separate repository, as listed in the [subrepos](subrepos) file.

All original work is by [Andrej Karpathy](https://github.com/karpathy). Refer to the upstream repositories for the canonical source, documentation, and discussion.

## Projects

| Directory | Description | Upstream |
|-----------|-------------|----------|
| [llama2-c](llama2-c/) | Train the Llama 2 architecture in PyTorch and run inference with a single C file ([run.c](llama2-c/run.c)). Includes a quantized runner ([runq.c](llama2-c/runq.c)) and Windows build support ([build_msvc.bat](llama2-c/build_msvc.bat), [win.c](llama2-c/win.c)). | [karpathy/llama2.c](https://github.com/karpathy/llama2.c) |
| [llm-c](llm-c/) | LLM pretraining in pure C and CUDA, with a reproduction of GPT-2 and GPT-3 miniseries models. Includes a CPU reference implementation ([train_gpt2.c](llm-c/train_gpt2.c)) and a PyTorch reference ([train_gpt2.py](llm-c/train_gpt2.py)). | [karpathy/llm.c](https://github.com/karpathy/llm.c) |
| [micrograd](micrograd/) | A tiny scalar autograd engine with backpropagation over a dynamically built DAG, and a small neural network library on top of it. Includes demo notebooks and tests. | [karpathy/micrograd](https://github.com/karpathy/micrograd) |
| [nanochat](nanochat/) | A minimal, hackable harness for training LLMs on a single GPU node. Covers tokenization, pretraining, finetuning, evaluation, and inference through a CLI. | [karpathy/nanochat](https://github.com/karpathy/nanochat) |
| [nanoGPT](nanoGPT/) | A compact codebase for training and finetuning medium-sized GPT models. The upstream project is deprecated in favor of nanochat. | [karpathy/nanoGPT](https://github.com/karpathy/nanoGPT) |

## Repository layout

```
kaparthy/
├── subrepos          # Git remotes for each project directory
├── llama2-c/
├── llm-c/
├── micrograd/
├── nanochat/
└── nanoGPT/
```

Each subdirectory has its own `README.md`, license, and setup instructions. Follow those for installation and usage.

## Attribution

These projects are based on work by [karpathy (Andrej)](https://github.com/karpathy). Licenses for each project are included in its directory.
