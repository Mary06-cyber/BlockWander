# August 2026 MSX Referral Code (1KSn77) | How Is the MSX Liquidation Price Calculated? Margin, Leverage and Liquidation Explained

MSX offers crypto perpetual futures as well as RWA-related perpetual products tied to tokenized U.S. stocks and other real-world assets. These products allow traders to open leveraged long or short positions, but once leverage is introduced, the key number is no longer just the entry price.

You also need to understand:

- Initial Margin
- Maintenance Margin
- Mark Price
- Liquidation Price
- Isolated Margin vs Cross Margin
- Funding Fees
- Position Size
- Leverage

The basic liquidation logic is simple:

When the margin supporting a position falls below the required maintenance margin, the position may enter forced liquidation.

MSX currently provides perpetual futures trading with Cross margin and adjustable leverage on its trading interface, while its official materials also warn that leveraged futures positions can lose their entire margin if liquidation occurs.

For users creating a new MSX account in August 2026:

📌 **MSX Referral Code:** 1KSn77

🔗 **MSX Registration Link:**

https://msx.com/?code=1KSn77

MSX's official invitation program states that spot and futures referral commissions can reach up to 20%, while the actual benefit depends on the account, campaign, and referral relationship.

## 1. 📌 What Is Liquidation on MSX?
Liquidation means the platform forcibly closes a leveraged position because the available margin is no longer sufficient to satisfy the position's maintenance margin requirement.

For example:

You open a BTC perpetual long position.

If BTC rises, the position generates unrealized profit.

If BTC falls, unrealized losses reduce your effective margin.

Once losses become large enough that the remaining margin approaches the maintenance margin threshold, the account may trigger liquidation.

The process can be summarized as:

Open leveraged position → Price moves against position → Unrealized loss increases → Margin ratio deteriorates → Maintenance margin threshold reached → Forced liquidation

MSX's own educational materials describe perpetual liquidation as a situation where insufficient margin causes a position to be forcibly closed, potentially resulting in the loss of the entire margin allocated to that position.

## 2. 📊 Initial Margin vs Maintenance Margin vs Available Margin
These three concepts are often mixed together.

| Margin Term | What It Means | When It Matters |
|---|---|---|
| Initial Margin | Capital required to open a leveraged position | When opening the trade |
| Maintenance Margin | Minimum margin required to keep the position open | Determines liquidation risk |
| Available Margin | Funds still available to support positions or new orders | Changes with PnL and other positions |
| Position Margin | Margin currently supporting a specific position | Important in isolated mode |
| Account Equity | Account balance plus unrealized PnL | Important in cross-margin calculations |

Suppose you open a 10,000 USDT position using 10x leverage.

Ignoring fees for the moment:

- Position Notional: 10,000 USDT
- Leverage: 10x
- Initial Margin ≈ 1,000 USDT

This does not mean you can safely lose the entire 1,000 USDT before liquidation.

The platform still needs to retain a certain maintenance margin, so liquidation normally occurs before the position margin reaches zero.

## 3. 📊 How Leverage Changes Liquidation Risk
The higher the leverage, the less price movement is required to consume the available margin.

| Leverage | Approximate Initial Margin for a $10,000 Position | Approximate Price Move That Becomes Dangerous* | Risk Level |
|---|---|---|---|
| 2x | $5,000 | Large move required | Lower |
| 3x | $3,333 | Relatively large move | Lower–Medium |
| 5x | $2,000 | Moderate adverse move | Medium |
| 10x | $1,000 | Roughly single-digit % adverse move can become critical | High |
| 20x | $500 | Small adverse move can become critical | Very High |
| 50x | $200 | Very small price move can threaten margin | Extreme |

*This is a conceptual comparison, not an exact MSX liquidation-price table. Actual liquidation depends on maintenance margin, fees, funding, position size, margin mode, and account equity.

The important point is:

Leverage does not make the asset itself more volatile. It makes your margin more sensitive to the same price movement.

## 4. 🧮 How Is MSX Liquidation Price Calculated?
There is no safe universal formula that can reproduce the exact liquidation price shown by every MSX contract, because the displayed liquidation price can depend on several account-level parameters.

At a high level, the calculation needs to account for:

Entry Price + Position Direction + Leverage + Initial Margin + Maintenance Margin + Fees + Funding + Margin Mode

For a simplified USDT-margined long position, a teaching approximation is:

`Liquidation Price ≈ Entry Price × (1 − Initial Margin Rate + Maintenance Margin Rate)`

For a simplified short position:

`Liquidation Price ≈ Entry Price × (1 + Initial Margin Rate − Maintenance Margin Rate)`

