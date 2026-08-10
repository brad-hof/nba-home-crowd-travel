# NBA Home vs Away Performance, Crowd Size & Travel Impact (2024-25 Regular Season)

In this Jupyter Notebook I use python and data from the **2024-25 NBA regular season** to answer:  
1. Does playing at home really boost win rates?
2. How does crowd size (attendance) influence performance?
3. Does long-distance travel hurt away teams?


## Visualization Technique
The four charts appear together on one screen at the end of the notebook. The **Team** dropdown updates the scatter/box/violin plots simultaneously while the bar chart always shows every team.
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


## Final Interactive Dashboard
<img width="1606" height="487" alt="grouped_bar_chart" src="https://github.com/user-attachments/assets/7aa01882-1cb2-47a1-aac3-479475f37d64" />
<img width="1609" height="424" alt="scatter_plot" src="https://github.com/user-attachments/assets/85987028-6dbe-4001-880c-774ec03fa229" />
<img width="1612" height="422" alt="box_plot" src="https://github.com/user-attachments/assets/a00351aa-2017-427c-940a-afaf03b0bdcb" />
<img width="1612" height="407" alt="violin_plot" src="https://github.com/user-attachments/assets/845e8933-c9e7-4d83-b43c-99295cad930f" />
