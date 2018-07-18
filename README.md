## A Disciplined Approach to Neural Network Hyper-parameters: Part 1 - Learning Rate, Batch Size, Momentum and Weight Decay

- Reviewing the approach for setting Hyperparameters by Leslie Smith. 
- 'Setting the hyper-parameters remains a black art that requires years of experience to acquire' - Leslie Smith

You can review the paper here: (https://arxiv.org/abs/1803.09820)

The 1 cycle policy involves a cycle with 2 steps of equal length: Step 1 where the learning rate increases linearly from the maximum to the minimum and Step 2 where it linearly decreases.

<p align="center">
<imgsrc="images/one_cycle.png" width=110/>
</p>

