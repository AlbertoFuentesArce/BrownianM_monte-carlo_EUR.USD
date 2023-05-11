# BrownianM_monte_carlo_EUR.USD
Monte Carlo Simulation with Geometric Brownian Motion Model to Predict Future EUR/USD Exchange Rate
<h2>Monte Carlo Simulation with Geometric Brownian Motion Model to Predict Future EUR/USD Exchange Rate</h2>

<p>In this notebook, we will be using the Geometric Brownian Motion (GBM) Model to predict the future evolution of the EUR/USD exchange rate. GBM is a stochastic process that is commonly used in financial modeling to simulate the random movement of assets such as stock prices, exchange rates, and commodity prices. It is based on two components: Drift and Volatility.</p>

The following formula shows how today's price is affected by its value yesterday and its return:

$$
Today's Price = Yesterday's Price \cdot e^{r}
$$

Where r is the logarithmic return of today's price with respect to yesterday's price. 

Next, we will use the Geometric Brownian Motion Model to predict the future evolution of the EUR/USD exchange rate. The model uses two components for Monte Carlo simulation: Drift and Volatility.

**Drift:** The direction in which returns have moved in the past, reflects the long-term trend in stock prices.

$$
drift = μ - \frac{1}{2} \cdot σ^2
$$

**Random Variable:** Represents the historical volatility of the evolution of the exchange rate multiplied by the value z of a random number between 0 and 1. The random variable is generated automatically. The Z value represents the probability of an event happening depending on how many standard deviations it deviates from the mean.

$$
Random Variable = σ \cdot Z(Random(0;1))
$$

Using the Greometric Brownian Model, the equation that generates future data for the exchange rate is as follows:

$$
Today's Price = Yesterday's Price \cdot e^{(μ-\frac{1}{2}\cdot σ^2)+σZ(Random(0;1))}
$$

Here, μ represents the expected return and σ represents the standard deviation of returns. 


```
