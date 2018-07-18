## A Disciplined Approach to Neural Network Hyper-parameters: Part 1 - Learning Rate, Batch Size, Momentum and Weight Decay

- Reviewing the approach for setting Hyperparameters by Leslie Smith. 
- 'Setting the hyper-parameters remains a black art that requires years of experience to acquire' - Leslie Smith

You can review the paper here: (https://arxiv.org/abs/1803.09820)

The 1 cycle policy involves a cycle with 2 steps of equal length: Step 1 where the learning rate increases linearly from the maximum to the minimum and Step 2 where it linearly decreases.

![](/images/one_cycle.png)

The peak in the middle of the cycle (at 100 iterations) acts as a regularization method to prevent overfitting

### Batch Size and Learning Rate Analysis

![](/images/BS_LR.png)

Low BS and High LR as well as High BS and High LR produce the highest accuracy

### Learning and Validation Loss Analysis based on Weight Decay

![](/images/Under_over.png)

Pictorial explanation of the tradeoff between underfitting and overfitting

![](/images/loss.png)

- The graphs from left to right potray Training (Orange) and Validation (Blue) Loss plots with a Weight Decay(wds) of 1e5, 1e4, 1e3 and 1e2
- The graphs show that the Training loss is above the Validation loss when the wds is 1e5 and 1e4 but the two losses then intersect when the wds is 1e3 and 1e2
