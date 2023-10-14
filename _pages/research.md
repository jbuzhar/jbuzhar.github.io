---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

## Controlled density transport
The problem of controlling distributions of states has many applications, including uncertainty propagation and quantification, stochastic control and motion planning under uncertainty, controlled fluid transport, and control of distributed multiagent systems. In such problems, the distribution of states is modelled as a probability density function.  The animations below illustrate this idea on a Duffing system.  The left figure shows the time evolution of a single state in state space; the right figure shows the evolution of an ensemble of states, which are modelled as a probability density function. 

<video id="myBGvid" autoplay muted loop width="400" >
<source src="/files/duffing.mp4" type="video/mp4">
</video>
<video id="myBGvid" autoplay muted loop width="400" >
<source src="/files/duffing_densprop.mp4" type="video/mp4">
</video>

To model the time evolution of density functions, we use ideas from the operator-theoretic view of dynamical systems.  The Perron-Frobenius operator is the operator which propagates density functions forward in time under the flow of a dynamical system.  This operator is the adjoint of the Koopman operator, which propagates observable functions along trajectories of a dynamical system.  This relationship enables the use of data-driven methods, such as extended dynamic mode decomposition (EDMD) for constructing finite dimensional approximations of the operator.

For a controlled dynamical system, this method yields a high-dimensional bilinear system for the density evolution.  We solve an optimal control problem on this system to steer an initial distribution of states to a desired target.  As an application, we consider the problem of a rotor-driven Stokes flow, where the torques on a pair of micro-rotors are controlled to manipulate a blob of fluid particles toward a target, as shown below.  The plot on the right shows the optimal rotor torques of the left and right rotors over time. 

<div style="display: flex; align-items: center;">
  <video id="myBGvid" autoplay muted loop width="400">
    <source src="/files/rotlets_free_2f_5s_PF.mp4" type="video/mp4">
  </video>
  <img src="/files/gammscratch.png" alt="Rotor controls" width="400">
</div>

For more details, see the following paper: 
>Controlled density transport using Perron Frobenius generators \
>J. Buzhardt, P. Tallapragada. \
>IEEE Conference on Decision and Control, 2023. [Preprint](/files/cdc2023_bt.pdf) 


## Rolling, Jumping Robot
Littlewood's hopping hoop is a classic dynamics example, which consists of a lightweight hoop with a heavy eccentric mass.  This simple mechanism is known to exhibit a hopping behavior when rolled fast on flat ground or from rest on an incline, as shown in the video below. 
<div style="display: flex; align-items: center;">
  <video controls muted loop width="300">
    <source src="/files/PassiveHoop.mp4" type="video/mp4">
  </video> 
  <img src="/files/PassiveHoop.png" alt="Rotor controls" width="400">
  <img src="/files/HoopFBD_simple.png" alt="Rotor controls" width="200">
</div>

This hopping behaviour is due to a lifting effect on the hoop created by the large centripetal acceleration of the offset mass, as shown in the schematic above.  Inspired by this, we design a robot to roll and jump from flat ground by actuating a heavy pendulum at high speed in order to jump.  As shown in the video below, our robot is able to achieve vertical jumps of 2.4 body lengths.  
<video controls muted loop width="600" >
<source src="/files/vertonly.mp4" type="video/mp4">
</video>

Additionally, the robot can clear large horizontal distances while in air by achieving a high rolling velocity before initiating a jump.  As shown in the video below, the robot clears over 6 body lengths in air and is able to achieve multiple jumps with minimal recovery time.  
<video controls muted loop width="600" >
<source src="/files/horonly.mp4" type="video/mp4">
</video>

For more details, see the following papers:  
>A Pendulum-Driven Legless Rolling Jumping Robot\
>J. Buzhardt, P. Chivkula, P. Tallapragada. \
>IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), 2023 [Preprint](/files/IROS2023_bct.pdf) 

>A Passive Jumping Mechanism\
>P. Tallapragada, J. Buzhardt, R. Seney. \
> 2019 Dynamic Systems and Control Conference (DSCC) ASME. October 2019. [Paper Link](https://doi.org/10.1115/DSCC2019-9194) | [Preprint](/files/tbs_dscc2019.pdf)

## Low Reynolds number swimming
coming soon

## Offroad vehicle navigation
coming soon
