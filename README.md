# cartpole
Balancing cartpole using PPO and DQN

This repository contains my experiments with reinforcement learning on the CartPole-v1 environment, focusing on understanding and comparing value-based and policy-based methods using DQN and PPO.

I first trained a DQN agent to get a baseline understanding of how a value-based algorithm learns to solve CartPole. The agent was trained for a fixed number of timesteps and evaluated using a deterministic policy. While the DQN agent was able to learn the task and balance the pole for a reasonable duration, its performance varied noticeably across episodes. Some runs showed stable behavior, while others terminated early, highlighting the sensitivity of DQN to exploration strategy and hyperparameter choices even in a simple environment.

After working with DQN, I implemented PPO on the same CartPole environment to study a policy-based approach. PPO uses an actor–critic architecture and applies clipped policy updates to ensure stable learning. Compared to DQN, PPO exhibited smoother learning behavior and more consistent episode lengths during evaluation. The stochastic policy helped with exploration without relying on epsilon-greedy methods, and overall training felt more stable.

Finally, I compared both algorithms using average episodic reward over multiple evaluation episodes. While both DQN and PPO were capable of solving CartPole, PPO generally showed lower variance and more reliable performance. DQN required more careful tuning and showed higher fluctuations in reward, whereas PPO was less sensitive to hyperparameters and easier to train consistently. This comparison helped me clearly understand the practical trade-offs between value-based and policy-based reinforcement learning methods and why PPO is often preferred for stability in more complex tasks.

Through this project, I gained hands-on experience with training, evaluating, saving, and comparing reinforcement learning agents, as well as interpreting their behavior beyond just raw reward values.
I have seperately given my readme files in th folder for each and every algorithm implementation.
