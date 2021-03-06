# Baxter-project-1

<p align="center">
<img src="https://github.com/zhouyuan7/Baxter-project-1/blob/master/gif/baxter_project_1_gif_3.gif"/>
</p>

## Introduction

This is my first Baxter project! It is also a course project of ME570 Robot Motion Planning from Boston University. The propose of this project is tracing a target tennis ball on a plane using Baxter robot arm. 

This is a robot arm on-line plane tracking project, which in detail can be divided into vision and motion parts. For vision part, using Baxter arm camera recognizes a tennis target through openCV color detection method and with given depth information,  convert the target camera view frame location to the Baxter coordinate system.  

![alt text](https://github.com/zhouyuan7/Baxter-project-1/blob/master/gif/paper_final.jpg)
<p align="center">
color detector results
</p>

For the motion part, after received the target X-Y location in Baxter coordinate. We set start position from Baxter ros message '/endpoint_pose' and use a potential based function to generate a plane vector as a control signal. Use Baxter default IK solver service and joint move API to control the robot arm in configuration space.

## Report Abstract

In this project, my classmate Wen and I describe a visual servoing control method enhanced by an obstacle avoidance strategy 
using  potential based function. The solution requires both relative bearing measurements and relative distance measurements, 
which  acquire from the RGB-camera by color-based detection method through OpenCV. This property allows us to reduce the 
dependence  on the relative distance measurements, which are relatively more inaccurate compared with relative bearing 
measurements in most cases. Eye-in-hand sensor arrangement can provide a relative high accuracy and avoid vision collision. 
We also validate our approach by implementation on the Baxter robot.


## More Videos

<p align="center">
<img src="https://github.com/zhouyuan7/Baxter-project-1/blob/master/gif/baxter_project_1_gif_1.gif"/>
</p>

<p align="center">
<img src="https://github.com/zhouyuan7/Baxter-project-1/blob/master/gif/baxter_project_1_gif_2.gif"/>
</p>
