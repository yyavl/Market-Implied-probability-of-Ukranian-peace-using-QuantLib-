# Market-Implied Probability of Ukrainian Peace (QuantLib Model)

This project estimates how likely markets think peace in Ukraine is — using the prices of two government bonds. One bond has a special "step-up" payment that only happens if peace is reached by 2028. The other bond does not.
By comparing the market prices of both bonds and building theoretical prices under war and peace scenarios, we back out a market-implied probability of peace.

---

## 🔧 What the Code Does

- Prices Ukrainian bonds using **QuantLib**
- Models two cases:
  - **War scenario**: no peace, no extra payments
  - **Peace scenario**: peace happens, bondholders get more
- Builds a simple formula to compute the **implied probability of peace**
- Plots that probability over time
- Annotates with major political events (e.g. Trump election, Easter truce rumors)

---

## 📄 Bonds Used

- `XS2895056955`: 2034 bond, no peace clause
- `XS2895057177`: 2035 bond, includes peace-triggered extra payments
