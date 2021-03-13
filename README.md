# Analysing the offensive playing style of a defender based on defender's preferred foot
## About
- This repository aims to analyse the role of footedness on the playing style of a defender in a game of football.<br>
- The effect of the dominant foot of a player goes hand in hand with the position they play in and thus comparisons are drawn between left footed and right footed Left Center Backs. <br>
- Only Left and not Right Center Backs are considered for this investigative study because of varying opinions about the dominant foot of an LCBs.<br> 
- Since the scope of offensive playing style of a Center Back is majorly limited to attacking buildup, we only concentrate on the passing style of left vs right footed Left Center Backs. <br>

## Download Data
The entire [Data](https://drive.google.com/drive/folders/1uk9jFdjHnN0BZOjbXeB4eidDlwacuTG0?usp=sharing) for all the code notebooks is already formatted and organised in seperate sub-folders for direct use. Simply download the data from the link mentioned previously and make sure to keep the `code` and `data` folder in the same directory. <br>

## Overview of the Data Pre-Processing
Notebooks 1, 2 and 3 deal with the Data Preparation and Processing <br>
1. Here, the team formation data for the top 5 european leagues - English Premier League, Bundesliga, Serie A, Ligue 1 and La Liga for the 2017-18 season is extracted from https://fbref.com 
2. The team formation data and the [Wyscout Data](https://figshare.com/collections/Soccer_match_event_dataset/4415000/5) are processed to generate a dataset that's inclusive of the defensive lineup and it's footedness for each team and each match. This dataset contains a key that connects it to the event based spatio-temporal data, for each match.
3. These matches are then seperated and clustered into sub-categories based on their defensive lineup (4 defender formations and 3/5 defender formations). Multiple passing based attributes are also computed for defenders for each match.

## Overview of the Analysis Tasks
- Notebooks 4 to 9 deal with the analysis and visualizations to compare the passing behaviour between left and right Footed LCBs in three, four and five at the back formations. All of these comparisons have been generalised and tested for their statistical significance using the Z-Test for proportions. <br>
- These notebooks take into consideration - accurate and inaccurate - short, aerial, long and progressive passes. <br> 
- In order to quantify the value addition of these passes, the [`socceraction`](https://github.com/ML-KULeuven/socceraction) package's VAEP framework has been used. <br>
- Notebooks 8 and 9 analyse and visualize the LCBs using their passing metrics.

## Future Work
- Clustering defenders at each position using multiple passing metrics to provide insight into similarities and differences in playing style of defenders.
