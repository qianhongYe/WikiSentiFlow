# WikiSentiFlow

## Introduction

This widget is used to show the changes of sentiment scores for Wikipedia entities (concepts) over time. It shows 25%, 50% (median), 75% quantile of sentiment score for each month to present the sentiment distribution.

Wikipedia entities contains entities in Wikipedia Article and Wikipedia Talk. Talk page is an area for editors to discuss about corresponding article, which can be visited from upper left side of article page.

This widget includes entities both People and Events. The date for people indicates birth date, while the date for events indicates occurrance date.

The text of Articles and Talks is extracted from Wikipedia Dump, and time stamps are extracted from DBPedia.

The scores are calculated with term frequency for sentiment words based on certain lexicons (OL, MPQA, LIWC, ANEW). For ANEW we take valency into account too.

## How to use it

1. You can use the link below to run this jupyter notebook with mybinder.

https://mybinder.org/v2/gh/qianhongYe/WikiSentiFlow/master

It takes around 10 mins to prepare the environment.

2. Click time_widgets_1.ipynb in the home page to open the notebook.

3. You can open Appmode to ignore the codes by clicking "Appmode" in toolbar (recommended for general user). Alternatively, you can choose "Run All" inside Cell menu without entering appmode (recommended for programmer).

Now you can operate with the widget.

## What can be seen with the widget

After selecting value for each field and click "Go" button, it comes up with plot.

For each run there will be two plots sharing x-axis. 

The first plot is the number of entities matching the setting.

The second plot shows a red line with purple shadows representing the corresponding scores. 

The red line presents median (50% quantile) of scores based on your settings.

And the shadows cover 25% to 75% quantile of the scores.

If rolling average is ticked, then the shadows and red line refer to rolling average of 25%, 50%, 75% quantile.

In the bottom you will get the data characteristics for the current run.

The time is splited with month as unit.

## Run it locally

If you want to run it locally, you need to install libraries listed in environment.yml with version showed in requirements.txt. Dataset can download dataset in the following link.

https://www.dropbox.com/sh/mt7by5f1wgl6n3z/AACddwkFPq5lPpH3ry83MgSDa?dl=0

