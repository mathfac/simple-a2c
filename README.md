 # Simple Advantage Actor Critic (A2C)

The notebooks in this repo build an A2C from scratch in PyTorch, starting with a Monte Carlo version that takes four floats as input (Cartpole) and gradually increasing complexity until the final model, an n-step A2C with multiple actors which takes in raw pixels. These models are simple in an effort to facilitate understanding. For a more production-strength A2C check out [this model](https://github.com/rgilman33/baselines-A2C) converted from OpenAI baselines.

Notebooks:
1) Monte Carlo A2C
2) Adding N-Step
3) Code walk-through TUTORIAL: A simplified version of 2a used for teaching purposes. Compliment to comic. 
4) Adding in multiple actors
5) Allowing model to take in a stack of "frames" rather that single frame. This in preparation for next step when we add in stack of frames from raw pixels.
6) Transitioning to raw pixel input. Changing FC NN to CNN. Takes hours on p2x large rather than seconds on laptop to train.

0) MC A2C which is also trained to predict its own next state and reward. Currently being used for experiments in transfer learning, prediction, data generation. If a model can predict its own future states, can it use this predictor to generate data for "mental training"?


## Credits

Forked from https://github.com/rgilman33/simple-A2C and adopted for the workshop.