# Carla-RL
Reinforcement Learning codebase for self-driving car in Carla

1. Install python 3.7.
2. Download CARLA 0.9.11 from [here](https://github.com/carla-simulator/carla/releases/tag/0.9.11). Due to a bug in CARLA (see [this PR](https://github.com/carla-simulator/carla/issues/4861)) we can't use carla 0.9.12 and up.
3. Edit settings in settings.py
4. Run with train.py
5. You can just play using play.py after the model get trained.

The agent code is buggy.
It implemented the multi-threading and multi-processing wrongly, caused lots of synchronization issues.
However when it works it should be able to run stabily to be able to finish the training.

When CARLA crashed, you'll need to manually kill the python processes and restart it. It can't actually recover even if the code tried.
