# Install MuJoCo Pixel #


(1) Install MuJoCo 1.3.1

wget https://www.roboti.us/download/mjpro131_linux.zip;
unzip mjpro131_linux.zip;
cp -r mjpro131 ~/.mujoco/;

export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/home/danny/.mujoco/mjpro131/bin

pip install mujoco-py==0.5.7;

(2) Install this gym:

pip install -e .



#########
Usage:

xvfb-run -s "-screen 0 1400x900x24" bash;
python
###########################################
import gym
env = gym.make('HalfCheetahPixel-v1')
state = env.reset()  # should be 84x84x4 for now

 

