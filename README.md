# Controlling Backyard Flayer Drone with Python Script
This project is mainly used for controlling drone simulator. The project has the following main steps
1. Installing simulator
2. Install miniconda and the corresponding environment
3. running the script (backyard_flayer.py)

## 1. Installing the simulator
To run the backyard_flyer.py script, you might want to get setup with the Udacity drone simulator. to run backyard_flyer.py script you should hold this simulator **running**.

### Download and Installation
You can download the simulator [[here]](https://github.com/udacity/FCND-Simulator-Releases/releases).
Once you've downloaded the latest release, unzip the file and open the simulator by double-clicking on the app/executable.

![](https://github.com/mohandesosama/Backyard-Flayer/blob/master/docs/screen-shot-2018-01-19-at-2.41.57-pm.png)

### Arming
Arming implies that the power is now being supplied to the motors and the drone is ready to fly. Think of it like using your keys to start your car before you hit the gas! You always need to arm your drone first before you begin to fly. Once you click on arming, you'll notice that the propellers start to spin. And once you click Disarm, the motors stop. Remember to always `Arm` your drone before you can fly and `Disarm` the drone when not flying it.

### Manual vs Guided
As the name suggests, when you are flying the drone in Manual mode, you are the pilot. If it's a real drone, then you'll be using an RC controller. In the simulator, you can use your keyboard to fly the drone. Note that even in Manual mode, the drone is doing a lot of the work "autonomously" as it converts your high-level commands into rotor rotation rates.

Guided mode is used when you want the drone to perform tasks autonomously without any human control. You can do this either by sending commands to the drone via console or by writing a script to execute those commands depending on the mission requirements.

For this project, you'll be writing a program that will lead the drone to execute a mission. In order for the drone to run the mission on its own, it needs to be in Guided mode.

You can manually control the drone using the following key commands:
| Key(s)	| Control |
|---------|---------|
|W/S	|move forward / back|
|A/D	|move left / right|
|Q/E	|turn left/ right|

