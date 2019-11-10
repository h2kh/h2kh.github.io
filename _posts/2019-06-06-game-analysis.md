---
layout: post
title: "PC vs Console gaming: the battle continues"
subtitle: "Exploratory analysis on video games from the last 20 years"
nottableau: 'true'
---


This **[Kaggle dataset](https://www.kaggle.com/egrinstein/20-years-of-games)** contains information on over 18,000 video games released between 1996 and 2016. This data was collected from IGN.com which is a popular entertainment review website.

Some of the things that I will investigate in this project are popular publishing platforms and common genres. We'll illustrate our findings with some charts and diagrams.

(Note: the Kaggle dataset this project was based on has been taken down by the uploader. However, you can still see my analysis in the linked notebook without any issues.)

Feel free to look through the code in my **[Jupyter notebook](https://nbviewer.jupyter.org/github/h2kh/video_game_exploratory/blob/master/game-analysis.ipynb)**. I have used the following Python libraries in this project: Pandas, Matplotlib, and Seaborn.

Here is a snapshot of what the data looks like: 

{:refdef: style="text-align: center;"}
![Data]({{ site.baseimg }}/assets/Capture15.JPG){:height="300px" width="700px"}
{: refdef}

We can see that the number of releases increases from August to November in the lead up to Black Friday and Christmas before a sharp drop in December. The number of games released per year rises steadily until 2008 before dropping pretty quickly. Given the increasing popularity of games and the advent of new platforms like mobile gaming over the last few years, this seems unlikely. Further investigation is needed but a simple explanation could be the fact that IGN (the data source) just isn't that popular a game rating website as it used to be (because of competitors like Steam).

{:refdef: style="text-align: center;"}
![Data]({{ site.baseimg }}/assets/Capture17.png){:height="650px" width="900px"}
{: refdef}

The distribution for the game ratings/scores appear to be skewed to the left with a majority of the scores in the 6 to 9 range with mean at 6.95.

{:refdef: style="text-align: center;"}
![Data]({{ site.baseimg }}/assets/Capture18.png)
{: refdef}

Almost 20% of all games were created for the PC. This number, however, pales in comparison to the nearly 40% that were created for consoles.

{:refdef: style="text-align: center;"}
![Data]({{ site.baseimg }}/assets/Capture12.png)
{: refdef}

We can see the trends over the years in the average scores for each genre in the following diagram. The RPG (role-playing game) genre has done consistently well over the years (apart from 1996) while the Action genre has generally languished in the 6 to 7 range.

{:refdef: style="text-align: center;"}
![Data]({{ site.baseimg }}/assets/Capture11.png)
{: refdef}

{:refdef: style="text-align: center;"}
![Data]({{ site.baseimg }}/assets/Capture13.png)
{: refdef}

{:refdef: style="text-align: center;"}
![Data]({{ site.baseimg }}/assets/Capture14.png)
{: refdef}




