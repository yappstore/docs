
# Overview


### Introduction

This document outlines the monetization model for our online marketplace platform, detailing the pricing structure, fees, and the rationale behind our approach. Our platform is designed to provide a space where developers can publish and sell their applications, as well as offer free applications, which incur no costs. Below, we provide a comprehensive breakdown of our pricing model, which is crafted to ensure sustainability and profitability for both the platform and the developers.

### Pricing Structure

Our platform operates on a commission-based model, where we take a percentage of each sale as a platform fee. This fee is variable and depends on the pricing of the application set by the developer.

### Tiered Commission Rates:

- For applications priced at €3.50 or higher, we charge a modest 8% commission fee.
- For applications priced below €3.50, we charge a 30% commission fee.


The tiered structure is designed to encourage developers to maintain a minimum price threshold, ensuring that they receive a fair share of the revenue while also covering the costs associated with payment processing through Stripe.


| TRANSACTION STEPS                       | Example 1 | Example 2 | Example 3 | Example 4 |
|-----------------------------------------|-----------|-----------|-----------|-----------|
| **Amount received from customer (Price)**           | $ 5.24    | $ 3.22    | $ 2.56    | $ 0.84    |
| **Stripe Payment Fee 1 (Transaction %)**    | $ 0.01750 | $ 0.01750 | $ 0.01750 | $ 0.01750 |
| **Stripe Payment Fee 2 (Fixed)**            | $ 0.30    | $ 0.30    | $ 0.30    | $ 0.30    |
| **Stripe Takes (Payment Total)**            | $ 0.39    | $ 0.36    | $ 0.34    | $ 0.31    |
|---|---|---|---|---|
| Balance                                 | $ 4.85    | $ 2.86    | $ 2.22    | $ 0.53    |
| Platform commission %                   | 5%      | 8%      | 10%      | 30%      |
| Platform takes                          | $ 0.26    | $ 0.26    | $ 0.26    | $ 0.25    |
| Seller supposed to get                  | $ 4.59    | $ 2.61    | $ 1.96    | $ 0.27    |
| Stripe Payout Fee 1 (Transaction %)     | 0.25%  | 0.25%  | 0.25%  | 0.25%  |
| Stripe Payout Fee 2 (Fixed)             | $ 0.25    | $ 0.25    | $ 0.25    | $ 0.25    |
|---|---|---|---|---|
| Stripe Takes from Platform (Payout Total)| $ 0.25066 | $ 0.25064 | $ 0.25064 | $ 0.25063 |
| Stripe Takes from Seller (Payout Total) | $ 0.26147 | $ 0.25652 | $ 0.25490 | $ 0.25068 |
| Seller Payout (minus fees)              | $ 4.32    | $ 2.35    | $ 1.70    | $ 0.02    |
| Platform Payout (Minus fees)            | $ 0.01    | $ 0.01    | $ 0.01    | $ 0.01    |
| Total Amt Platform have paid to Stripe  | $ 0.65    | $ 0.61    | $ 0.60    | $ 0.57    |
| Profit / Loss to Platform               | $ 0.001   | $ 0.001   | $ 0.001   | $ 0.001   |


The tiered commission structure is informed by the fixed and variable costs imposed by Stripe for payment processing. By setting a higher commission rate for lower-priced apps, we mitigate the relative impact of Stripe's fees, which are more significant for lower transaction amounts. Conversely, the lower commission rate for higher-priced apps provides developers with a greater share of the revenue, incentivizing them to set prices that reflect the value of their applications.