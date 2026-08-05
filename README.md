# NBA Home vs Away Performance, Crowd Size & Travel Impact (2024-25 Regular Season)

In this notebook I explore the **2024-25 NBA regular season** to answer:  
1. Does playing at home really boost win rates?
2. How does crowd size (attendance) influence performance?
3. Does long-distance travel hurt away teams?


## Visualization Technique
These four charts appear together on one screen. The **Team** dropdown updates three visualizations simultaneously. The bar chart always shows every team for easy league-wide comparison.
1. **Grouped Bar Chart** (Home vs Away Win %): Shows the classic home-court advantage at a glance and per team.
2. **Scatter Plot** (Attendance vs Point Differential): Reveals whether bigger crowds lead to bigger margins. Color-coded by home/away and win/loss.
3. **Box Plot** (Point Differential by Travel Distance Bucket): Illustrates how fatigue from long travel hurts away performance.
4. **Violin Plot** (Win Margin by Attendance Level & Home/Away): Adds density information to show not just averages but the full spread of outcomes when crowds are small/medium/large.


## Plotly Library
I chose **Plotly** (with `plotly.express`) + `ipywidgets` because:
- It creates great interactive & web-ready charts.
- Handles thousands of games instantly and supports WebGL for smooth performance.
- Open-source, actively maintained, and integrates perfectly with Jupyter notebooks.
- Allows multiple charts to update together via widgets.

Installation (run once): `pip install plotly ipywidgets`


## Summary / Insights
These trends prove the classic NBA wisdom: **home crowds matter, and travel hurts**.
Next steps could include building a prediction model for next season’s home advantage.
