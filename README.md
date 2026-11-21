# Autoregressive AR(p) Models – Time Series Analysis in R

University project in **Business Mathematics** at **HTW Berlin**, by **Meryl Tchuinkeu**.

The project asks how past values of a time series influence its present value. It covers the definition, the mathematical representation and the main theoretical properties of autoregressive models.

> 🚧 **Work in progress.** The project materials are written in German.

## The AR(p) model

In an autoregressive model of order *p*, the current value depends on its own *p* previous values plus a random error:

$$X_t = c + \varphi_1 X_{t-1} + \varphi_2 X_{t-2} + \dots + \varphi_p X_{t-p} + \varepsilon_t$$

| Symbol | Meaning |
|---|---|
| $X_t$ | current value |
| $p$ | number of past values used (model order) |
| $\varphi_i$ | influence of the past value $X_{t-i}$ |
| $\varepsilon_t$ | random error (white noise) |

Example: an **AR(1)** model uses exactly one past value.

## What the project covers

- **Backshift operator**: compact notation for lagged values, $B X_t = X_{t-1}$
- **Stationarity**: constant mean and variance, with covariances that depend only on the lag. For AR(1) the condition is $|\varphi_1| < 1$.
- **Causality**: representing the process through current and past random errors
- **ACF and PACF**: describing temporal dependence and identifying the model order *p*. The PACF cuts off after lag *p*.
- **Interpretation**: what the model order means, and where AR models reach their limits

## Repository contents

| File | Description |
|---|---|
| `Autoregressive_ARp_Kurzvortrag.pptx` | Short presentation (in German): idea, theory and goals of the project |

## Tools

R · Time series analysis · Statistics

## Author

Meryl Tchuinkeu – B.Sc. Business Mathematics, HTW Berlin
