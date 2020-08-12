# FootballPlayerFootedness
## About
- This repository aims to Analyse the role of Footedness on the Playing Style of a Defender in a game of Football.<br>
- The effect of the Dominant Foot of a Player goes hand in hand with the Position they play in and thus comparisons are drawn between Left Footed and Right Footed Left Center Backs. <br>
- Only Left and not Right Center Backs are considered for this investigative study because of the shortage of data for Left Footed LCBs.<br> 
- Since the scope of Offensive Playing Style of a Center Back is majorly limited to Passing only, we only concentrate on the Passing Style of Left vs Right Left Center Backs (LCBs). <br>

## Download Data
The entire [Data](https://drive.google.com/drive/folders/1cp88C71CKapTq6quW3iEsBpck32SrGq6?usp=sharing) for all the code notebooks is already formatted and organised in seperate sub-folders for direct use. Simply download the data from the link mentioned previously and make sure to keep the `code` and `data` folder in the same directory. 

## Overview of the Data Pre-Processing
Notebooks 1, 2 and 3 deal with the Data Preparation and Processing <br>
1. Here, the Team Formation data for the Premier League 2017-18 season is extracted by Scraping the [English Premier League Website](https://www.premierleague.com/match/22342) 
2. The scraped data and the [Wyscout Data](https://figshare.com/collections/Soccer_match_event_dataset/4415000/5) are processed to generate a Dataset that's inclusive of the defensive lineup and it's Footedness for each team and each match. This dataset contains a key that connects it to the Event based Spatio-Temporal Data, for each match.
3. These matches are then seperated and clustered into sub-categories based on their Defensive Lineup and it's Footedness. Multiple passing based attributes are also computed for defenders for each match.

## Overview of the Analysis Tasks
- Notebooks 4 to 9 deal with the Analysis and Visualizations to compare the Passing Behaviour between Left and Right Footed LCBs in 3,4 and 5 at the back Formations. All of these comparisons have been generalised and tested for their Statistical Significance using the Z-Test for Proportions. <br>
- These notebooks take into consideration all- Accurate and Inaccurate Normal, Aerial and Progressive Passes. <br> 
- In order to quantify the Value Addition of these passes, the [`socceraction`](https://github.com/ML-KULeuven/socceraction) package's VAEP Framework has been used. <br>
- Notebooks 8 and 9 analyse and visualize the LCBs using their Passing Metrics computed for the 17-18 P.L. Season.

## Future Work
- Clustering the LCBs using Passing Metrics, Footedness and Player Location Embeddings as features using various ML and DL based Clustering Algorithms.
