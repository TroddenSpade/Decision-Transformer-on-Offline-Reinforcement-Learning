# Decision Transformer on Offline Reinforcement Learning

This repository includes Decision Transformer, Conservative Q-Learning, and Behavior cloning implementations on OpenAI Gym's MuJoCo environments. Instead of training a policy through conventional Reinforcement Learning Algorithms, models are trained on collected experiences recorded by an expert player based on Offline Reinforcement Learning setting. In Offline RL, unlike the traditional RL in which data are obtained via interactions with environments, the policy has only access to a limited dataset consisting of trajectory rollouts. This setting restricts the agent's ability by preventing them from exploring the environment and obtaining feedback; however, the Offline RL approaches depicted successful results despite those difficulties. 

## Requirements

* PyTorch
* OpenAI Gym
* [D4RL](https://github.com/Farama-Foundation/D4RL)
* [Hugging Face Transformers](https://github.com/huggingface/transformers) (GPT-2 Model)

## Contents
  - [x] Behavior Cloning (BC)
  - [x] Decision Transformer
  - [ ] GPT-2
  - [x] Soft Actor-Critic (SAC)
  - [x] Conseravtive Q-Learning (CQL)
  
## Experiments
### HalfCheetah-v3 Environment

#### Behavior Cloning

https://user-images.githubusercontent.com/33734646/190910946-5e885c8e-cb0d-4e0f-8f1c-0940305a6971.mp4

#### Conservative Q-Learning

Trained the model for 1M iterations and for each iteration a batch of 256 rollouts were sampled.

![HC-CQL](https://github.com/TroddenSpade/Decision-Transformer-on-Offline-Reinforcement-Learning/blob/main/assets/HC-CQL.png?raw=true)

https://user-images.githubusercontent.com/33734646/193818250-0f772f50-7801-47b3-bf46-d5025961b71a.mp4

#### Decision Transformer

https://user-images.githubusercontent.com/33734646/190910960-275cdfc8-5669-4413-9d6d-bb1a3bf03012.mp4


### Hopper-v2 Environment

#### Behavior Cloning

https://user-images.githubusercontent.com/33734646/190911324-19f988e3-a565-4941-afac-98038dda0057.mp4

#### Conservative Q-Learning

Trained the model for 1M iterations and for each iteration a batch of 256 rollouts were sampled.

![H-CQL](https://github.com/TroddenSpade/Decision-Transformer-on-Offline-Reinforcement-Learning/blob/main/assets/H-CQL.png?raw=true)

https://user-images.githubusercontent.com/33734646/193813226-6a9ffff7-918c-45fc-bec3-9258396c2278.mp4

#### Decision Transformer

https://user-images.githubusercontent.com/33734646/190912391-68f80548-8825-4526-9473-24d41c0be286.mp4


### Walker-v2 Environment

#### Behavior Cloning

https://user-images.githubusercontent.com/33734646/190911092-ecd330f5-d71f-44f4-8b59-bc3bbe465f4f.mp4

#### Conservative Q-Learning

Trained the model for 1M iterations and for each iteration a batch of 256 rollouts were sampled.

![W-CQL](https://github.com/TroddenSpade/Decision-Transformer-on-Offline-Reinforcement-Learning/blob/main/assets/W-CQL.png?raw=true)

https://user-images.githubusercontent.com/33734646/194069972-0080de45-14a9-44be-aac5-d1b804f30d6c.mp4

#### Decision Transformer

https://user-images.githubusercontent.com/33734646/190911220-72eb4bf6-43c6-4aef-af65-3d9cda0882de.mp4


## References

1. Lili Chen, Kevin Lu, Aravind Rajeswaran, Kimin Lee, Aditya Grover, Michael Laskin, Pieter Abbeel, Aravind Srinivas, Igor Mordatch. Decision Transformer: Reinforcement Learning via Sequence Modeling. CoRR (2021). [ArXiv](https://arxiv.org/abs/2106.01345)
2. Aviral Kumar, Aurick Zhou, George Tucker, Sergey Levine. Conservative Q-Learning for Offline Reinforcement Learning. [ArXiv](https://arxiv.org/abs/2006.04779)
3. D4RL: Datasets for Deep Data-Driven Reinforcement Learning. Justin Fu and Aviral Kumar and Ofir Nachum and George Tucker and Sergey Levine. 2020.
4. [Hugging Face Transformers](https://github.com/huggingface/transformers)
5. [Edward Beeching's Gym Replays](https://huggingface.co/datasets/edbeeching/decision_transformer_gym_replay)
6. [CleanRL](https://github.com/vwxyzjn/cleanrl) and the authors' [Study Group](https://youtu.be/AjudkPZKIr4)
