# Baxter-project-1

## Introduction

This is my first Baxter project! It is also a course project of ME570 Robot Motion Planning. 

In this project, My classmate Wen and I describe a visual servoing control method enhanced by an obstacle avoidance strategy 
using  potential based function. The solution require both relative bearing measurements and relative distance measurements, 
which  acquire from the RGB-camera by color-based detection method through OpenCV. This property allows us to reduce the 
dependence  on the relative distance measurements, which are relatively more inaccurate compared with relative bearing 
measurements in most cases. Eye-in-hand sensor arrangement can provide a relative high accuracy and avoid vision collision. 
We also validate our approach by implementation on the Baxter robot.

## Feature

This project can be viewed as an online plane tracking and can be suddivided into vision and motion parts.
