### Observations
- DQN showed higher variance across episodes.
- PPO learning was smoother and more stable.
- PPO required less manual tuning.
- DQN performance fluctuated more during training.

This project compares the performance of Deep Q-Network (DQN) and Proximal Policy Optimization (PPO) 
on the CartPole-v1 environment.
Both algorithms were trained under similar conditions and 
evaluated using the same metric: average episodic reward over multiple evaluation episodes.
DQN, a value-based method, was able to learn the task but showed higher variance in performance and
 greater sensitivity to hyperparameter tuning.
Exploration relied on an epsilon-greedy strategy, which occasionally led to unstable behavior.
PPO, a policy-based Actor–Critic method, demonstrated smoother and more stable learning.
The clipped policy objective prevented large policy updates, resulting in more consistent performance across episodes.
This comparison illustrates the practical trade-offs between value-based and policy-based reinforcement learning approaches.
 While DQN is effective for simple discrete tasks, PPO provides greater stability and scalability, making it a preferred choice for more complex environments.

Files included:
cartpole_dqn.ipynb – DQN implementation
cartpole_ppo.ipynb – PPO implementation
cartpole_comparison.ipynb – evaluation and analysis notebook