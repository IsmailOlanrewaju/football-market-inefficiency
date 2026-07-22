## Methodology

This project uses a statistical modelling approach to examine the relationship between player characteristics and football market valuations.

Since player valuation is influenced differently across positions, separate regression models were developed for defenders, midfielders, and forwards rather than applying a single model to all players.

### Data Preparation

Before modelling, the dataset underwent several preparation steps:

- Players with insufficient playing time were removed to reduce the effect of unreliable performance samples.
- Position-specific performance metrics were combined into broader contribution indicators.
- Market values were transformed using a logarithmic scale to reduce skewness and improve model stability.

### Statistical Modelling

Multiple linear regression models were used to estimate the relationship between player characteristics and market value.

The dependent variable for each model was:

**Log-transformed market value**

The independent variables included:

### Player Factors
- Age
- Big club status

### Performance Factors
- Position-specific performance contribution metrics
- Per-90 performance indicators

Separate models were created for:

- Defender valuation
- Midfielder valuation
- Forward valuation

The purpose of the models was not to predict future transfer fees, but to measure how much of current market valuation can be explained by observable characteristics.

### Market Comparison Analysis

After estimating model-based values, predicted valuations were compared with observed market values.

This comparison was used to identify:

- Players whose market values were broadly supported by measurable characteristics.
- Players whose valuations differed significantly from statistical expectations.

These differences were interpreted as potential market valuation gaps rather than definitive evidence of incorrect pricing.
