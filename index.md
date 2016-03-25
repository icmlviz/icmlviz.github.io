---
layout: default
---

# Workshop on Visualization for Deep Learning

## Organizers:

##### Biye Jiang (UC Berkeley, bjiang@berkeley.edu)
	
##### John Canny (UC Berkeley, canny@berkeley.edu)

##### Polo Chau (Georgia Tech, polo@gatech.edu)

##### Aditya Khosla (MIT, khosla@csail.mit.edu)

## Abstract##

Deep networks have had profound impact across machine learning research and in many application areas. DNNs are complex to design and train. They are non-linear systems that almost always have many local optima and are often sensitive to training parameter settings and initial state. Systematic optimization of structure and hyperparameters is possible e.g. with Bayesian optimization, but hampered by the expense of training each design on realistic datasets. Exploration is still ongoing for best design principles. We argue that visualization can play an essential role in understanding DNNs and in developing new design principles. With rich tools for visual exploration of networks during training and inference, one should be able to form closer ties between theory and practice: validating expected behaviors, and exposing the unexpected which can lead to new insights. Likely topics for the workshop include, but are not limited to:

## Topics:##

•	directly visualizing the activations and parameters in intuitive aggregates

•	visualizing weights as features

•	visualizing gradient aggregates during training

•	Improving interpretability of networks:

•	Localizing "responsbility" in the network for particular outputs

•	Sensitivity/stability of network behavior

•	visualizing loss function geometry and the trajectory of the gradient descent process

•	visual representation of the input-output mapping of the network

•	visualizing alternative structures and their performance

•	monitoring/debugging the training process, i.e to detect saddle points or local optima, saturation units

•	visualizing distributed training methods across a cluster

•	using animation in network visualization

•	interactive visualizations for exploration or parameter tuning

•	software architectures for effective visualization

•	visualization and interaction user interfaces



## Motivation##

Visualization has already proven its power to inform the design of DNNs. It was an essential part of Clarifai’s entry that won the ImageNet 2013 Classification Challenge [Zeiler 2014]. “Deconvnet”s are now a powerful tool in the toolbox for deep net design. Image-based nets are perhaps the most natural domain for visualization, but we believe it applies in many other domains. Here are some representative areas where better visualization could inform design:

### Structure Design:###
 
There are many potential pitfalls in DNNs, and visualization can help expose them. The “vanishing gradient” problem is an issue for RNNs, but quantifying its effects helps draw the line between potential and actual failure. Many intuitive metrics can be applied to the design of DNN layers, and visualizing these across the entire network can quickly help find the best structures. Some straightforward visualizations used in [Glorot 2010] already proved to be very useful. In contrast to black-box methods like Bayesian optimization, visualization helps discover why a particular structure is doing poorly, and potentially how to improve it. 

### Improving Interpretability of DNNs: ###

DNNs are powerful predictors under the chosen loss function on predictions. But it is notoriously difficult to infer more than the prediction itself. How confident is the prediction? How sensitive is it to the training data? What features are most important in the DNN’s output?  What are the most (visually) similar inputs and how do their outputs vary? What are the most similar inputs based on the networks’ feature maps? Visualization[Zeiler 2014, Karpathy 2015, Yosinski 2015] is critical for answering most of these questions. Also, several work [Zhu 2014, Mahendran 2015, Dosovitskiy 2015] have been focusing on generating images from the generative CNN models to interpret its internal behavior.
 
### Improving Hyperparameter Tuning:###

 DNNs are highly sensitive to hyperparameter settings, and well-tuned parameters can lead to orders-of-magnitude improvements in training efficiency. The optimal learning rates for complex networks are highly dynamic. In one study, training an image digit recognizer apparently followed a pattern of training the network in “waves” from last to first layer [Maclaurin 2015]. The graphs in that paper already suggest abstraction from that particular model to others. They also suggest various theoretical mechanisms for the optimal training trajectories. 

### Improving parallel training of DNNs: ###
Many DNN applications could leverage much larger training data than is practical today. Training is likely to be much more distributed in future, and more complicated: basic SGD does not scale, and does not use the potential of the cluster to explore the parameter space. We believe that parallel MCMC methods will be very important in future, but in any case, optimization of any distributed training process[Zhang 2015] is much more challenging than on a single machine. For deep reinforcement learning [Nair 2015, Mnih 2016], the problems are even more challenging. Visualization can help expose the complex interactions across the network, and inform the design of better methods. 

These topics are representative only. Visualization has the potential to impact many other areas of deep learning research. 



## Tentative Schedule##

Morning Session: (9-noon)

Welcome and goals for the workshop (20 minutes)

Invited talk: 45 mins + 15 minutes questions

Break (20 minutes)

Research talks (3 @ 20 minutes)

Lunch + posters (80 minutes)

Afternoon Session: (1pm-5:30pm)

Invited talk: 45 mins + 15 minutes questions

Research talks (2 @ 20 minutes)

Break (20 minutes)

Research talks (2 @ 20 minutes)

Breakout Sessions (80 minutes)

Report from Breakout groups (30 minutes)
