# jax-rl

A base Dockerfile containing all the required dependencies for running my RL experiments with JAX.

Includes:

-   Python@3.10
-   CUDA & cuDNN for GPU acceleration
-   JAX and [jaxtyping](https://github.com/google/jaxtyping).
-   DeepMind's [Haiku](https://github.com/deepmind/dm-haiku), [Optax](https://github.com/deepmind/optax), [RLax](https://github.com/deepmind/rlax), [chex](https://github.com/deepmind/chex) and [Distrax](https://github.com/deepmind/chex).
-   [Weights&Biases](https://wandb.ai) and [tensorboardX](https://github.com/lanpa/tensorboardX) for logging.
