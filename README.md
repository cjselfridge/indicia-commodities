# Indicia Labs: Commodity Data Pipeline Project

**Project Goal:** Scope and develop a data collection system to extend Indicia's AI asset management into commodities.
**Focus:** Market research, investment universe definition, data sourcing, and algorithmic implementation.

---

## 1. Investment Universe (Market Research)
*Goal: Define the cross-section of liquid assets.*

### A. Tokenized Commodities (RWA)
*Source: rwa.xyz (Initial Screen)*

**Precious Metals**
- [ ] **Tether Gold (XAUT)** - *Peg: Gold (oz)*
- [ ] **Paxos Gold (PAXG)** - *Peg: Gold (oz)*
- [ ] **Matrixdock Gold (XAUm)** - *Peg: Gold (oz)*
- [ ] **Comtech Gold (CGO)** - *Peg: Gold (grams)*
- [ ] **tGold (TXAU)** (Aurus) - *Peg: Gold (grams)*
- [ ] **GOLD** (Gold Issuance Inc) - *Peg: Gold (oz)*
- [ ] **WisdomTree Gold Token (WTGOLD)** - *Peg: Gold (oz)*
- [ ] **VNX Gold (VNXAU)** - *Peg: Gold (grams)*
- [ ] **tSilver (TXAG)** (Aurus) - *Peg: Silver (grams)*
- [ ] **tPlatinum (TXPT)** (Aurus) - *Peg: Platinum (grams)*

**Agriculture**
- [ ] **JSOY** (Justoken) - *Peg: Soybeans (bushels)*
- [ ] **JSOY_OIL** (Justoken) - *Peg: Soybean Oil (pounds)*
- [ ] **JCOT** (Justoken) - *Peg: Cotton (pounds)*
- [ ] **JCORN** (Justoken) - *Peg: Corn (bushels)*
- [ ] **Teucrium Wheat Fund (WEAT.d)** (Dinari) - *Peg: Wheat Fund*

**Other/Mixed**
- [ ] **Mineral Vault I (MNRL)** - *Peg: Mineral Basket*

### B. Traditional Commodities (Futures/Spot)
*Target: Liquid commodities with >6 years of history*
- [ ] *Pending Research: Energy (Crude, Nat Gas)*
- [ ] *Pending Research: Industrial Metals (Copper, Aluminum)*

---

## 2. Data Scope (Variables to Collect)
*Goal: Identify predictive features for the AI model.*

| Data Type | Description | Potential Source | Status |
| :--- | :--- | :--- | :--- |
| **Market Data** | OHLCV, Order Book Depth | CoinGecko, Refinitiv | ⏳ Pending |
| **On-Chain Data**| Mint/Burn volume, Holder distribution | Etherscan, PolygonScan | ⏳ Pending |
| **Fundamental** | Inventory levels, Crop reports, Fed rates | USDA, EIA, Fred | ⏳ Pending |
| **Alternative** | Weather data, Satellite imagery | OpenWeatherMap | ⏳ Pending |

---

## 3. Data Landscape (Vendor Analysis)
*Goal: Select robust vendors and aggregate data.*

- **Tier 1 (Premium):** Bloomberg, CME Group
- **Tier 2 (Aggregators):** Nasdaq Data Link, Barchart
- **Tier 3 (Crypto/RWA Specific):** rwa.xyz API, CoinMarketCap

---

## 4. Algorithms & Implementation
*Goal: Adapt existing R/Python scripts for commodity APIs.*

- [ ] src/fetch_market_data.py
- [ ] src/clean_data.py
- [ ] src/store_data.py
