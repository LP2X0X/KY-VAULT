- A Cost Function transforms everything that occurs within the network into a number that represents the Total Error of the network. Essentially, it is a measure of how wrong a network is.
- In order for a Neural Network to successfully train it must minimize the difference between its actual output and target output to find the Global Minimum (or a Local Minimum that is close enough to the global). This difference is the Total Error, which essentially tells us how wrong a network is.
### Example
- Mean Squared Error: The Mean Squared Error function takes the sum of all squared output errors in a network and averages them.
![[Pasted image 20230104081418.png|center]]
---
![[Pasted image 20230104081718.png|center]]
1. Calculate the Local Error of each Output Node: The Local Error is the difference between a single training example’s Actual Output and Target Output.
![[Pasted image 20230104081739.png|center|500]]
```ad-note
One training is one [[1st Stage of Neural Network]].
```
2. Sum the Local Errors of all training examples: In this step all of the final Local Errors of every training example are summed.
![[Pasted image 20230104082121.png|center]]
1. Multiply and Average: In this final step, 1 is divided by the total number of training examples, n. The result is then multiplied against the sum of all Local Errors. This <u>normalizes</u> the sum, which transforms the error into a common frame of reference that we can understand and work with.
![[Pasted image 20230104084439.png|center]]