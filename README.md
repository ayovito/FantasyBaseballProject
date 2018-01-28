# Uncovering potential fantasy baseball breakout players for the 2018 season

Hello and welcome. In this project, I am going to use data from MLB Statcast (https://baseballsavant.mlb.com/statcast_search) and data from FanGraphs (http://www.fangraphs.com/) in an effort to use advanced metrics to uncover potential breakout players for the 2018 MLB season. The term "breakout" is relative because each player needs to be judged against the prevailing expectation of that player which is best described in consensus draft position. For instance calling Mike Trout a breakout candidate because he fits my model is a waste of time because he has already broken out. I'm more interested in those who are currently flying under the radar.

In this project, I will clean and merge both hitting and pitching data. On the hitting side, I will first look at xwOBA as it is one of the most encompassing statistics available today for expected production. The major issue with xwOBA is that is doesn't take into account speed so those that derive value from their speed are overlooked in xwOBA. I will have to revisit that issue later in this project. 

On the pitching side, I'll create a similar model and look at xFIP and SIERA to see what players could breakout in 2018. 

Future iterations of the project will hopefully include:
Further exploring advanced batted ball profile statistics to further enhance my hitting model
Incorporating speed into my hitting model
Exploring specific pitch types and incorporate them into my pitching model
Comparing projected breakout players to their draft position or auction value

Further further iterations of the project:
Creating a 2018 projection model based off of expected playing time
Incorporate minor league numbers and create comparable players for when players are called up
