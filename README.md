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

Try using these controls to take off, fly in a square shape, and then land.

## 2. Installing miniconda and environment
Before you can program flight plans for the simulator, there's a bit of setup that's required first.

You are welcome to skip this section if you are taking the free preview and do not want to command the drone with Python code or complete the Backyard Flyer project.

### Setup Instructions 
Read through the instructions below. If these commands look familiar to you, then you should use these VERY abbreviated instructions to get yourself set up.

* download [miniconda](https://conda.io/miniconda.html) and then install by opening the file/app that you download.

* `conda env create -f environment.yml` to create the miniconda environment: this took me 20 minutes to run due to the large number of installs required.

* `source activate fcnd` to activate the environment (you'll need to do this whenever you want to work in this environment).

### NOTE: 
If the above command fails due to internet issues or timed out HTTP request then remove the partially built environment using the following command (then run the above create command again):

`conda env remove -n fcnd`
Verify that the FCND (listed fcnd) environment was created in your environments:

`conda info --envs`
Cleanup downloaded libraries (remove tarballs, zip files, etc):

`conda clean -tp`

## 3. Running the backyard_flyer.py script
* run the Drone simulator 
* Open miniconda and make sure you are on the fcnd enviroment by using 
`$ source activate fcnd`
or
`$ activate fcnd`
* cd to the folder of the project. 
* run `python backyard_flyer.py`
It is expected that the drone will fly in square and then return back to its initial position. 

Regards
Osama Hosameldeen

