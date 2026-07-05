url: https://samvermeir1606.github.io/SpaceTraderSimulatorWebGame/

# 🚀 CosmoTrader OS v3.1

> "If deep-space commerce was managed on a salvaged Windows 98 terminal."

CosmoTrader OS is a lightweight, zero-dependency, single-file procedural space-trading economy simulator built entirely in plain HTML, CSS, and vanilla JavaScript. Designed to run completely client-side, it utilizes local JSON import/export profiles instead of a backend database, making it 100% portable and instantly playable on both desktop and mobile web browsers.

---

## 📟 Executive Summary & Core Loop

You are an independent merchant captain navigating a procedurally generated star system node cluster. Your objective is simple but demanding: build your operational enterprise from a humble $1,500 seed loan up to a net liquid corporate valuation of **$250,000 Credits** to secure your luxury retirement package.

The game is a tight economic balance of supply and demand manipulation, spatial fuel routing, hull degradation maintenance, factory real estate acquisition, and corporate quest completion.

---

## 🔧 Strategic Mechanics Matrix

### 1. Market Price Elasticity & Delayed Impact
The star system features a reactive, fluid economy. However, local markets guarantee their listed exchange values for your entire dock stay. Price shifts caused by your transactions are stored in a temporary memory buffer:
* **Buying** drains local supply, scaling prices **upwards** (+1.5% of base value per unit).
* **Selling** floods the market, dumping commodity value (-1.5% of base value per unit).
The cumulative economic impact of your trades is calculated and permanently baked into the galactic ledger *only after* you initiate a hyper-jump warp or spend a turn waiting in the hangar.

### 2. Space-Age Real Estate (Factory Assets)
Spend capital to construct production infrastructure tied directly to planetary specializations (e.g., *Hydroponic Greenhouses* on Agricultural worlds, *Deep Core Drillers* on Mining worlds). Factories accumulate 2 units of automated cargo reserves every cycle you jump or wait.
* **Extraction:** Land at the factory node to lift your inventory into your cargo bays for free.
* **Quantum Beaming Matrix:** Pay a premium sub-space transmission fee per item to beam factory stock directly into your ship's hold from anywhere in the cluster—allowing you to cash in on breaking market surges before they expire.

### 3. Corporate Logistics Boards
Contracts boards generate high-paying delivery quests locked permanently to the **historical maximum baseline** of an asset plus a +30% corporate premium. 
* **The Speculation Play:** Smart traders accept premium contracts and wait for a localized market crash (like an Ore Supply Surge) to buy the cargo for cheap, fulfilling the job for a massive return on investment.
* **The Ticking Clock:** Contracts feature decay counters. Jumps or port waits tick down their lifespan. If they expire, the file is scrubbed from the board.

### 4. Specialized Crew Manifest
Reinvest your capital into enlistment contracts to staff your ship with dedicated officers, unlocking powerful passive modifiers:
* **👨‍✈️ Chief Navigator:** Reduces warp drive fuel consumption per hyper-jump up to -50%.
* **💼 Trade Broker:** Slashes local market spread transaction fees down to 0%.
* **🔧 Chief Engineer:** Patches defensive grids, reducing structural warp damage up to -75%.
* **👩‍🔬 Science Officer:** Expands sensor ranges, adding up to +5 cycles to contract lifespans.
* **🛡️ Security Chief:** Mitigates risk, providing up to a +35% credit yield on completed jobs.

---

## 🎨 Retro UX Features & Architecture

* **Responsive Bottom Taskbar:** Bypasses clumsy multi-column constraints on touch devices. Adaptive flexible tabs simulate a retro OS taskbar that scales cleanly across mobile phones, tablets, or monitors.
* **3-Line Ticker Tape:** Surfaces sensor telemetry. Line 1 monitors active radar anomalies and forecasts upcoming cluster events; lines 2 and 3 act as a historical transaction receipt log.
* **Database-less Diagnostics Chart:** Utilizes the HTML5 Canvas API to plot a real-time running history of your capital trajectory. Graph data sits persistently inside the state object, meaning your financial charts are fully preserved when you save your game.
* **Pure Math Sound Synthesis:** Implements the native web browser Audio Context API. Highs, lows, and fanfares are generated using algorithmic sound frequencies—**requiring zero external `.mp3` or `.wav` assets**.

---

## 💾 Saving and Loading

Because this project uses no database, you are the database manager:
1. **Export:** Click `Export` to generate and download a serialized `.json` data file to your device.
2. **Import:** Click `Import`, choose your save file, and your ship, ledger, graph history, and unique galaxy layout are instantly reconstructed.
3. **End Run:** If you run out of fuel or funds, use the `End Run` terminal to liquidate the enterprise and review an advanced audit performance statement.

---

## 🚀 Deployment Instructions

### Local Execution
Simply clone or download this repository, and double-click `index.html`. It will run instantly inside any web browser.

### Hosting via GitHub Pages
To host this online for free without setting up automated Node runners:
1. Push your `index.html` to a public GitHub repository.
2. Go to **Settings > Pages** inside your repository.
3. Under **Build and deployment**, set the Source dropdown to **Deploy from a branch**.
4. Set your target branch to `main` (or `master`) and the folder path to `/ (root)`.
5. Click **Save**. Your simulator will be live at `https://yourusername.github.io/your-repo-name/` in under two minutes!
