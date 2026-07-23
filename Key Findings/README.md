# Key Findings

## 1. Limited First-Team Exposure: The Hidden Market Capital

Before modelling player valuation, we investigated players with **fewer than 10 league appearances (90-minute equivalent)** during the 2025/26 season.

These players represent a unique market segment: **high-value U-23 assets with limited first-team exposure**.

The analysis identified players whose market values remained high despite limited league involvement.

### Clubs with the Highest Idle Market Value

| Rank | Club | Total Market Value (€) | Number of Players |
| 1 | Chelsea | €174M | 7 |
| 2 | Arsenal | €110M | 3 |
| 3 | RB Leipzig | €102M | 5 |
| 4 | Bayern Munich | €100M | 1 |
| 5 | AC Milan | €69M | 4 |

Chelsea recorded the highest accumulated market value among players with limited league exposure.

However, this metric should not be interpreted as evidence of poor squad management or incorrect valuation.

Limited minutes can occur because of:

- Injury situations
- Tactical decisions
- Competition within elite squads
- Gradual player development pathways

For example, **Jamal Musiala** appeared among the highest-valued limited-minute players, but his reduced playing time was heavily influenced by injury.

The purpose of this analysis is therefore not to label these players as inefficient, but to highlight where significant financial value exists despite limited recent match exposure.

---

# 2. Statistical Valuation Models

We developed separate regression models for:

- Defenders
- Midfielders
- Forwards

The objective was to estimate how much of player market value could be explained by measurable football characteristics.

The dependent variable was:
Log(Market Value)

This transformation reduced the impact of extreme transfer values and allowed better modelling of football's highly skewed market.


# 3. Model Performance

## Defender Model

### Variables

- Age
- Big club status
- Defensive contribution metrics
- Defensive composite metric

### Results

| Metric | Value |
| R² | 0.254 |
| Adjusted R² | 0.215 |
| Model significance | p < 0.001 |

### Significant Factor

**Big club status**

(p < 0.001)

---

The defender model explained approximately **25% of market value variation**.

Interestingly, traditional defensive statistics alone explained limited variation.

This suggests that young defender valuations are heavily influenced by:

- Club reputation
- Development potential
- Scouting perception
- Future expectations

---

# Midfielder Model

### Variables

- Age
- Big club status
- Defensive actions
- Creative output
- Composite midfield metric

### Results

| Metric | Value |
| R² | 0.282 |
| Adjusted R² | 0.239 |
| Model significance | p < 0.001 |

### Significant Factor

**Big club status**

(p < 0.001)

---

The midfielder model explained approximately **28% of valuation differences**.

Midfielders were the most difficult position to evaluate statistically because their impact depends heavily on:

- Tactical role
- Ball progression
- Pressing responsibilities
- System fit

Many important midfield qualities are difficult to capture using only basic match statistics.

---

# Forward Model

### Variables

- Age
- Big club status
- Dispossessions
- Attacking contribution metrics

### Results

| Metric | Value |
| R² | 0.323 |
| Adjusted R² | 0.272 |
| Model significance | p < 0.001 |

### Significant Factors

- Big club status
- Attacking performance metric

---

The forward model achieved the highest explanatory power.

This suggests attacking output is easier to measure statistically through variables such as:

- Expected goals
- Shots on target
- Chance creation
- Goal contributions

However, even the strongest model explained only around one-third of market valuation.

---

# 4. Market Value vs Model Prediction

After generating predicted valuations, we compared model estimates against actual market values.

Across **210 U-23 players included in the final modelling dataset:**

| Category | Players |
| Model valuation above market value | 93 |
| Market value above model valuation | 117 |

---

# 5. Understanding Large Market Differences

The confidence interval analysis highlighted players where market values were significantly different from statistical expectations.

## Example: Pau Cubarsí

| Metric | Value |
| Market Value | €80M |
| Model Prediction | €32.9M |
| 95% Confidence Interval | €23.3M - €46.4M |

---

Cubarsí's current measurable contribution aligns closer to the €30M-€40M range.

However, the market valuation reflects additional factors:

- Exceptional age profile
- Barcelona development pathway
- Elite competition exposure
- Future potential
- Scarcity of elite young defenders

This difference represents the gap between:

**Statistical contribution value**

and

**Football market value**

---

# 6. Examples of Market Premiums

Several elite midfielders demonstrated large differences between statistical estimates and market valuation.

| Player | Market Value | Model Estimate |
| João Neves | €140M | €42M |
| Pedri | €150M | €60M |
| Jude Bellingham | €130M | €48M |

---

# 7. Interpreting Model R²

The models achieved R² values between:


25% - 32%


This does not indicate model failure.

Football markets contain many variables that cannot easily be measured:

- Potential
- Reputation
- Contract situation
- Agent influence
- Market demand
- Trophy exposure
- Future expectations

The remaining unexplained variation represents the complexity of football valuation.

The objective of this project was not to perfectly predict transfer fees.

Instead, it investigates:

> How much of football market valuation can be explained through measurable performance, and where market perception begins to dominate statistical evidence.

---

### Final Conclusion

This project demonstrates that football transfer markets are not purely determined by measurable performance.

Using U-23 players from Europe's top five leagues:

Premier League
La Liga
Bundesliga
Serie A
Ligue 1

we found that statistical performance indicators explain only a portion of market valuation.

The remaining valuation gap represents the complexity of football economics: potential, reputation, scarcity, and market perception.

The future of football transfer market requires more advanced models that combine traditional statistics with broader contextual variables to better estimate true player value and reduce inefficient spending in an increasingly expensive transfer market.