Where:

`Initial Margin Rate ≈ 1 ÷ Leverage`

This is useful for understanding the mechanism, but it should not be used as a substitute for the liquidation price displayed by MSX.

The actual platform value is more important because maintenance margin can vary by position size and contract rules.

## 5. 📈 Example: 10x Long Position
Assume:

- BTC Entry Price: 100,000 USDT
- Position Size: 10,000 USDT
- Leverage: 10x
- Initial Margin: approximately 1,000 USDT
- Maintenance Margin Rate: hypothetical 0.5% for demonstration

Initial Margin Rate:

`1 ÷ 10 = 10%`

Simplified liquidation approximation:

`100,000 × (1 − 10% + 0.5%)`

≈

`90,500 USDT`

So under this simplified example, the position could approach liquidation around 90,500 USDT, not exactly 90,000 USDT.

Why?

Because the platform still requires maintenance margin.

And in real trading, the displayed liquidation price could move further because of:

- Trading fees
- Funding fees
- Additional margin
- Position size tiers
- Cross-margin equity
- Other open positions

## 6. 📉 Example: 10x Short Position
Now assume the same conditions but the trader opens a short position:

- Entry: 100,000 USDT
- Position: 10,000 USDT
- Leverage: 10x
- Initial Margin Rate: 10%
- Hypothetical Maintenance Margin Rate: 0.5%

Simplified approximation:

`100,000 × (1 + 10% − 0.5%)`

≈

`109,500 USDT`

For a short position, rising prices increase losses.

So the liquidation price appears above the entry price.

## 7. 📊 Long vs Short Liquidation Comparison
| Item | Long Position | Short Position |
|---|---|---|
| Profits When | Price rises | Price falls |
| Loses When | Price falls | Price rises |
| Liquidation Price Usually | Below entry price | Above entry price |
| Higher Leverage Effect | Liquidation moves closer to entry | Liquidation moves closer to entry |
| Adding Margin | Usually moves liquidation farther away | Usually moves liquidation farther away |
| Funding Impact | Depends on funding direction | Depends on funding direction |

This is why simply saying “10x leverage means liquidation at exactly -10%” is inaccurate.

Maintenance margin and trading costs mean liquidation generally happens before the theoretical margin reaches zero.

## 8. ⚖️ Isolated Margin vs Cross Margin
This is one of the most important comparisons when discussing liquidation.

| Feature | Isolated Margin | Cross Margin |
|---|---|---|
| Margin Source | Margin assigned to one position | Shared eligible account balance |
| Risk Containment | Better | Lower |
| Other Funds Can Support Position | Usually no | Yes |
| One Losing Position Can Affect Other Funds | More limited | Yes |
| Liquidation Price Stability | Easier to understand | Can change with account equity |
| Suitable for Beginners | Usually easier to manage | Requires more account-level risk management |
| Capital Efficiency | Lower | Higher |

### Isolated Margin
In isolated mode, a fixed amount of margin supports the individual position.

Example:

You allocate 500 USDT to an NVDA perpetual position.

If the trade moves sharply against you, the loss is mainly contained within the margin assigned to that position.

Adding more margin can move the liquidation price farther from the current market.

### Cross Margin
In cross margin, the platform can use eligible account equity to support the position.

That means a losing position may consume more of the available balance before liquidation.

The advantage is that temporary market movements may be easier to withstand.

The disadvantage is that one bad position can affect a much larger part of the account.

MSX's trading interface currently displays Cross margin as an available perpetual trading configuration.

## 9. 📊 Isolated vs Cross: Example
Assume two traders each have 5,000 USDT total capital and open the same 10x position.

| Item | Trader A: Isolated | Trader B: Cross |
|---|---|---|
| Total Account Balance | 5,000 USTT | 5,000 USDT |
| Position Notional | 10,000 USDT | 10,000 USDT |
| Assigned Initial Margin | 1,000 USDT | 1,000 USDT |
| Extra Account Funds Supporting Position | No, unless manually added | Potentially yes |
| Maximum Loss Exposure | More contained | Can consume more account equity |
| Liquidation Behavior | More position-specific | Depends on entire account condition |

Cross margin may produce a liquidation price that appears farther away, but that does not make the trade safer automatically.

It simply means more account capital may be available to absorb losses.

## 10. 🏷️ What Is Maintenance Margin?
Maintenance margin is the minimum equity required to keep a leveraged position open.

It is one of the core inputs behind liquidation.

MSX-related materials specifically note that a higher maintenance margin rate reduces effective usable leverage and causes liquidation thresholds to become more restrictive.

