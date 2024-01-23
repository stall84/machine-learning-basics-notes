### Statistics Review (Limited) and Probabilistic Model (Distribution) in ML

#### Distribution Concepts

- [Definition:](https://en.wikipedia.org/wiki/Probability_distribution#Absolutely_continuous_probability_distribution) In probability theory and statistics, a probability distribution is the mathematical function that gives the probabilities of occurrence of different possible outcomes for an experiment. It is a mathematical description of a random phenomenon in terms of its sample space and the probabilities of events (subsets of the sample space).
- _"The *shape* of data"_
- Of course _not *all* data can be considered_ in evaluating statistics on any one subject. So instead we'll look at _samples_ of data, which can be thought of as _'shadows'_ of the complete set of all data, and in doing so we look for _shapes_ in the sample data that allow extrapolation to the whole.
- [_Standard Deviation_ $\sigma$:](https://en.wikipedia.org/wiki/Standard_deviation) The average distance between any point and the _mean_ of a probability distribution (dataset). Can also be stated as _The measure of the amount of *variation* of a random variable expected about it's mean_. A low $\sigma$ indicates that the values tend to be close to the mean (a.k.a. 'expected value') of the set, while a high $\sigma$ indicates the values are spread out over a wider range.
- SD Formula: $\sigma = \sqrt{\dfrac{\sum(x_i - \mu)^2}{N}}$
- Where $\sigma$ is the standard deviation, $N$ is the size of the population, $x_i$ is each value from the population, and $\mu$ is the population mean
- [Empirical Rule (aka 68-95-99.7 Rule or 3-sigma Rule)](https://en.wikipedia.org/wiki/68%E2%80%9395%E2%80%9399.7_rule). Basically in a _normal distribution_, 68% of the points/samples will fall within $1\sigma$ of the population mean. 95% within $2\sigma$ and 99.7% within $3\sigma$
- [Z-Score:](https://en.wikipedia.org/wiki/Standard_score) How many standard deviations away your datapoint is from the population mean

#### Probabilistic Model

- There exists a probability distribution $D$ over input/output pairs
- If we write $x$ as input and $y$ as output, then $D$ is a distribution over $(x,y)$ pairs.
- This is often called the _data generating distribution_

- Unreasonable pairs occur rarely while more reasonable input-output pairs occur more often.
