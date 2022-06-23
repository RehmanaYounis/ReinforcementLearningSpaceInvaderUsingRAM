# ReinforcementLearningSpaceInvaderUsingRAM

In this project, I implement a deep learning model to successfully learn control policies directly from high-dimensional sensory inputs using reinforcement learning. We chose to work with RAM Monitor. In this case, environmental monitoring is provided by the state of the RAM, that is, a set of 128 values. Each value is a byte (an integer from 0 to 255). RAM is a compact representation of state compared to algorithms that display the image as a state. In this environment, the player can perform 6 actions: NOOP, RIGHT, LEFT, FIRE, RIGHTFIRE and LEFTFIRE. The reward in the Space Invaders gym environment is the result in the given time step. We notice that different invaders (aliens) have different ranks. 
##Authors: Nicolás Arrieta Larraza
![200](https://user-images.githubusercontent.com/70255794/175225037-63d3b173-1c03-46a7-a2db-e64b65fa7a14.gif)
![ezgif com-gif-maker](https://user-images.githubusercontent.com/70255794/175225069-777ff7b7-0cc4-4265-bd61-cb3aa8a39fac.gif)
![450](https://user-images.githubusercontent.com/70255794/175225118-822df131-1cde-4148-b843-16f18f18b49d.gif)