A simplified relationship is:

`Margin Remaining > Maintenance Margin → Position remains open`

`Margin Remaining ≤ Maintenance Margin → Liquidation risk`

The exact maintenance margin rate may vary depending on:

- Contract
- Position size
- Risk tier
- Leverage
- Market conditions
- Platform rules

That is why two positions using the same leverage may not necessarily have exactly the same liquidation-distance percentage.

## 11. 📍 Mark Price vs Last Price: Which One Matters for Liquidation?
This distinction is critical.

**Last Price**
The last price is the most recent price at which a trade occurred in the order book.

**Mark Price**
The mark price is designed to provide a fairer reference value and reduce the chance that a temporary order-book spike alone triggers liquidation.

For perpetual futures, liquidation systems generally rely on a mark-price or index-based risk mechanism rather than simply reacting to one isolated last trade.

MSX states that its stock-related perpetual contracts use an index/oracle-style reference mechanism, while its trading interface separately displays an MSX Index Engine for market data.

For practical trading, always check which price MSX specifically identifies as the liquidation trigger for the contract you are trading.

Do not assume that because the candlestick touched your liquidation price, the position must have been liquidated—or that because the last price has not touched it, liquidation is impossible.

## 12. 💵 Do Trading Fees Affect Liquidation Price?
Yes, indirectly.

Trading fees reduce account equity.

MSX currently lists contract trading fees on its official site, with a maker fee of 0.02% and taker fee of 0.045% on the platform FAQ.

For example:

If you open a 100,000 USDT notional perpetual position using a market order at a 0.045% taker fee:

`100,000 × 0.045% = 45 USDT`

That 45 USDT cost reduces your effective equity.

For a low-leverage trade, the difference may be small.

For a highly leveraged position with very little margin buffer, fee costs become much more meaningful.

## 13. 💸 Can Funding Fees Push a Position Closer to Liquidation?
Yes.

Perpetual contracts do not expire, so funding payments are used to help keep the contract price aligned with the underlying reference price.

MSX-related material states that funding is settled periodically and can become a meaningful holding cost, particularly during highly directional markets.

Suppose you hold a leveraged long position for several funding periods and longs are paying shorts.

Each funding payment reduces your effective account equity.

That can gradually move the position closer to liquidation even if the market price itself does not change significantly.

A position can therefore become riskier over time because of:

`Trading Loss + Funding Cost + Trading Fees`

not just price movement.

## 14. 📊 What Moves the Liquidation Price?
| Factor | Effect on Liquidation Risk |
|---|---|
| Higher Leverage | Liquidation price moves closer to entry |
| Lower Leverage | More room before liquidation |
| Add Margin | Usually increases liquidation buffer |
| Remove Margin | Reduces liquidation buffer |
| Larger Adverse Price Move | Increases liquidation risk |
| Funding Fees Paid | Reduces equity |
| Trading Fees | Reduce available equity |
| Higher Maintenance Margin Requirement | Liquidation occurs sooner |
| Cross-Margin Extra Balance | Can support losing positions |
| Other Losing Cross Positions | Can reduce support available |

This is why liquidation price should be treated as a dynamic risk number, especially in cross margin.

## 15. 🚨 What Happens When MSX Liquidates a Position?
A simplified liquidation process looks like:

Mark/reference price approaches liquidation threshold → Margin condition fails → Platform takes control of risk reduction → Position is reduced or closed

The purpose is to prevent losses from exceeding the collateral available to the position or account.

In extremely volatile markets, the final execution price may differ from the liquidation trigger because of liquidity and slippage.

MSX-related futures material also references an Auto-Deleveraging (ADL) mechanism in leveraged derivatives risk management.

ADL is not the same thing as normal liquidation.

## 16. 📊 Liquidation vs ADL vs Stop-Loss
| Mechanism | Who Triggers It? | Purpose | When It Happens |
|---|---|---|---|
| Stop-Loss | Trader | Exit before losses become too large | At user-defined trigger |
| Liquidation | Platform risk engine | Protect margin system | Margin requirement fails |
| ADL | Platform | Reduce counterparty/system risk | Extreme liquidation conditions |
| Manual Close | Trader | Exit position voluntarily | Anytime market allows |

The best outcome is usually not to “manage liquidation.”

It is to avoid getting close enough for liquidation to become the main exit mechanism.

A stop-loss is a trading instruction.

Liquidation is a platform risk-control process.

They should not be treated as substitutes.

## 17. 📉 Why High Leverage Causes Positions to Liquidate So Quickly
Assume a trader has 1,000 USDT.

