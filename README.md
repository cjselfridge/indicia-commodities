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
*Selection Criteria: High liquidity & >10 years of historical data availability*
**Energy**
- [ ] **Crude Oil WTI** (Ticker: CL) - *Global benchmark, high volatility*
- [ ] **Crude Oil Brent** (Ticker: B) - *European benchmark.*
- [ ] **Natural Gas** (Ticker: NG) - *Highly weather-dependent.*
- [ ] **Heating Oil** (Ticker: HO) - *Seasonal demand driver.*
- [ ] **RBOB Gasoline** (Ticker: RB) - *Consumer demand proxy.*

**Metals**
- [ ] **Gold** (Ticker: GC) - *Inflation hedge*
- [ ] **Silver** (Ticker: SI) - *Industrial + precious.*
- [ ] **Copper** (Ticker: HG) - *Key economic indicator*
- [ ] **Platinum** (Ticker: PL) - *Auto demand*

**Agriculture**
- [ ] **Corn** (Ticker: ZC) - *Biofuel & feed demand*
- [ ] **Soybeans** (Ticker: ZS) - *Global trade (China/US)
- [ ] **Wheat** (Ticker: ZW) - *Geopolitical sensitivity.*
- [ ] **Coffee** (Ticker: KC) - *Soft commodity, weather sensitive.*

---

## 2. Data Scope (Variables to Collect)
*Mapping Indicia's Crypto Framework to Commodities*

| Indicia Category | Commodity Equivalent | Specific Variables | Potential Source |
| :--- | :--- | :--- | :--- |
| **Market Data** | Futures Market | Open, High, Low, Close (OHLC), Volume, **Open Interest**, **Term Structure** (Contango/Backwardation). | CME, Yahoo Fin |
| **Network Usage** | Physical Supply/Demand | **Inventory Levels** (e.g., Cushing Oil Stocks), Import/Export data, Refinery utilization rates. | EIA, USDA |
| **Blockchain Data** | Position Data | **Commitment of Traders (COT)** reports (shows Hedge Fund vs. Producer positioning). | CFTC.gov |
| **News/Social** | Macro/Event Data | Fed Rate decisions, OPEC+ meeting minutes, Extreme weather alerts (NOAA). | Fed, Refinitiv |
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
