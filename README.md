# fly_bird_RL

使用深度学习算法 DQN 来玩 flappy bird

# 安装依赖
pip install parl == 1.3.1

pip install pygame

pip install paddlepaddle

# 模拟环境 PLE 库
(PyGame-Learning-Environment)[https://github.com/ntasfi/PyGame-Learning-Environment]

# 模型简介

使用了 百度 PARL 深度学习库直接调用 DQN 算法

由于游戏的 state 仅有 8 维，所以模型网络仅使用了 2 个全连接层

# 收敛情况

在训练了 1000 个 episode 以后可以明显看出在逐步收敛

在训练了 10000 个 episode 以后，测试中基本可以保持一直进行下去，所以不得不限制到达一定分数就终止游戏

# 参数调整心得

需要保持较高的探索概率，30%-20%较佳

