# Charting the Rise of Small-Ball in NBA
Clusters NBA Player-Seasons since 2013-2014 &amp; Analyzes Lineup Types

### Methodology

With NBA tracking data, I was able to use Sci-Kit Learn's linear discriminant analysis to reduce the data into two dimensions. From there, I used spectral clustering to determine offensive positions. Positional separation (via the silhouette coefficient) was by far the highest with 3 clusters, and this strongly corresponded to a ball-handlers/wings/bigs model. Defensive positions were broadly similar, and I use guard/forward/interior terminology.

![Giannis](https://github.com/mattignal/SmallBallNBA/blob/master/giannis.jpg)

### Trends

From here, I used lineup data from the NBA to look at the different types of lineups. I used a simple definition for distinguishing between traditional and small-ball lineups: If a lineup had two or more bigs, it was "traditional". If there was one or fewer bigs, it is a "small-ball" lineup.

![GrowthOfSmallBall](https://github.com/mattignal/SmallBallNBA/blob/master/GrowthofSmall-ball.png)

### Small vs. Traditional

There are some signs that suggest small-ball lineups tend to "beat" traditional lineups in the modern NBA: A) The fact that it is fast-growing, and coaches use it more in the playoffs, B) Many of the best lineups are small (continued)

[NBA Lineup Types](http://rpubs.com/matthewignal/300987) <- Click for Interactive Plot
![NBA Lineup Types](https://github.com/mattignal/SmallBallNBA/blob/master/LineupTypes.png)

C) Whenever we reduce the overall dataset to the most used lineups (such as in the NBA.com data, shown below) or by using only lineups with the BPM leader, small-ball lineups slightly outclass traditional ones.

![SmallvsBig](https://github.com/mattignal/SmallBallNBA/blob/master/smallvsbig.png)

D) Small-ball lineups outperformed traditional lineups when matched up head-to-head in the regular season. However, the trend reversed in the playoffs, albeit on a much smaller sample size.

![HeadtoHead](https://github.com/mattignal/SmallBallNBA/blob/master/Possession Weighted Net Ratings.png)

### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [ggplot](http://ggplot.yhathq.com/)

There is also plot generation using [RStudio](https://www.rstudio.com/).

You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)
