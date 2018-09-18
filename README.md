#Was just messing around with markdown so made everything into comments 

#*italic*
#**bold**
#***bold italic***

### Just messing around with this video game sales data set from kaggle.com

#* had some trouble originally figuring out the process of uploading data sets

#* Still a work in progress being able to manipulate them

#* The plot isn't meaningful or pretty by any means but just messing around with the process of working with matplotlib and making sure I could get one made for now 

import pandas as pd

import matplotlib.pyplot as plt

data = pd.read_csv('vgsales.csv')

print(data.head())

print(data.describe())

print(data['Publisher'].value_counts())

plt.plot(data['NA_Sales'])

plt.show()

   Rank                      Name Platform    Year         Genre Publisher  \
0     1                Wii Sports      Wii  2006.0        Sports  Nintendo   
1     2         Super Mario Bros.      NES  1985.0      Platform  Nintendo   
2     3            Mario Kart Wii      Wii  2008.0        Racing  Nintendo   
3     4         Wii Sports Resort      Wii  2009.0        Sports  Nintendo   
4     5  Pokemon Red/Pokemon Blue       GB  1996.0  Role-Playing  Nintendo   

   NA_Sales  EU_Sales  JP_Sales  Other_Sales  Global_Sales  
0     41.49     29.02      3.77         8.46         82.74  
1     29.08      3.58      6.81         0.77         40.24  
2     15.85     12.88      3.79         3.31         35.82  
3     15.75     11.01      3.28         2.96         33.00  
4     11.27      8.89     10.22         1.00         31.37  
               Rank          Year      NA_Sales      EU_Sales      JP_Sales  \
count  16598.000000  16327.000000  16598.000000  16598.000000  16598.000000   
mean    8300.605254   2006.406443      0.264667      0.146652      0.077782   
std     4791.853933      5.828981      0.816683      0.505351      0.309291   
min        1.000000   1980.000000      0.000000      0.000000      0.000000   
25%     4151.250000   2003.000000      0.000000      0.000000      0.000000   
50%     8300.500000   2007.000000      0.080000      0.020000      0.000000   
75%    12449.750000   2010.000000      0.240000      0.110000      0.040000   
max    16600.000000   2020.000000     41.490000     29.020000     10.220000   

        Other_Sales  Global_Sales  
count  16598.000000  16598.000000  
mean       0.048063      0.537441  
std        0.188588      1.555028  
min        0.000000      0.010000  
25%        0.000000      0.060000  
50%        0.010000      0.170000  
75%        0.040000      0.470000  
max       10.570000     82.740000  
Electronic Arts                           1351
Activision                                 975
Namco Bandai Games                         932
Ubisoft                                    921
Konami Digital Entertainment               832
THQ                                        715
Nintendo                                   703
Sony Computer Entertainment                683
Sega                                       639
Take-Two Interactive                       413
Capcom                                     381
Atari                                      363
Tecmo Koei                                 338
Square Enix                                233
Warner Bros. Interactive Entertainment     232
Disney Interactive Studios                 218
Unknown                                    203
Midway Games                               198
Eidos Interactive                          198
505 Games                                  192
Microsoft Game Studios                     189
Acclaim Entertainment                      184
D3Publisher                                184
Vivendi Games                              164
Codemasters                                152
Idea Factory                               129
Deep Silver                                122
Nippon Ichi Software                       105
Zoo Digital Publishing                     104
Majesco Entertainment                       92
                                          ... 
Simon & Schuster Interactive                 1
Legacy Interactive                           1
PopTop Software                              1
Milestone                                    1
Pow                                          1
Black Label Games                            1
Berkeley                                     1
GameTek                                      1
Ongakukan                                    1
RED Entertainment                            1
Playmates                                    1
Merscom LLC                                  1
Glams                                        1
Takuyo                                       1
mixi, Inc                                    1
Palcom                                       1
CokeM Interactive                            1
Gameloft                                     1
The Learning Company                         1
Visco                                        1
Nexon                                        1
Codemasters Online                           1
CCP                                          1
Kando Games                                  1
PM Studios                                   1
WayForward Technologies                      1
On Demand                                    1
Fields                                       1
Giza10                                       1
Havas Interactive                            1
Name: Publisher, Length: 578, dtype: int64

