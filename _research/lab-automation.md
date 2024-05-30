---
title: "Lab Automation"
layout: single-portfolio
excerpt: "<img src='/images/research/maholo_mini.jpg' alt=''>"
category: Current Projects
collection: research
order_number: 2
header: 
  og_image: 
---

The following constitutes one of the [two projects](/research/lab-automation){: target="_blank"} I am currently working on as a postdoctoral researcher at the [Saito Laboratory](https://www.ytksailab.org){: target="_blank"} at Tokyo, Japan, in the field of [Laboratory Automation](https://en.wikipedia.org/wiki/Laboratory_automation){: target="_blank"}.

Laboratory automation is a field that focuses on using technology to automate biological experiments. It involves integrating robotics, software, and advanced instrumentation to perform repetitive tasks. The automation of these tasks allows to enhance experimental consistency, reduce human errors, accelerate research processes, and allows scientists to focus on more complex analytical tasks. Especially, as mentioned in my [second](/research/lab-automation){: target="_blank"} and related postdoctoral project, the field of protein engineering seeks to develop new and improved protein for various applications, such as medicines and vaccines. However, It requires multiple experiments and their automation would enable high-throughput screening and analysis of new protein.

Laboratory automation has already demonstrated its effectiveness when the tasks to automate are fixed, relatively simple, or with little variability. However, when complex experiments need to be designed, automation is still possible but usually relies on robot programation that requires expert knowledge. One example is the robots in the following pictures, that is able to reproduce human movements using two independent arms, but that also involves precise movements configuration and in the right order. Complex experiments therefore increases programation time, during which the robots cannot be used for other experiments.

![](/images/research/maholo.jpg)

In my postdoctoral research, I work with this type of human-like robot and seek to integrate artificial intelligence algorithm to ease the programation and the design of new biological experiments. By doing so, each arm trajectory is not the result of a long and tedious robot arms trajectory refinement, but is inferred from a predictive model that finds the best arms trajectory to apply, in a given situation. More precisely, the model is a Reinforcement Learning model, which learns with trials an errors up until it has learned to effectively infer good trajectories. However, training this type of model within the real world and with the real robot not does not only take times -- to face it with large and varied situations -- but can also cause damage to the physical environment when it is not trained yet. So, the robot is actually trained in a simulated environment, called a [digital twin](https://en.wikipedia.org/wiki/Digital_twin){: target="_blank"}, that precisely reproduces the robot itself and the element it interacts with, so that it can be trained faster and without risks of damages. However, no simulated environment perfectly matches the real world. So, the challenge lies on how the knowledge acquired from the digital twin should be transferred to the real robot without loosing in performances. This can involve several related fields, such as [transfer learning](https://en.wikipedia.org/wiki/Transfer_learning) or [domain adaptation](https://en.wikipedia.org/wiki/Domain_adaptation), to name a few.

