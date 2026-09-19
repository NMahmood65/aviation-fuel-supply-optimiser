# ✈️ European Jet Fuel Supply Chain & Hedging Optimiser

## 📌 Project Overview
The **European Jet Fuel Supply Chain & Hedging Optimiser** is an automated, end-to-end supply chain model built to manage aviation fuel operations across three major European hubs: Frankfurt (FRA), Dublin (DUB), and Geneva (GVA). 

Acting as a digital supply chain manager, this system forecasts daily flight demand, monitors inventory levels to prevent stock-outs, automatically schedules multi-modal deliveries (pipeline, marine cargo, and rail), and tracks global oil markets to alert the commercial team of cost-saving purchasing opportunities.

### 📊 Live Interactive Dashboard
**[🟢 Click here to explore the live, interactive Excel Dashboard on MS OneDrive](https://1drv.ms/x/c/c497cb947e251d94/IQCDRJMk8TqnRI2FCB-QVk5XAe92dxjsDEoXOSKIndQgojM?e=3yCntI)**

(Note: The link above provides full "view-only" access to the interactive KPI dashboard. You can use the drop-down filters at the top of the dashboard to filter the automated inventory drawdown by airport, and isolate the exact days the crack spread triggered a hedging alert.)

## 🎯 The Business Problem
Aviation fuel supply is highly volatile. Analysts must balance rigid storage capacities, fluctuating flight schedules, complex regional logistics, and unpredictable global oil prices. Relying on manual calculations for these variables often leads to over-ordering (causing logistical bottlenecks), under-ordering (risking fuel-outs), or buying fuel at peak market prices.

## 💡 The Solution
This project solves these challenges by combining operational logistics with financial market strategy into a single, automated engine.

### Phase 1: The "Master Rulebook" (Scalable Data Architecture)
Instead of hard-coding rules day-by-day, the system is built on a centralized master framework. It understands the physical and financial realities of each airport, including:
* Maximum fuel farm storage capacities.
* Minimum "Safety Stock" requirements (e.g., 5 days of reserve fuel).
* Supplier lead times and freight costs.
* **Business Value:** Highly scalable. If the company acquires a contract for a new airport tomorrow, a user only needs to input the new location's rules once, and the entire system instantly knows how to manage it.

### Phase 2: Automated Inventory Forecasting
The system acts as a proactive monitor for the fuel tanks. By analyzing a 30-day schedule of outbound flights, it calculates exactly how much fuel will be burned each day.
* It projects future inventory levels and identifies the exact day an airport will approach its critical safety threshold.
* Before the safety line is breached, it automatically calculates and triggers a restock order designed to safely fill the tanks back to maximum capacity without overflowing.
* **Business Value:** Eliminates the risk of an airport running out of fuel while ensuring capital isn't tied up in unnecessary excess inventory.

### Phase 3: Smart Multi-Modal Logistics
Ordering 25,000 tons of fuel requires entirely different logistics depending on geography. The system features a smart routing engine that selects the most efficient delivery method for the region:
* **Frankfurt (FRA):** Automatically schedules underground **Pipeline Batches** through the European CEPS network.
* **Dublin (DUB):** Automatically groups massive orders onto **Marine Cargo Ships (MR Tankers)**, recognizing that island supply chains require sea freight rather than dispatching hundreds of road trucks.
* **Geneva (GVA):** Automatically schedules heavy **Rail Block Trains** for efficient inland mountain transport.
* **Business Value:** Proves an understanding of real-world, multi-modal supply chains and ensures the most cost-effective transportation method is always utilized.

### Phase 4: Market Strategy & Financial Hedging
Supply management is also about protecting profit margins. This model integrates commercial trading strategies by tracking the daily global prices of unrefined Brent Crude Oil versus refined Jet Fuel.
* The system monitors the "Crack Spread" (the price gap between the two commodities).
* When the gap shrinks—indicating that jet fuel is temporarily underpriced relative to crude—the system flashes an automated `EXECUTE FORWARD HEDGE` alert.
* **Business Value:** Acts as a financial watchdog, automatically alerting the trading desk to "lock in" and pre-purchase fuel when market conditions offer the best savings.

### Phase 5: The Executive KPI Dashboard
To make thousands of rows of operational data instantly actionable for management, the model includes a clean, visual control panel.
* **Inventory Health Tracker:** A visual proof-of-concept showing fuel levels safely bouncing between maximum capacity and the safety-stock baseline, with zero stock-outs over a 30-day period.
* **Commercial Insights Board:** A dual-axis market chart that allows the commercial team to filter and isolate the exact days the algorithm recommended bulk fuel purchases.

## 🛠️ Tech Stack & Skills Demonstrated
* **Tools:** Advanced Microsoft Excel
* **Techniques:** Relational Data Modeling, Nested Logical Functions, Automated Reordering Triggers, Multi-Modal Logistics Scheduling, Financial Market Analysis, Interactive Dashboarding (PivotTables/PivotCharts).

***


