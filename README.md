# DQN

In this notebook I implmented a Deep Q-Network (DQN) in Keras that plays "Airraid-V0" from Atari Games.

## Libraries

I used open AI gym to provide the environment wrapper (https://gym.openai.com/envs/AirRaid-v0/) and keras to implement the CNN architecture.

## Arhitecture

I used the architecture that was proposed by Mnih et al. 2013 in Playing Atari Games With Deep Reinforcement Learning.

The paper is available here : https://arxiv.org/abs/1312.5602

The first hidden layer convolves 16 8x8 filters with stride 4 with the input image and applies a rectifier nonlinearity (ReLU). The second
hidden layer convolves 32 4x4 filters with stride 2, again followed by a ReLU activation. The final hidden layer is fully-connected and consists of 256 rectifier units. The output layer is a fully-connected linear layer with a single output for each valid action (in our case 6).

## Future work

I need to work on hyper parameter-tuning and provide code for a demo.
