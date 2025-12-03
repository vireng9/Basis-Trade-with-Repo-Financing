# **Relative Value Arbitrage – Basis Trade with Repo Financing**
  Note: Full code files available upon request

## **Overview**
- Relative value arbitrage strategy - trading the basis between cash government bonds and their futures, with the bond leg financed in the repo market.​
- Targets mispricing between futures prices and cost‑of‑carry‑adjusted cash bond values, aiming for market‑neutral, rate‑hedged returns.
- Provides a research and backtesting framework that can be extended to other fixed‑income relative value strategies.​

## **Mechanics:**
- Cash Treasury (Leg 1) – The hedge fund buys a Treasury bond in the cash market.
- Financing – The purchase is financed using repurchase agreements (repo), where the bond acts as collateral to borrow cash.
- Futures Short (Leg 2) – Simultaneously, the fund sells short a corresponding Treasury future contract.
- Objective – Profit from the narrowing of the price differential (‘basis’) between the cash bond and the futures by settlement date. Any coupon income and financing cost (repo rate) are factored into the profitability calculation.
- Leverage – The use of repos allows large leverage, often 30 – 60 times capital, making small price differences profitable at scale.

## **Key Risks:**
- Rollover risk – The repo market is typically overnight or very short-term, so positions must be constantly rolled over. If repo rates spike or funding dries up, the position can become costly or even impossible to maintain.
- Liquidity risk – Markets can become illiquid during stress. In March 2020, for example, repo rates surged and margins increased, prompting large unwinds and resulting in negative price moves for Treasuries.
- Margin risk – Futures legs require margin. Rising margin requirements can force early liquidation of trades, leading to losses.
- Basis widening / Convergence risk – If the cash-futures basis does not converge as expected or widens, the trade loses money.
- Systemic risk – Large concentrations of leveraged basis trade across funds can create vulnerabilities, particularly if many players unwind simultaneously.

## **Recent Trends (2024- 2025)**
- Trade Size – Gross notional exposure for basis trades remains at $ 1  2 trillion, the highest ever.
- Central Bank Backstops – The NY Fed’s Standing Repo Facility now acts as a funding safety net, helping to dampen forced selling risk and stabilize markets during volatility (seen in April 2025).
- Regulatory Changes – The SEC is expanding central clearing for Treasuries through the Fixed-Income Clearing Corporation, with significant dates from late 2025 into 2026. This reduces bilateral risk, improves margin efficiency, and promotes market stability.
- 2025 Events – Despite April 2025 market volatility from tariff news, repo funding, and basis positions remained notably stable, in contrast to previous crises.
- Ongoing risks – Financial stability concerns persist, as basis trades are exposed to funding and liquidity shocks. Regulators remain alert to the systemic risk posed by concentrated, leveraged positions.

## **Files**
- ipynb shows full interactive notebook with code, outputs and visualizations.
- PDF shows static version for quick review.
- README.md shows project documentation.

## **Motivation**
- Relative value fixed‑income strategies aim to monetize pricing discrepancies between closely related instruments while minimizing exposure to broad rate moves. The cash–futures basis trade is a canonical example, where deviations between futures prices and the cost‑of‑carry‑adjusted cash bond value can become large due to funding conditions, balance sheet constraints, and risk sentiments, rather than changes in fundamental value.​
- Repo financing is central to the economics of this trade, because it determines the effective cost of holding the long bond leg and therefore the fair basis level. By explicitly modeling repo rates, haircuts, and specials, this project seeks to distinguish between apparent and realizable arbitrage, helping to understand when high headline spreads compensate for funding, balance sheet, and liquidity risks.
- A systematic, transparent implementation provides a platform for studying leverage, margin, and liquidity stresses in basis trades, which have been at the center of several market dislocations.
  
## **Author**

**Viren Ghaghada**  
[LinkedIn](https://www.linkedin/in/virenghaghada) | [Email](mailto:vireng9@yahoo.com) | [GitHub](https://www.github.com/vireng9) | [My Portfolio](https://vireng9.github.io/)  

## **Disclaimer**
This project is for educational and research purpose only. It should not be considered as a financial advice or a production-ready trading system.



