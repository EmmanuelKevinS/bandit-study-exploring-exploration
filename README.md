# bandit-study-exploring-exploration

Extending QCARE: How Reward Gap Difficulty Shapes the Cost of Over and Under Exploration
Emmanuel Kevin Suraiskumar
April 2026

This project extends the simulation analysis in Ding et al. (2024), who propose the QCARE model of human exploration-exploitation behaviour in multi-armed bandit problems.

Research Question:
How does the regret cost of over and under exploration vary across reward environments of different difficulty?

What I did:
Implemented QCARE from scratch in Python and simulated agent behaviour across four reward gap configurations and a full sweep of α values (0.1 to 2.0), with T=200 rounds and 5,000 simulations per condition.

Key Findings:
The cost of over-exploration increases sharply with reward gap size. Agents in easy environments are penalised far more for exploring too much
The optimal α shifts upward with gap size. Easy problems warrant more aggressive exploitation than Thompson Sampling prescribes
Thompson Sampling (α = 0.5) is not universally optimal in finite horizon settings

Reference
Ding, J., Feng, Y., & Rong, Y. (2024).
A behavioral model for exploration vs. exploitation. https://arxiv.org/pdf/2207.01028
