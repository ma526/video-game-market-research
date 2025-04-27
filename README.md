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



