# FSRS trained on simulated data

It's a notebook that trains FSRS on simulated data and evaluates the performance of the model.

The goal is to analyze the relationship between the parameters used to generate the data and the parameters trained on the data.

## Findings

- The trained parameters are not approaching the ideal parameters monotonically over the sample size.
- The trained parameters are even better than the ideal parameters. (It's truly a weird phenomenon.) Here are some hypotheses:
    - The trained parameters overfits the noise introduced during the simulation.
    - The diversity of the simulated data is so low that there are multiple sets of parameters that can fit the data optimally.
- The AUC decreases as the sample size increases. It proves that AUC is not a good metric again.
