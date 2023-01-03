# Safe, efficient, and comfortable velocity control based on reinforcement learning for autonomous driving
Source code for paper:   
[Zhu, M., Wang, Y., Pu, Z., Hu, J., Wang, X., & Ke, R. (2020). Safe, efficient, and comfortable velocity control based on reinforcement learning for autonomous driving. Transportation Research Part C: Emerging Technologies, 117, 102662.](https://www.sciencedirect.com/science/article/pii/S0968090X20305775)

## Description
Use DDPG for car following velocity control. The key part is the design of reward function. If the reward is not properly designed, the vehicle will either has poor jerk performances or stop there with zero speed (in this case the jerk is zero). So the weights between different objectives are important.

## Data format
Each element (cell or matrix) in the trainSet.mat and testSet.mat describes a car-following event. For each matrix (event), the columns are spacing, following vehicle speed, relative speed, leading vehilce speed. Events may have different durations. 

## How to run
- Set up python environment by installing the required packages according to requirements.txt
- Directly run Main.ipynb
- simulation_env is the simulaition environment for car following
- MPC_acc is the MPC based ACC implementation. This is a baseline. 

## Citation 
```angular2html
@article{zhu2020safe,
  title={Safe, efficient, and comfortable velocity control based on reinforcement learning for autonomous driving},
  author={Zhu, Meixin and Wang, Yinhai and Pu, Ziyuan and Hu, Jingyun and Wang, Xuesong and Ke, Ruimin},
  journal={Transportation Research Part C: Emerging Technologies},
  volume={117},
  pages={102662},
  year={2020},
  publisher={Elsevier}
}
```
