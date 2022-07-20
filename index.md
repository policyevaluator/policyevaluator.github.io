---
layout: default
---

## Abstract

Learning to evaluate and improve policies is a core problem of Reinforcement Learning (RL). 
Traditional RL algorithms learn a value function defined for a single policy. 
A recently explored competitive alternative is to learn a single value function for many policies. 
Here we combine the actor-critic architecture of Parameter-Based Value Functions and the policy embedding of Policy Evaluation Networks to learn a single value function for evaluating (and thus helping to improve) any policy represented by a deep neural network (NN). 
The method yields competitive experimental results. 
In continuous control problems with infinitely many states, our value function minimizes its prediction error by simultaneously learning a small set of  `probing states' and a mapping from actions produced in probing states to the policy's return. 
The method extracts crucial abstract knowledge about the environment in form of very few states sufficient to fully specify the behavior of many policies. 
A policy improves solely by changing actions in probing states, following the gradient of the value function's predictions.  
Surprisingly, it is possible to clone the behavior of a near-optimal policy in Swimmer-v3 and Hopper-v3 environments only by knowing how to act in 3 and 5 such learned states, respectively. 
Remarkably, our value function trained to evaluate NN policies is also invariant to changes of the policy architecture: we show that it allows for zero-shot learning of linear policies competitive with the best policy seen during training. 

## [Paper](https://arxiv.org/abs/2207.01566) 
## [Code](https://github.com/IDSIA/policyevaluator)


<br />

{% assign img_size = 95 %}

# Probing States Visualization
## Hopper
### Probing States of Untrained PSSVF
<img src="/assets/gifs/Hopper_untrained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_untrained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_untrained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_untrained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_untrained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

### Probing States of Trained PSSVF
<img src="/assets/gifs/Hopper_trained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_trained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_trained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_trained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Hopper_trained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

## Swimmer
### Probing States of Untrained PSSVF
<img src="/assets/gifs/Swimmer_untrained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_untrained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_untrained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_untrained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_untrained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

### Probing States of Trained PSSVF
<img src="/assets/gifs/Swimmer_trained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_trained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_trained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_trained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Swimmer_trained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

## HalfCheetah
### Probing States of Untrained PSSVF
<img src="/assets/gifs/HC_untrained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act5.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act6.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act7.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act8.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act9.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act10.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act11.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act12.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act13.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act14.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act15.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act16.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act17.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act18.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_untrained/videono_act19.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

### Probing States of Trained PSSVF
<img src="/assets/gifs/HC_trained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act5.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act6.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act7.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act8.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act9.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act10.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act11.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act12.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act13.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act14.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act15.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act16.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act17.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act18.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/HC_trained/videono_act19.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

## Ant
### Probing States of Untrained PSSVF
<img src="/assets/gifs/Ant_untrained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act5.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act6.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act7.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act8.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act9.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act10.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act11.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act12.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act13.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act14.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act15.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act16.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act17.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act18.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act19.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act20.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act21.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act22.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act23.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act24.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act25.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act26.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act27.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act28.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act29.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act30.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act31.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act32.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act33.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act34.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act35.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act36.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act37.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act38.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_untrained/videono_act39.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

### Probing States of Trained PSSVF
<img src="/assets/gifs/Ant_trained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act5.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act6.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act7.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act8.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act9.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act10.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act11.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act12.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act13.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act14.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act15.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act16.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act17.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act18.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act19.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act20.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act21.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act22.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act23.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act24.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act25.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act26.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act27.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act28.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act29.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act30.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act31.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act32.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act33.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act34.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act35.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act36.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act37.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act38.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Ant_trained/videono_act39.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

## Walker2d
### Probing States of Untrained PSSVF
<img src="/assets/gifs/Walker_untrained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act5.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act6.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act7.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act8.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act9.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act10.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act11.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act12.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act13.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act14.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act15.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act16.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act17.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act18.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act19.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act20.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act21.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act22.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act23.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act24.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act25.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act26.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act27.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act28.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act29.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act30.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act31.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act32.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act33.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act34.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act35.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act36.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act37.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act38.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act39.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act40.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act41.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act42.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act43.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act44.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act45.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act46.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act47.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act48.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_untrained/videono_act49.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

### Probing States of Trained PSSVF
<img src="/assets/gifs/Walker_trained/videono_act0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act5.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act6.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act7.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act8.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act9.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act10.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act11.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act12.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act13.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act14.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act15.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act16.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act17.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act18.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act19.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act20.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act21.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act22.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act23.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act24.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act25.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act26.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act27.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act28.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act29.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act30.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act31.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act32.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act33.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act34.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act35.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act36.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act37.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act38.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act39.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act40.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act41.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act42.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act43.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act44.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act45.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act46.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act47.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act48.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/Walker_trained/videono_act49.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">



