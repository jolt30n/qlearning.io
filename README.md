# Machine Learning for Trading
A short presentation on various points of QLearning

Certain points to note:

Slide 5:
- QLearning is not greedy
  
- The learner(the little robot) sees state s
- Take state s and looks in the Q table and find the action that corresponds to the maximum Q value in the policy
- Take that action (T)
- This results in 2 things: new state s’ and reward r
- The Q table then updates the information with these results

Slide 6:
- The query function. To find the new Q value, take the sum of the old value and the new best estimate. The new best estimate takes into consideration the discounted reward for all future actions.
- Alpha is known as the learning rate which is between 0 to 1, but typically around 0.2. A higher value would have the Qlearner learn quickly while a smaller value would have the learner learn slowly.
- Lambda is known as the discount rate which is between 0 to 1. The definition of this would be where the higher the value, the more later rewards are valued significantly while the lower the value, the less, later rewards are valued.
- r is the immediate reward.
