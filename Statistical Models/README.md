## Statistical Models

To examine how football market valuations relate to measurable player characteristics, this project developed separate statistical models for defenders, midfielders, and forwards.

A single model was not applied across all players because football positions have different responsibilities and valuation drivers. Instead, each position was evaluated using metrics that best represent its role on the pitch.

The general modelling framework was:

log(Market\ Value) = beta_0 + beta_1X_1 + beta_2X_2 + ... + epsilon

where:

- **Market Value** represents the player's estimated transfer market valuation.
- The logarithmic transformation was applied to market value because football valuations are highly skewed, with a small number of elite players having significantly higher values.
- (X) represents player characteristics and performance indicators.
- (epsilon) represents unexplained variation.

---

## Feature Selection Approach

One of the main challenges in developing the models was selecting appropriate performance indicators.

Football performance is multidimensional, and hundreds of available metrics can potentially influence player valuation. However, including excessive variables can create unnecessary complexity, increase overlap between metrics, and reduce the interpretability of the model.

Rather than using every available statistic, this project selected a limited number of position-specific indicators designed to capture key contributions while maintaining a balanced and interpretable model.

The selected variables were chosen based on three principles:

- **Football relevance:** Metrics should represent important contributions within each position.
- **Model simplicity:** A smaller number of meaningful variables improves interpretability.
- **Reduced bias:** Avoiding excessive metrics prevents the model from favouring players based purely on statistical volume.

---

# Defender Valuation Model

The defender model evaluates how defensive contribution and player context relate to market value.

### Dependent Variable

- Log-transformed market value

### Predictors

**Player Characteristics**
- Age
- Big club status

**Performance Indicators**
- Defensive contribution metric
- Dispossessions per 90 minutes

The defensive contribution metric combines:

- Tackles won per 90
- Interceptions per 90
- Recoveries per 90

These variables aim to represent a defender's ability to regain possession and contribute defensively.

---

# Midfielder Valuation Model

The midfielder model focuses on the combination of defensive, creative, and possession-related contributions.

### Dependent Variable

- Log-transformed market value

### Predictors

**Player Characteristics**
- Age
- Big club status

**Performance Indicators**
- Dispossessions per 90 minutes
- Midfield contribution metric

The midfield contribution metric combines:

- Recoveries per 90
- Interceptions per 90
- Chances created per 90
- Expected assists (xA) per 90

These variables represent both defensive involvement and creative influence.

---

# Forward Valuation Model

The forward model focuses on attacking output and chance creation.

### Dependent Variable

- Log-transformed market value

### Predictors

**Player Characteristics**
- Age
- Big club status

**Performance Indicators**
- Dispossessions per 90 minutes
- Attacking contribution metric

The attacking contribution metric combines:

- Expected goals (xG) per 90
- Dribbles per 90
- Shots on target per 90
- Expected assists (xA) per 90

These variables capture goal threat, attacking involvement, and creative contribution.

---

# Why Separate Models?

Player valuation is position-dependent. A defender is not evaluated using the same criteria as a forward, and a midfielder's contribution cannot be reduced to attacking output alone.

By developing separate models, this project attempts to reflect the different roles players perform while investigating how strongly measurable football characteristics explain market valuations.

The objective is not to estimate the "true" value of a player, but to analyse the relationship between observable performance indicators and the prices assigned by the football transfer market.
