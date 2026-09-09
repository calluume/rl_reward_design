# Reinforcement Learning Reward Design Exercise

[![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?logo=googlecolab&logoColor=fff&style=for-the-badge)](https://colab.research.google.com/drive/101AZsaAstLZ-zEZnoyOOoG-vcO1BaNv5?usp=sharing)

In this exercise, you will be applying the reinforcement learning and traffic management concepts explained in the knowledge capsule. We will be focusing on the reward function and how designers aim to guide RL agents towards learning an optimal policy.

All necessary code can be found in the '_RL KC Exercise_' notebook. We use a small 4-way intersection with a Deep Q-Network (DQN) traffic signal controller, as visualised below. An empty cell has been left for the implementation of the reward function itself, along with some instructions on how to fetch data from the simulation.

The exercise can easily be run locally, but you may also use [Google Colab](https://colab.research.google.com/drive/101AZsaAstLZ-zEZnoyOOoG-vcO1BaNv5?usp=sharing). In this case, create your own copy before starting your work ('_file_' > '_Save a copy in Drive_').

The scenario is simulated using the package UXsim:
  - Documentation: https://toruseo.jp/UXsim/docs/index.html
  - This exercise is based on this [DQN example](https://toruseo.jp/UXsim/docs/notebooks/demo_notebook_03en_pytorch.html).

---
## Objectives

1. Choose a demand profile in the '_Defining the Scenario_' cell.
2. Implement your reward design within the `comp_reward()` function.
3. Train the agent and observe performance using the visualisations at the bottom of the notebook.
4. **Try to produce the lowest overall average delay or travel time!**
5. Compare your approach to the suggested solutions in the separate '_Exercise Solution_' notebook.

Extra objectives (_optional_):
1. Change the OD-demand values or create your own profile to see how this impacts performance.
2. Test different hyperparameter values.

----
## Attribution

The DQN and environment implementation in this exercise are based on the [Pytorch/DQN example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) provided in the UXsim documentation. UXsim is developed by Toru Seo and is distributed under the MIT License. The original code has been modified for the purposes of this exercise.

  - Toru Seo. [UXsim: lightweight mesoscopic traffic flow simulator in pure Python](https://doi.org/10.21105/joss.07617). Journal of Open Source Software, Vol. 10, No. 106, p. 7617, 2025.