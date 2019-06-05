### Genetic playground

A Javascript web application to explore and experiment with evolutionnary computation principles.
Developed by theo champion as part of the evolutionary computing course at RMIT university.

Source code available at https://github.com/theochampion/genetic-playground
Demo avaialable at https://theochampion.github.io/genetic-playground/

### Genetic configuration parameters

| Name            | Default | Range/Type  | Description                                         |
| --------------- | ------- | ----------- | --------------------------------------------------- |
| Population Size | 10      | Real Number | Size of the population                              |
| Crossover Rate  | 0.9     | [0.0, 1.0]  | Probability of crossover operation (multi point)    |
| Mutation Rate   | 0.2     | [0.0, 1.0]  | Probability of mutation operation (safe random bit flip) |

### Selection operators

| Individual Selectors            | Description                                 |
| ------------------------------- | ------------------------------------------- |
| IndividualSelectors.Tournament2 | Select fittest of two random individuals    |
| IndividualSelectors.Tournament3 | Select fittest of three random individuals  |
| IndividualSelectors.Fittest     | Select fittest individual of the population |
| IndividualSelectors.Random      | Select a random individual                  |

| Pair-wise (parents) Selectors  | Description                                                         |
| ------------------------------ | ------------------------------------------------------------------- |
| ParentsSelectors.Tournament2   | Select a pair of individual using `IndividualSelectors.Tournament2` |
| ParentsSelectors.Tournament3   | Select a pair of individual using `IndividualSelectors.Tournament3` |
| ParentsSelectors.Random        | Select a pair of random individuals                                 |
| ParentsSelectors.FittestRandom | Select a pair of the fittest and a random individual                |
