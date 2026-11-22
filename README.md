# Autoregressive AR(p) Models

How past values of a time series influence today's value.

By Meryl Tchuinkeu. The material is written in German.

## What is it for?

Many numbers change over time: sales, prices, temperatures. Often today's value depends on the values from the days or months before. An autoregressive model describes exactly this dependence, and it is a common starting point for forecasts.

In an AR(p) model, today's value is a weighted sum of the last *p* values plus a random error:

$$X_t = c + \varphi_1 X_{t-1} + \varphi_2 X_{t-2} + \dots + \varphi_p X_{t-p} + \varepsilon_t$$

| Symbol | Meaning |
|---|---|
| $X_t$ | today's value |
| $p$ | how many past values the model uses |
| $\varphi_i$ | how strongly the value from *i* steps ago matters |
| $\varepsilon_t$ | random error |

An AR(1) model, for example, uses only yesterday's value.

## What I looked at

1. **A short way to write the model** with the backshift operator ($B X_t = X_{t-1}$).
2. **Stationarity**: when the series stays stable over time, with a constant mean and variance. For AR(1) this holds when $|\varphi_1| < 1$.
3. **Causality**: writing the series as a sum of current and past random errors.
4. **Choosing p**: using the autocorrelation function (ACF) and the partial autocorrelation function (PACF). For an AR(p) model, the PACF drops to zero after lag *p*.
5. **Limits of AR models**: what they can and cannot describe.

## Files

| File | Content |
|---|---|
| `AR_Modelle.pptx` | Presentation of the model and the results (German) |

## Tools

R
