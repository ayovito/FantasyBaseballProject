# Uncovering fantasy baseball "breakout" players for the 2018 season

Hello and welcome. In this project I am going to use data from MLB Statcast (https://baseballsavant.mlb.com/statcast_search) and data from FanGraphs (http://www.fangraphs.com/) in an effort to use advanced metrics to uncover potential "breakout" players for the 2018 MLB season. The term "breakout" is relative because each player needs to be judged against the prevailing expectation of that player which is best described by their consensus draft position or auction dollar value. For instance calling Mike Trout a breakout candidate because he fits my model is a waste of time because he has already broken out. I'm more interested in those who are currently flying under the radar.

In this project, I will clean and merge both hitting and pitching data. On the hitting side, I will first look at xwOBA as it is one of the most encompassing statistics available today for expected production. wOBA is a rate statistic which attempts to credit a hitter for the value of each outcome (single, double, etc) rather than treating all hits or times on base equally. Batting average and OBP assumes all hits are created equal, slugging weights hits but not accurately and ignores other ways of reaching base. wOBA formulas change year to year because it is based on relative contributions to run scoring and runs scored vary from year to year.

The 2017 formula for wOBA = (0.693×uBB + 0.723×HBP + 0.877×1B + 1.232×2B + 1.552×3B + 1.979×HR) / (AB + BB – IBB + SF + HBP)

xwOBA is a metric that utilizes launch angle and exit velocity to assign a hit value to every batted ball and then translates that into "expected" wOBA. The major issue with xwOBA is that is doesn't take into account speed so those that derive value from their speed are overlooked in xwOBA. I will have to revisit that issue later in this project. 

On the pitching side, I'll create a similar model and look at xFIP and SIERA to see what players could breakout in 2018. 

FIP - statistic that estimates a pitcher's run prevention independent of the performance of their defense. FIP is based on outcomes that do not inolve defense; strikeouts, walks, hit by pitches, and home runs allowed. FIP then uses those statistics and approximates a pitcher's ERA assuming average outcomes on balls in play.

xFIP - differs from FIP in that it normalizes a pitcher's ome runs allowed based on their fly ball rate rather than simply using the raw number of home runs allowed.

SIERA - skill interactive ERA that quantifies a pitcher's performance by trying to eliminate factors the pitcher can't control by himself. But unlike xFIP, SIERA considers balls in play and adjusts for the type of ball in play.


Future iterations of the project will hopefully include:

Further exploring advanced batted ball profile statistics to further enhance my hitting model

Incorporating speed into my hitting model

Exploring specific pitch types and incorporate them into my pitching model

Comparing projected breakout players to their draft position or auction value

Further further iterations of the project:

Creating a 2018 projection model based off of expected playing time

Incorporate minor league numbers and create comparable players for when players are called up
