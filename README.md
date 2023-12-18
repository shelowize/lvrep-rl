# Representation-based Reinforcement Learning
This repo contains implementations for RL with:
- Latent Variable Representations (LV), as outlined in [1].
- Contrastive Representations (CTRL), as described in [2].

## Directory
- `agent` hosts implementation files for various agents, including the Soft Actor-Critic baseline (`sac`), SAC with Latent Variable (`vlsac`), and SAC with Contrastive Representations (`ctrlsac`).
- `networks` contains base implementations for critics, policy networks, variational autoencoders (VAE), and more.
- `utils` comprises replay buffers and several auxiliary functions.

## Run
Execute the `main.py` script with your preferred arguments, such as `--alg` for algorithm type, `--env` for environment, and so on.

Example usage: `python main.py --alg vlsac --env HalfCheetah-v3`.

## References
[1] Ren, T., Xiao, C., Zhang, T., et al. 2022. Latent Variable Representation for Reinforcement Learning. arXiv.

[2] Zhang, T., Ren, T., Yang, M., Gonzalez, J.E., Schuurmans, D., and Dai, B. 2022. Making Linear MDPs Practical via Contrastive Representation Learning. arXiv.
