For this Lab, you will train an agent to solve the Physical Deception problem.

This is an ungraded project, Feel free to explore various parameters and see how it affects the way agents approach the problem.

## Goal of the environment

Blue dots are the "good agents", and the Red dot is an "adversary". All of the agents' goals are to go near the green target. The blue agents know which one is green, but the Red agent is color-blind and does not know which target is green/black! The optimal solution is for the red agent to chase one of the blue agent, and for the blue agents to split up and go toward each of the target.

## Running within the workspace ( Recommended Option)

- No explicit setup commands need to run by you, we have taken care of all the installations in this lab, enjoy exploration.
- ./run_training.sh Let's you run the program based on the parameters provided in the main program.
- ./run_tensorboard.sh will give you an URL to view the dashboard where you would have visualizations to see how your agents are performing. Use this as a guide to know how the changes you made are affecting the program.
- Folder named Model_dir would store the episode-XXX.gif files which show the visualization on how your agent is performing.

## Running on your own computer

- If you choose to run the program on your computer, you should download the files from the workspace and all the above commands should work the same except for few installations below.
- Use of GPU wouldn't impact the training time for this program, Instead, Multicore environments would be a better choice to increase the training speed.

###  Requirements

- [OpenAI baselines](https://github.com/openai/baselines), commit hash: 98257ef8c9bd23a24a330731ae54ed086d9ce4a7
- [PyTorch](https://pytorch.org), version: 0.3.0.post4
- [OpenAI Gym](https://github.com/openai/gym), version: 0.9.4
- [Tensorboard](https://github.com/tensorflow/tensorboard), version: 0.4.0rc3 and [Tensorboard-Pytorch](https://github.com/lanpa/tensorboardX), version: 1.0 (for logging)

## To Experiment
- Feel free to clear the model_dir and log folder and start training on your own to see how your agent performs. ./clean.sh should help you accomplish this goal.
- This lab is meant to prepare you for the final project, writing your own functions in maddpg.py will improve your learning curve.
- Also experiment with parameter tuning in main.py, Make note that a larger number of episodes would mean greater training time.
- Lab might take more than one hour to train depending on how the parameters are tuned.