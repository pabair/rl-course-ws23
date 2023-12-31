# Lab 2

In this second lab we implement the `policy iteration algorithm` that we saw in the lecture, in order to find the best policy for the `FrozenLake` environment.

### Task:
- Use the file `2_FrozenLake_PolicyEval.py` to implement your solution.
- Implemente the `policy iteration algorithm` that we saw in the lecture to find the best policy. Use a discount factor of `gamma=1`.
Hint: You can access the transition probabilty matrix of the environemnt with `env.unwrapped.P` as follows: 

```
tp_matrix = env.unwrapped.P
for p, s_next, reward, _ in tp_matrix[s][a]:
	print(p)
	print(s_next)
	print(reward)
```

This will give you for a given state `s` and action `a` all possible next states, the transition probability and the associated reward.