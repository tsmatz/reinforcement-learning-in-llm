# Reinforcement Learning in LLM Tutorial (Python)

Here I show you reinforcement learning (RL) examples to train (fine-tune) **language models** (LM).

All these examples are implemented from scratch (manually) in a step-by-step manner (&ast;1), and also shows you theoretical aspects behind this implementation in IPython notebook.<br>
All these examples also work on a signle GPU with small footprint (&ast;2).

- [RLHF (with PPO)](./01-rlhf-ppo.ipynb)
- [DPO](./02-dpo.ipynb) (&ast;3)
- [GRPO](./03-grpo.ipynb) (critic-free RL)

If you're not familiar with reinforcement learning, please see [reinforcement learning tutorials](https://github.com/tsmatz/reinforcement-learning-tutorials) (&ast;4) for the outline of reinforcement learning (RL) algorithms.

These examples are not for "large" language model, but small language model. But this repository would be sufficient to help you learn the fundamental of applying reinforcement learning in language models (i.e., Transformer Reinforcement Learning, TRL).

> Note (&ast;1) : In this repository, Hugging Face API is used to download pre-trained models, but the regular PyTorch training loop is manually applied. (I don't use any built-in training class in Hugging Face.)

> Note (&ast;2) : I have experimented all examples on a single NVIDIA Tesla T4 (16 GB GPU memory).

> Note (&ast;3) : Strictly speaking, DPO is not a reinforcement learning method (RL-free algorithm), because it doesn't use any reward functions. In this repository, however, I also treat DPO, because it's a widely-used method induced from reinforcement learning (RLHF) ideas.

> Note (&ast;4) : Especially, the following 4 contents in [reinforcement learning tutorials](https://github.com/tsmatz/reinforcement-learning-tutorials) will help to improve your understanding of RL theories behind examples.<br>
> Q-Learning, Policy Gradient, Actor Critic, PPO
