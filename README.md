# cs
**TO GET THIS SOLUTION VISIT:** [CS](https://mantutor.com/product/cs/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116147&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
The purpose of this first project is to help you learn the basics of how to operate individual robots with various levels of accuracy, and to stress the knowledge you have acquired during the first few lectures (from introduction to low-level/mid-level designs).

The GRITSBot is controlled using unicycle dynamics,

𝑢 = # 𝜔𝑣’ = ( 𝑥𝜃̇+̇ –

where 𝜃 is the angle of the body frame of the robot with respect to the frame defined on the testbed. The units of the velocity inputs 𝑣 and 𝜔 are m/s and rad/s respectively.

Figure 1. The GRITSBot X (the bigger one on the left).

Figure 2. Drawing of the arena.

An overhead sensor is used to return pose data for the robot,

𝑥

𝑝 = /𝑦 1.

𝜃

The position coordinates (x, y) are given in meters and 𝜃 is in radians, with a range of [-pi, pi].

The Robotarium simulator, along with more information on the GRITSBot X and

testbed can be found on the Robotarium website

(https://www.robotarium.gatech.edu/faq).

Modeling the Kinematics of the Robots

1. Learn how to perform basic operations on the robots (e.g. move from base to a point with a given orientation, return to a base point etc.) on the Robotarium simulation.

a. Find out the equation describing the relationship between the rpm of the wheels, 𝜔wheel, and the forward velocity of the robot, v, with the given parameters. The radius of the wheels is 1.5cm.

b. Find out the relationship between the translational velocity of the wheels, vwheel, and the angular velocity of the robot, 𝜔, assuming the wheels are rotating in opposite directions and with the same speed.

2. Describe the feedback control loop for controlling the orientation, 𝜃, of the robots along a path used in the Robotarium using a block diagram. That is, a desired orientation is commanded and thus should be your input. Make sure to start with the input and end with the output in order to have a complete diagram.

This could be helpful: https://en.wikipedia.org/wiki/Control_theory

Make sure to label each block as sensor/controller/actuator and label on each line what variable is passed to the next block. An open loop block diagram of the robot is like this:

3. Give brief descriptions of the sensor, actuator and controller. What do they do? Relate these components to the actual relevant functions in the code.

Simulation Activities

Note: Do NOT use any pre-defined functions in the Robotarium simulator (/ examples and /utilities).

Prepare a script for your robot to do the following list of tasks:

1. Open the file, Template_Project_1.py, which contains two 3×1 pose vectors (i.e. [𝑥; 𝑦; 𝜃]) with the names target1 and target2.

2. Command one robot to target1.

3. Once Task 2 is completed, command the robot to target2, with constant velocity 8 cm/s and no angular velocity (open loop control). This can be done by first pointing the robot to a desired direction at its current location, and then calculating the theoretical number of iterations needed to reach target2 at the given speed. The controller is running at 30 Hz (i.e. one iteration corresponds to about 0.033 seconds).

4. Command the robot to target1.

5. Command the robot to target2 with constant 8 cm/s and a feedback strategy where the angular velocity is adjusted (closed loop control) based on the angular deviation from the direction to the target position. Stop the experiment when the robot reaches the target position, within 1 cm and 0.1 radian accuracy. The feedback strategy can be expressed like the following:

𝜔 = 𝑘(𝜃789:;87 − 𝜃=&gt;;;8?@),

where k is a gain value of 1.

6. Command the robot to target1.

Submit Your Experiment

Once you are satisfied with the simulation, submit the script,

Template_Project_1.py, to the Robotarium through your account. Data will be accessible in several days.

Data Analysis

1. Plot the experimental position data of Task 3 and Task 5 on the same Y vs X plot.

2. Plot the distance to the target position of Task 3 and Task 5 against the number of iterations (normalized from 0) on the same plot.

3. Discuss and explain what you see in the plots.

Report and Grading

All the tasks are accomplished by the robot. (50 pts)

In your report, please do the following:

1. Answer the 3 questions in the Modeling section. (30 pts)

2. Indicate the theoretical number of iterations needed in Simulation Task 3. (5 pts)

3. Include 2 plots and the discussion from the Data Analysis section. (15 pts)

Submissions

P1 Attempt 1 &amp; 2: The simulation .mat file (renamed simulation.mat) and source .py file from your simulation. From robotarium your public experiment link and .mat file (renamed experiment.mat) all submitted to Canvas.

*P1 Attempt 2 is optional if you do not like your score or need to make modifications to your P1 Attempt 1. The best of the two scores will be used.

Python Installation

Python is restricted to 3.5.x+

https://github.com/robotarium/robotarium_python_simulator