Compare two positions:

**Position A**
5x leverage:

`1,000 × 5 = 5,000 USDT position`

**Position B**
20x leverage:

`1,000 × 20 = 20,000 USDT position`

A 1% adverse move creates approximately:

- 5x position → 50 USDT unrealized loss
- 20x position → 200 USDT unrealized loss

Same 1% market move.

Very different effect on margin.

| Market Move Against Position | 5x Position PnL Impact* | 10x Position PnL Impact* | 20x Position PnL Impact* |
|---|---|---|---|
| -1% | -5% of margin | -10% | -20% |
| -2% | -10% | -20% | -40% |
| -3% | -15% | -30% | -60% |
| -4% | -20% | -40% | -80% |
| -5% | -25% | -50% | -100% theoretical |

*Simplified leverage illustration before maintenance margin, fees, and funding.

This table explains why a 20x position does not need a 20% market crash to get liquidated.

A much smaller adverse move can consume most of the margin.

## 18. 📈 MSX Tokenized Stock Perpetuals Have Additional Risk
MSX is not limited to BTC and ETH perpetuals. Its platform also provides RWA perpetual contracts tied to U.S. stock-related indices and other real-world assets. MSX describes RWA perpetuals as on-chain contracts tied to stock-token indexes that allow leveraged long or short positions without expiry.

This adds several risks beyond standard crypto perpetuals:

- U.S. market session changes
- Earnings announcements
- Pre-market and after-hours volatility
- Index/oracle pricing
- Lower liquidity outside core market hours
- Large overnight gaps
- Company-specific news
- Macro events

For example, NVDA may move sharply after an earnings release.

A trader holding a highly leveraged NVDA perpetual may see the liquidation buffer disappear much faster than expected.

## 19. 📊 Crypto Perpetual vs Tokenized Stock Perpetual Liquidation Risk
| Risk Factor | BTC/ETH Perpetual | U.S. Stock / RWA Perpetual |
|---|---|---|
| Market Hours | 24/7 crypto market | Underlying stock market has sessions |
| Overnight Gap Risk | Continuous trading reduces traditional gaps | Can be more relevant |
| Earnings Risk | Not applicable | Very important |
| Company-Specific News | Lower | High |
| Macro Sensitivity | High | High |
| Funding | Yes | Product dependent |
| Leverage Risk | High | High |
| Oracle / Index Risk | Yes | Particularly important |
| Weekend Underlying Market Closure | Crypto remains active | Stock underlying may be closed |

The liquidation mechanism may look similar, but the source of volatility can be very different.

## 20. 🛡️ How to Reduce Liquidation Risk
There is no method that removes futures risk, but several practices materially change the margin buffer.

**Use Lower Leverage**
Instead of asking:

“What is the maximum leverage MSX allows?”

ask:

“How much adverse movement can this position survive?”

**Prefer Isolated Margin When Learning**
Isolated margin makes it easier to understand the maximum capital allocated to a specific trade.

**Set Stop-Loss Before Liquidation**
Do not use the liquidation price as the stop-loss.

There should normally be meaningful distance between:

`Entry Price → Stop-Loss → Liquidation Price`

**Keep Margin Buffer**
Do not use nearly 100% of available account equity as initial margin.

**Watch Funding**
A position held for multiple funding periods may lose margin even when the market is relatively stable.

**Reduce Position Size Before Major Events**
For tokenized stock perpetuals, events such as:

- NVIDIA earnings
- Tesla earnings
- FOMC
- CPI
- Nonfarm Payrolls
- Major geopolitical events

can create abrupt price movements.

## 21. 📝 How to Register MSX With Referral Code 1KSn77
If you do not yet have an MSX account:

📌 **MSX Referral Code:** 1KSn77

🔗 **MSX Registration Link:**

https://msx.com/?code=1KSn77

MSX's registration page includes an optional invitation-code field, so the code should be checked before account creation.

A typical setup flow is:

Open referral link → Enter email → Confirm 1KSn77 → Create account → Complete required verification → Secure account → Deposit USDT → Transfer to trading account → Open perpetual market

Before opening any leveraged position, review the contract's:

- Leverage range
- Margin mode
- Maintenance margin
- Mark/index price
- Funding rate
- Liquidation price
- Trading fee

## 22. ⚠️ Common MSX Liquidation Mistakes
1. **Thinking 10x leverage means exactly a 10% liquidation distance**
   It does not.
   Maintenance margin, fees, funding, and account structure affect the actual liquidation price.

2. **Looking only at the last traded price**
   The risk engine may use a mark/index-based mechanism.

