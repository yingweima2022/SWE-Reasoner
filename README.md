# SWE-Reasoner

## Overview

**SWE-Reasoner**:  is an open-source large language model specifically designed for software improvement. Built upon the foundation of the Qwen series base models, SWE-Reasoner has undergone additional LongCoT training using software engineering development process data to enhance its capabilities in solving complex software engineering tasks.

**SWESynInfer+**: four-stage software engineering process data synthesis and inference workflow. SWE-SynInfer divides the issue resolution process into three steps: (1) repository understanding to identify relevant codebase files, (2) fault localization to pinpoint problematic code segments, and (3) patch generation to produce candidate code edits. We extend this framework to include a Patch Verification phase, following Agentless, and call it SWE-SynInfer+.

## Model Performance

SWE-Reasoner has demonstrated impressive performance in software engineering tasks:

- 🌟 Achieved a **37.60% (32B) solution rate on the authoritative SWE-bench Verified** leaderboard for software engineering intelligent agents.
- 🌟 When combined with External TTC (budget=8), our model’s performance further **increases to 46.0%**.

## Model Link
https://modelscope.cn/models/Lingma/SWE-Reasoner

## Training data
We have provided the training data for SWE-Reasoner in the **training_data/**.

## Quick Start

Code is coming soon.

## Citation

@misc{ma2025thinkinglongerlargerenhancing,
      title={Thinking Longer, Not Larger: Enhancing Software Engineering Agents via Scaling Test-Time Compute}, 
      author={Yingwei Ma and Binhua Li and Yihong Dong and Xue Jiang and Rongyu Cao and Jue Chen and Fei Huang and Yongbin Li},
      year={2025},
      eprint={2503.23803},
      archivePrefix={arXiv},
      primaryClass={cs.SE},
      url={https://arxiv.org/abs/2503.23803}, 
}

## Acknowledgments

We would also like to thank the [SWE-bench](https://github.com/princeton-nlp/SWE-bench), [AutoCodeRover](https://github.com/nus-apr/auto-code-rover), [SWESynInfer](https://github.com/LingmaTongyi/Lingma-SWE-GPT), [SWE-Gym](https://github.com/SWE-Gym/SWE-Gym), [Nebius](https://huggingface.co/datasets/nebius/SWE-bench-extra), [SWE-fixer](https://github.com/InternLM/SWE-Fixer), [SWE-RL](https://github.com/facebookresearch/swe-rl) and [Agentless](https://github.com/OpenAutoCoder/Agentless) teams for their foundational work, which played an important role in the development of SWESynInfer+.
