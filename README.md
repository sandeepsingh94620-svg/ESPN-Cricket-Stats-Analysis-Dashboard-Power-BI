📊 ESPN-Cricket-Stats-Analysis-Dashboard-Power-BI
Analyzes ESPN cricket data to reveal insights on player performance, team comparisons, and match outcomes. Highlights batting and bowling KPIs like strike rate, average, economy, wickets, and runs. Interactive filters enable analysis by player, team, tournament, match type, and season trends.

Live Link: https://app.powerbi.com/links/d8-NeYVWZ8?ctid=e0d6db51-483a-41a8-bc9f-57219bf8811f&pbi_source=linkShare&bookmarkGuid=bdcba38d-9f0f-4d1b-b498-90b5c5d0900b

💻 Technologies Used
• 📊 Power BI Dashboard
• 🔄 Power Query (Data Cleaning & Transformation)
• 🎨 Canva (Images & Background Design)
• 🧮 DAX (KPIs & Calculations)
• 🗂️ Data Modeling

🗂️ Data Source
• 🌐 Web Scraping (ESPN Cricket Data) to collect match, player, and team performance statistics.

# Dax Calculation
Absolute Deviation = ABS(Batting[Deviation]) 
Category = LOOKUPVALUE('Strike Rate Table'[Category],'Strike Rate Table'[Strike Rate],Batting[SR])
Deviation = Batting[Runs]-AVERAGE(Batting[Runs]) 
Rank = RANKX(ALL(Batting),Batting[SR],,DESC,Dense)
Squared Deviation = POWER(Batting[Deviation],2) 

