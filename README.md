# video-game-market-research

I am trying to apply all the things I learned about spreadsheets and data analytics so far to study video game sales worldwide!

I picked up datasets of a company that is creating video games and I am trying to research the market to better understand what kind of video games are in demand and how the trends are evolving. I will explore a custom dataset and quantify several factors that affect video game sales worldwide. The dataset contains information about sales of video games launched in year 2018, with total sales calculated from their launch date up until 08/22/2024.

Data Sources
The first dataset in this lab contains data extracted from VGChartz.com You can find the dataset here:-https://drive.google.com/file/d/1ri9Zg2wquerFt8ngWi6fYsQhT2_nkv2e/view


The second dataset in this lab contains data from the 
Popularity of Games on Steam
 dataset. you can find it here:-https://www.kaggle.com/datasets/michau96/popularity-of-games-on-steam?resource=download

Fields
Every row (observation) in the dataset represents a video game and the columns (features) are: 

● Name - The game's name

● Platform - Platform of the game's release (i.e. PC,PS4, etc.)

● Genre - Genre of the game

● Publisher - Publisher of the game

● NA_Sales - units sold in North America (in millions)

● EU_Sales - units sold in Europe (in millions)

● JP_Sales - units sold in Japan (in millions)

● Other_Sales - units sold in the rest of the world (in millions)

● Global_Sales - Total units sold worldwide (in millions)

● Release_Date - The game's release date.



First part:-
There are 1569 rows in the dataset and 10columns.

The numerical values in the dataset are the following:-NA_Sales,EU_Sales,JP_Sales,Other_Sales,Global_Sale,Release_Date

all the categorical features in the dataset are the following: Name,Platform,Genre,Publisher

1.Used filtering:- a)First I tried to Remove games with an empty value in the Global_Sales column and have less than 0.1M global sales.For that:-I  Filtered the Global_Sales column:Clicked the filter button.Filtered by Blanks first and deleted those rows.Then Filtered by Numbers:Choosed "Less than" 0.1 and deleted those rows too.

for deletion:-Click the first row number (the first filtered row).Then press Shift on your keyboard and click the last row number.This will select everything between.Once all the rows are highlighted (you'll see them shaded), you can:Right-click on any selected row number.Choose Delete Row.

 b)copied the result to sheet1.

 c)Tried to Apply named ranges to each column so you can easily call them in the next upcoming steps if needed.
  Open your Google Sheet.

Selected the first column:

For example, we have to click on the first data cell under your header (not the header itself).

Drag down to select all the values in that column.

Go to the menu at the top:

Click Data → then Named ranges.

A panel will open on the right side called Named ranges.

In the panel:

Type a name for the range (example: Global_Sales).

Click Done.

Repeated steps 2–5 for all the columns.

d)Trying to find on what date earliest game was released?Click the Release Date column.

Went to Data → Sort A → Z (Oldest to Newest).

The first row after sorting will show the earliest release date and the game.
It's 2018-01-01

e)How many rows in filtered dataset? 205


2)Regional sales:- a)suming up total sales for each region
Used this formula for North America sales:-=SUM(NA_Sales) and similar way for all sales
	Region	All sales	
	North America	60.53	millions of units
	Europe	48.18	millions of units
	Japan	8.4	millions of units
	Rest of the world	16.86	millions of units
	Global	133.97	millions of units

 3)Top categories
 a)calculating global sales for top three categories with the following formula:-=SUMIFS(Global_Sale, Platform, "PS4", Release_date, ">2010")
 same formula for other two categories
 Top 3 platforms by global sales	Global Sales
PS4	78.43
XOne	34.57
NS	16.74

b)Calculating the number of games published on each of the platforms in cells using formula
=COUNTIF(Platform,"PS4")
Top 3 platforms by global sales	Global Sales	Number of Games
PS4	78.43	88
XOne	34.57	48
NS	16.74	50

d)

=SUMIFS(Global_Sale,Genre,"Shooter",Release_Date,">2010")
c)


