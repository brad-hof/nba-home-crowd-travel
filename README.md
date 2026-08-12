# NBA Home vs Away Performance, Crowd Size & Travel Impact

In this Jupyter Notebook I use python and data from the **2024-25 NBA regular season** to answer:  
1. Does playing at home really boost win rates?
2. How does crowd size (attendance) influence performance?
3. Does long-distance travel hurt away teams?


## Visualizations
The four charts appear together on one screen at the end of the notebook where the **Team** dropdown updates the scatter / box / violin plots simultaneously while the bar chart always shows every team. 

I landed on these 4 visualizations because I believed they were the best way to directly and complementarily answer my project’s three core questions. Other options I considered (simple histograms, correlation heatmaps, line charts of rolling margins, or static facet grids) were less effective at showing both categorical comparisons and distributional shape at the same time.

1. **Grouped Bar Chart** (Home vs Away Win %): Shows the classic home-court advantage at a glance and per team.
2. **Scatter Plot** (Attendance vs Point Differential): Reveals whether bigger crowds lead to bigger margins. Color-coded by home/away and win/loss.
3. **Box Plot** (Point Differential by Travel Distance Bucket): Illustrates how fatigue from long travel hurts away performance.
4. **Violin Plot** (Win Margin by Attendance Level & Home/Away): Adds density information to show not just averages but the full spread of outcomes when crowds are small/medium/large.


## Summary
The trends in the final output prove the classic NBA wisdom: **home crowds matter, and travel hurts**.

Overall, this project strengthened my practical skills in the end-to-end sports analytics process. It was great experience cleaning and feature-engineering large game-level data (pandas, derived metrics such as Haversine travel distance and quantile bins for attendance/travel), designing multi-view interactive dashboards that support both league-wide patterns and team-level exploration (Plotly Express + ipywidgets), and choosing visualization types that match specific analytical questions.


## Insights
Next steps could include:
- Restrict (or compare across) specific seasons and add rest days, back-to-backs, time-zone crossings, and direction of travel.
- Statistical tests / regressions that control for team strength and opponent quality so the effects of crowd size and travel can be isolated more rigorously.
- Add geospatial travel-route maps, multi-season trend lines, and simple predictive models of win probability based on these factors.


## Final Interactive Dashboard
<img width="1606" height="487" alt="grouped_bar_chart" src="https://github.com/user-attachments/assets/7aa01882-1cb2-47a1-aac3-479475f37d64" />
<img width="1609" height="424" alt="scatter_plot" src="https://github.com/user-attachments/assets/85987028-6dbe-4001-880c-774ec03fa229" />
<img width="1612" height="422" alt="box_plot" src="https://github.com/user-attachments/assets/a00351aa-2017-427c-940a-afaf03b0bdcb" />
<img width="1612" height="407" alt="violin_plot" src="https://github.com/user-attachments/assets/845e8933-c9e7-4d83-b43c-99295cad930f" />
