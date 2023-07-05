# lvrep-rl

## Installation
[Miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html) is used to handle the environment dependencies.
Once miniconda is installed, the environment can be created and activated with the following commands:
`conda create --name <env_name>`
`conda activate <env_name>`
`conda install --file requirements.txt`

## Run the project
To run the project, the environment must be activated.
Then, the following command can be used:
`python main.py <--args=value>`
The list of arguments can be found in the `main.py` file and are described in the following section.

### Arguments

| Argument            | Description                              | Default value  |
| ------------------- | ---------------------------------------- | -------------- |
| alg                 | Name of the algorithm (sac, vlsac)       | sac            |
| batch_size          | Batch size for actor and critic          | 256            |
| dir                 | Dir number                               | 0              |
| discount            | Discount factor                          | 0.99           |
| env                 | Environment name                         | HalfCheetah-v3 |
| eval_freq           | How often (time steps) we evaluate       | 5000           |
| expl_noise          | Std of Gaussian exploration noise        | 0.1            |
| extra_feature_steps | Use extra feature steps                  | 3              |
| feature_dim         | Latent feature dimension                 | 256            |
| hidden_dim          | Network hidden dimensions                | 256            |
| learn_bonus         | Save model and optimizer parameters      | store_true     |
| max_timesteps       | Max time steps to run environment        | 1000000        |
| save_model          | Save model and optimizer parameters      | store_true     |
| seed                | Sets Gym, PyTorch and Numpy seeds        | 0              |
| start_timesteps     | Time steps initial random policy is used | 25000          |
| tau                 | Target network update rate               | 0.005          |