3. **Treating Cross Margin as “safer”**
   Cross margin can prevent an individual position from liquidating as quickly, but it can expose more account equity.

4. **Using the liquidation price as a stop-loss**
   Liquidation is an emergency risk-control mechanism, not a trading plan.

5. **Ignoring funding fees**
   Funding payments can reduce margin over time.

6. **Increasing leverage because the liquidation price “looks far away”**
   Position size and volatility matter just as much.

7. **Using maximum leverage on stock perpetuals around earnings**
   A small gap or sudden repricing can eliminate the margin buffer quickly.

## 23. ❓ August 2026 MSX Liquidation FAQ
**Q1: What is the MSX referral code?**
The referral code used in this guide is:
**1KSn77**
Registration link:
https://msx.com/?code=1KSn77

**Q2: What triggers liquidation on MSX?**
At a high level, liquidation occurs when the margin supporting a leveraged position can no longer satisfy the required maintenance margin.

**Q3: Does 10x leverage mean I get liquidated after exactly a 10% loss?**
No.
Maintenance margin, trading fees, funding, position size, and margin mode mean the actual liquidation price is different.

**Q4: Is liquidation based on Last Price?**
Do not assume so.
For perpetual futures, the platform risk engine may rely on mark/index-based reference prices. Always check the specific contract information displayed by MSX.

**Q5: Is isolated margin safer than cross margin?**
Isolated margin contains the margin allocated to one position more clearly.
Cross margin can use more eligible account balance to support positions, but that means more account capital may be exposed.

**Q6: Can I move the liquidation price?**
Adding margin, reducing position size, or lowering effective leverage can generally increase the liquidation buffer.
The exact effect depends on the contract and margin mode.

**Q7: Can funding fees cause liquidation?**
Yes.
If your position pays funding, those payments reduce equity and can move the account closer to the maintenance margin threshold.

**Q8: What happens when liquidation starts?**
The platform risk engine may take control of the position and close or reduce it to prevent further losses from exceeding available collateral.

**Q9: What is ADL?**
Auto-Deleveraging is an additional risk-management process used during extreme liquidation conditions.
It is different from a normal user stop-loss.

**Q10: Are MSX stock perpetuals real stocks?**
No. MSX describes RWA perpetuals as contracts tied to stock-token indexes that allow leveraged long or short exposure. They should not be treated as direct ownership of traditional shares.

**Q11: Why did my liquidation price change?**
Possible reasons include:
- Funding payments
- Additional margin
- Margin withdrawal
- Position-size changes
- Cross-margin account equity changes
- Other open positions
- Updated maintenance margin requirements

**Q12: What leverage should beginners use?**
There is no universally safe leverage.
Lower leverage creates more room for adverse price movement, while higher leverage moves liquidation risk closer to the entry price.

---

## ✅ Conclusion: Liquidation Price Is a Risk Boundary, Not a Target
The key idea behind MSX liquidation is:

`Position Losses Reduce Margin → Margin Approaches Maintenance Requirement → Liquidation Risk Increases → Risk Engine Can Force-Close the Position`

The actual liquidation price is affected by much more than leverage alone.

The most important inputs include:

`Entry Price + Position Size + Leverage + Maintenance Margin + Margin Mode + Fees + Funding + Account Equity`

A useful comparison is:

| Lower-Risk Setup | Higher-Risk Setup |
|---|---|
| Lower leverage | Maximum leverage |
| Smaller position | Large position relative to account |
| Isolated margin while learning | Cross margin without understanding account risk |
| Stop-loss well before liquidation | No stop-loss |
| Margin buffer | Nearly all equity committed |
| Check funding and mark price | Only watch candlestick last price |
| Reduce size around major events | Hold maximum leverage through earnings/FOMC |

If you are new to MSX, start by understanding the position panel before placing the trade. The platform currently supports perpetual trading and RWA derivatives, and leveraged products can result in the loss of the entire margin allocated to the position.

📌 **MSX Referral Code:** 1KSn77

🔗 **MSX Registration Link:**

https://msx.com/?code=1KSn77

Before opening your first leveraged position, check the liquidation price displayed by MSX itself rather than relying only on a simplified formula from an external article.

> ⚠️ **Risk Notice:** Perpetual futures, leveraged crypto products, and RWA derivatives involve substantial risk. Liquidation can result in the loss of part or all of the margin allocated to a trade, while cross margin can expose additional account equity. Maintenance margin, liquidation rules, contract specifications, fees, and product availability may change. This article is for educational and platform-operation purposes only and does not constitute investment, legal, or financial advice.
