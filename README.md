# Decision Transformer on Offline Reinforcement Learning

This repository includes Decision Transformer, Conservative Q-Learning, and Behavior cloning implementations on OpenAI Gym's MuJoCo environments. Instead of training a policy through conventional Reinforcement Learning Algorithms, models are trained on collected experiences recorded by an expert player based on Offline Reinforcement Learning setting. In Offline RL, unlike the traditional RL in which data are obtained via interactions with environments, the policy has only access to a limited dataset consisting of trajectory rollouts. This setting restricts the agent's ability by preventing them from exploring the environment and obtaining feedback; however, the Offline RL approaches depicted successful results despite those difficulties. 

## Requirements

* PyTorch
* OpenAI Gym
* Hugging Face Transformers (GPT-2 Model)

## Contents
  - [x] Behavior Cloning (BC)
  - [x] Decision Transformer
  - [ ] GPT-2
  - [ ] Conseravtive Q-Learning (CQL)
  
## Experiments
### HalfCheetah-v3 Environment

* Behavior Cloning

https://user-images.githubusercontent.com/33734646/190910946-5e885c8e-cb0d-4e0f-8f1c-0940305a6971.mp4

* Decision Transformer

https://user-images.githubusercontent.com/33734646/190910960-275cdfc8-5669-4413-9d6d-bb1a3bf03012.mp4



### Hopper-v2 Environment

* Behavior Cloning


https://user-images.githubusercontent.com/33734646/190911324-19f988e3-a565-4941-afac-98038dda0057.mp4


* Decision Transformer


https://user-images.githubusercontent.com/33734646/190912391-68f80548-8825-4526-9473-24d41c0be286.mp4



### Walker-v2 Environment

* Behavior Cloning

https://user-images.githubusercontent.com/33734646/190911092-ecd330f5-d71f-44f4-8b59-bc3bbe465f4f.mp4

* Decision Transformer


https://user-images.githubusercontent.com/33734646/190911220-72eb4bf6-43c6-4aef-af65-3d9cda0882de.mp4



## References

1. Lili Chen, Kevin Lu, Aravind Rajeswaran, Kimin Lee, Aditya Grover, Michael Laskin, Pieter Abbeel, Aravind Srinivas, Igor Mordatch. Decision Transformer: Reinforcement Learning via Sequence Modeling. CoRR (2021). [ArXiv](https://arxiv.org/abs/2106.01345)
2. Aviral Kumar1, Aurick Zhou1, George Tucker2, Sergey Levine. Conservative Q-Learning for Offline Reinforcement Learning. [ArXiv](https://arxiv.org/abs/2006.04779)
3. [Hugging Face Transformers](https://github.com/huggingface/transformers)
4. [Edward Beeching's Gym Replays](https://huggingface.co/datasets/edbeeching/decision_transformer_gym_replay)
