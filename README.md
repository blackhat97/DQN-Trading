# DQN-Trading

심층 강화 학습을 통한 주식 거래 시장 OpenAI GYM 환경


## Requirements

- Python2.7 or higher
- Numpy
- HDF5
- Keras with Beckend (Theano or/and Tensorflow)
- OpenAI Gym

## Usage

Note that the most sample training data in this repo is Korean stock. 
You may need to re-download your own training data to fit your purpose.

After meet those requirements in above, you can begin the training both algorithms, Deep Q-learning and Policy Gradient.

Train Deep Q-learning:

    $ python market_dqn.py <list filename> [model filename]

Train Policy Gradient:

	$ python market_pg.py <list filename> [model filename]

For example, you can do like this:

	$ python market_pg.py ./kospi_10.csv pg.h5

Aware that the provided neural network architecture in this repo is too small to learn.
So, it may under-fitting if you try to learn every stock data.


## Reference

[1] [Playing Atari with Deep Reinforcement Learning](http://arxiv.org/abs/1312.5602)  
[2] [Deep Reinforcement Learning: Pong from Pixels](http://karpathy.github.io/2016/05/31/rl/)  
[3] [KEras Reinforcement Learning gYM agents, KeRLym](https://github.com/osh/kerlym)  
[4] [Keras plays catch, a single file Reinforcement Learning example](http://edersantana.github.io/articles/keras_rl/)
