# Reinforcement Learning in Generative AI Tutorial (Python)

Here I show you reinforcement learning (RL) examples to train (fine-tune) **language models** (LM).

All these examples are implemented from scratch (manually) in a step-by-step manner (&ast;1), and also shows you theoretical aspects behind this implementation in IPython notebook.<br>
All these examples use a small language model with only 135M parameters, and you can then experiment on a signle small GPU (&ast;2).

- [RLHF (with PPO)](./01-rlhf-ppo.ipynb)
- [DPO](./02-dpo.ipynb) (&ast;3)
- [GRPO](./03-grpo.ipynb) (critic-free RL)

If you're not familiar with reinforcement learning (RL), please see [reinforcement learning tutorials](https://github.com/tsmatz/reinforcement-learning-tutorials) (&ast;4) for the outline of RL algorithms.

I hope that this repository helps you learn the fundamental for applying reinforcement learning in language models (i.e., applying Transformer Reinforcement Learning, TRL).

> Note (&ast;1) : In this repository, Hugging Face API is used to download pre-trained models, but the regular PyTorch training loop is manually applied. (I don't use any built-in training class in Hugging Face.)

> Note (&ast;2) : I have tested all examples on a single NVIDIA Tesla T4 (16 GB GPU memory).

> Note (&ast;3) : Strictly speaking, DPO is not a reinforcement learning method (i.e., RL-free algorithm). In this repository, however, I also treat DPO, because it's a widely-used method induced from reinforcement learning (RLHF) ideas.

> Note (&ast;4) : Especially, the following 4 contents in [reinforcement learning tutorials](https://github.com/tsmatz/reinforcement-learning-tutorials) will help to improve your understanding of RL theories behind examples.<br>
> Q-Learning, Policy Gradient, Actor Critic, PPO
