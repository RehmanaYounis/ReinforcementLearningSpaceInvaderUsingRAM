#**Reinforcement Learning Space Invader Using RAM**

In this project, I implement a deep learning model to successfully learn control policies directly from high-dimensional sensory inputs using reinforcement learning. We chose to work with RAM Monitor. In this case, environmental monitoring is provided by the state of the RAM, that is, a set of 128 values. Each value is a byte (an integer from 0 to 255). RAM is a compact representation of state compared to algorithms that display the image as a state. In this environment, the player can perform 6 actions: NOOP, RIGHT, LEFT, FIRE, RIGHTFIRE and LEFTFIRE. The reward in the Space Invaders gym environment is the result in the given time step. We notice that different invaders (aliens) have different ranks. 
##Authors: Nicolás Arrieta Larraza

**Motivation**

Quote - Gaming is an Intelligent Art. PERIOD.
As kids we always were intrigued with gaming and computers. One specific part of gaming is 
Arcade games which involves custom built machines which has its own ways of playing each 
game. One such popular game is Space Invaders. As humans we are always looking for some 
extra-terrestrial existence and our race might be invaded some day from the outlanders. This 
game simulates the very scenario in a beautiful and intuitive way. As kids we always loved 
playing and trying to save the planet from this invasion.
Now the A.I field has become so advanced that we can write an effective algorithm, use neural 
network to process the information at hand, learn over practice just like any human does and 
with some tinkering can also outplay many gifted gamers in the world.
We wanted to learn and implement these techniques and train an agent to play just like a human 
being. This agent will use only the present state of the environment and make decisions by 
learning over the time. The very thought is straight from sci-fi but in this generation, it is 
possible for an agent to play with high performance and sometimes better than us.


**Approach and Methods**
In this project, we use the open-source Atari emulator for OpenAI (Brockman et al. 2016), 
OpenAI gym. This emulator offers two possible environments to play Space Invaders. 
The first environment represents each state with a raw RGB image with input dimensions of 
(210,160,3) (SpaceInvaders-v0).
The second environment represents the state of 128 byte RAM (SpaceInvaders-ram-v0). 
As we mentioned in the previous section, we aim to create an agent policy that will make it 
possible for agents to the play the game efficiently and learn from the past experiences over the 
period of time, in this case training with a greater number of episodes. To do this, we use a 
reinforcement learning approach. Nevertheless, learning from high-dimensional state 
representations such as images is not an easy task for traditional reinforcement learning methods 
with literal features. Instead, we use a similar approach called DQN and extending this approach 
in various ways. In this section, we introduce the concept of Deep Q-Nets, reexperiencing, and 
dual-Q learning, all of which are important components of our approach


**Experiments on the RAM State Space**
 
The Atari 2600 uses 128 bytes of RAM for its internal representation of the game state. This 
compact representation is intended to hold all the information that describes the current state of 
the game. This relatively low dimensional representation is attractive way for learning by 
reinforcement algorithm and the Deep Q Learning technique. Working in this state space, we 
experiment with four different architectural models:
• Linear model: a simple linear model, which approximates the Q function as a linear set of 128 
features and has 774 parameters.
• Two-Layer Fully Connected Network: A fully connected neural network in a hidden layer 
consisting of 512 units. This model contains approximately 69,000 parameters.
Fully connected 3-layer network: Two different types of 3-layer neural networks, one with 256 
and 128 hidden layers and the other with 512 and 128 hidden layers.
The performance of these models is shown in by number of episodes




![200](https://user-images.githubusercontent.com/70255794/175225037-63d3b173-1c03-46a7-a2db-e64b65fa7a14.gif)
![ezgif com-gif-maker](https://user-images.githubusercontent.com/70255794/175225069-777ff7b7-0cc4-4265-bd61-cb3aa8a39fac.gif)
![450](https://user-images.githubusercontent.com/70255794/175225118-822df131-1cde-4148-b843-16f18f18b49d.gif)


200 Episodes                300 Episodes                450 Episodes
