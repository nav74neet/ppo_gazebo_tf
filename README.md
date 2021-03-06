# ppo_gazebo_tf
Reinforcement Learning for solving the custom **cartpole** balance problem in **gazebo environment** using **Proximal Policy Optimization(PPO)**. [Note: this repo is under development]

### Environment
- Custom cartpole in gazebo (similar to the one from OpenAI gym)
- Observation Space: 4 (<strong>continuos</strong>)
- Action Space: 2 (<strong>discrete</strong>) 

### Dependencies

- <b><a href="http://releases.ubuntu.com/16.04/">Ubuntu 16.04</a></b> 
- <b><a href="http://wiki.ros.org/kinetic">ROS Kinetic</a></b>
- <b><a href="http://gazebosim.org/">Gazebo 7</a></b>
- <b><a href="https://www.tensorflow.org/">TensorFlow: 1.1.0</a></b> 
- <b><a href="https://github.com/openai/gym">gym: 0.9.3</a></b>
- <b>Python 3.6</b>

### File setup:
- **cartpole_gazebo** contains the robot model(both **.stl** files & **.urdf** file) and also the ***gazebo launch file***.

- **cartpole_controller** contains the reinforcement learning implementation of ****Proximal Policy Optimization(PPO)**** for custom cartpole environment.

### Training Phase:
```
python3 ppo_train.py
```
<p align= "center">
  <img src="cartpole-gazebo-ppo/cartpole_gazebo/gifs/ppo_training.gif" width="300" height="300">
</p>

### Testing trained policy:
```
python3 ppo_test.py
```
### References:
- <b><a href="https://blog.openai.com/openai-baselines-ppo/">Proximal Policy Optimization by OpenAI</a></b> 
- <b><a href="https://github.com/uidilr/ppo_tf">PPO implementation using TensorFlow</a></b>

### TODO:
- Use Tensorboard for plotting the training and testing graphs. 

## Project collaborator(s): 
**<a href="https://github.com/ioarun">Arun Kumar</a>** (arunkumar12@iisc.ac.in)


