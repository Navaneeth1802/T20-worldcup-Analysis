<h2>
  AIM:Create a Power-BI Dashborad,that can help us to evaluvate Player performances in 2022-T20 worldcup
</h2>
<h4>
  Dataset:CricInfo(Webscraping)<br>
  <br></br>
  Tools used:
  Python-Pandas(Data cleaning)
  <br></br>
  Power-BI(Data modeling,Dax measures,Visualisation)
</h4>
<p align=left><b>Dataset-overview</b>

- Table 1 [Batting Summary]
   - Columns:[Batsman name,Match,Runs scored in each match,Balls faced,Number of fours,Number of sixes,Battingpos,Strikerate,Out/notout]
   - Measures Created  [Total Runs,Avg Score,Avg ballsfaced,Total innings Dismissed,Boundry%]
- Table 2 [Bowling Summary]
   - Columns: [Bowler name,Match,Balls,Overs,noBalls,Runs conceded,Sixes,Fours,Wickets,Wides]
   - Measures Created [Bowling Economy,Dot Ball%,Total Wickets,Total Runs Conceded,Boudary Conceded]
- Table 3 [Match Summary]
   - Columns :[ground,team1,team2,winner,margin,match_id]
- Table 4 [Player_info]
    - Colums : [name,team,descrpiton,batting style,bowling style]

<h5>Pre-Processing Steps</h5>
- Removing null values
- Removing inconsistencies
- Creating new columns
<h6> Power Query </h6>
- Data validation
<h6> Data Modeling </h6>

  -  MatchSummary[match_id]&Bowlingsummary[match_id]
  
  -  MatchSummary[match_id]&Battingsummary[match_id]
     
  -  battingSummary[playername]&Playerinfo[playername]
     
  -  bowlingSummary[playername]&Playerinfo[playername]

  <h5>Visualisation</h5>
  <p><img src="https://github.com/user-attachments/assets/d112dab7-539d-4ed2-94b2-94c7b1493121"></p>

  <p><img src="https://github.com/user-attachments/assets/e761bc5c-ab55-4cac-9635-ee6b12535c02"></p>

  <p><img src="https://github.com/user-attachments/assets/13c6aaf6-a9be-4323-97f1-df40de2c9718"></p>

  <p><img src="https://github.com/user-attachments/assets/4ac4e08e-3216-4c7a-85cd-c7631d36de0c"></p>

  <p><img src="https://github.com/user-attachments/assets/a7d91c25-b21c-4d2b-a374-daafa040faa8"</p>

