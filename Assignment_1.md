```python
import pandas as pd
```


```python
# data about happiness counter around the world-2019
data1=pd.read_csv("/Users/adityakatheeth/Desktop/Datasets/2019.csv")
```


```python
# data about Chess game
data2=pd.read_csv("/Users/adityakatheeth/Desktop/Datasets/games.csv")

```


```python
# data about netflix_titles
data3=pd.read_csv("/Users/adityakatheeth/Desktop/Datasets/netflix_titles.csv")


```


```python
# data about Solar power generation from a single plant
data4=pd.read_csv("/Users/adityakatheeth/Desktop/Datasets/Solarplant.csv")


```


```python
# data about wine_reviews
data5=pd.read_csv("/Users/adityakatheeth/Desktop/Datasets/winereview.csv")


```


```python
data3.info

```




    <bound method DataFrame.info of        show_id     type                                        title  \
    0     81145628    Movie      Norm of the North: King Sized Adventure   
    1     80117401    Movie                   Jandino: Whatever it Takes   
    2     70234439  TV Show                           Transformers Prime   
    3     80058654  TV Show             Transformers: Robots in Disguise   
    4     80125979    Movie                                 #realityhigh   
    ...        ...      ...                                          ...   
    6229  80000063  TV Show                                 Red vs. Blue   
    6230  70286564  TV Show                                        Maron   
    6231  80116008    Movie       Little Baby Bum: Nursery Rhyme Friends   
    6232  70281022  TV Show  A Young Doctor's Notebook and Other Stories   
    6233  70153404  TV Show                                      Friends   
    
                          director  \
    0     Richard Finn, Tim Maltby   
    1                          NaN   
    2                          NaN   
    3                          NaN   
    4             Fernando Lebrija   
    ...                        ...   
    6229                       NaN   
    6230                       NaN   
    6231                       NaN   
    6232                       NaN   
    6233                       NaN   
    
                                                       cast  \
    0     Alan Marriott, Andrew Toth, Brian Dobson, Cole...   
    1                                      Jandino Asporaat   
    2     Peter Cullen, Sumalee Montano, Frank Welker, J...   
    3     Will Friedle, Darren Criss, Constance Zimmer, ...   
    4     Nesta Cooper, Kate Walsh, John Michael Higgins...   
    ...                                                 ...   
    6229  Burnie Burns, Jason Saldaña, Gustavo Sorola, G...   
    6230  Marc Maron, Judd Hirsch, Josh Brener, Nora Zeh...   
    6231                                                NaN   
    6232  Daniel Radcliffe, Jon Hamm, Adam Godley, Chris...   
    6233  Jennifer Aniston, Courteney Cox, Lisa Kudrow, ...   
    
                                           country         date_added  \
    0     United States, India, South Korea, China  September 9, 2019   
    1                               United Kingdom  September 9, 2016   
    2                                United States  September 8, 2018   
    3                                United States  September 8, 2018   
    4                                United States  September 8, 2017   
    ...                                        ...                ...   
    6229                             United States                NaN   
    6230                             United States                NaN   
    6231                                       NaN                NaN   
    6232                            United Kingdom                NaN   
    6233                             United States                NaN   
    
          release_year    rating    duration  \
    0             2019     TV-PG      90 min   
    1             2016     TV-MA      94 min   
    2             2013  TV-Y7-FV    1 Season   
    3             2016     TV-Y7    1 Season   
    4             2017     TV-14      99 min   
    ...            ...       ...         ...   
    6229          2015        NR  13 Seasons   
    6230          2016     TV-MA   4 Seasons   
    6231          2016       NaN      60 min   
    6232          2013     TV-MA   2 Seasons   
    6233          2003     TV-14  10 Seasons   
    
                                                  listed_in  \
    0                    Children & Family Movies, Comedies   
    1                                       Stand-Up Comedy   
    2                                              Kids' TV   
    3                                              Kids' TV   
    4                                              Comedies   
    ...                                                 ...   
    6229  TV Action & Adventure, TV Comedies, TV Sci-Fi ...   
    6230                                        TV Comedies   
    6231                                             Movies   
    6232           British TV Shows, TV Comedies, TV Dramas   
    6233                     Classic & Cult TV, TV Comedies   
    
                                                description  
    0     Before planning an awesome wedding for his gra...  
    1     Jandino Asporaat riffs on the challenges of ra...  
    2     With the help of three human allies, the Autob...  
    3     When a prison ship crash unleashes hundreds of...  
    4     When nerdy high schooler Dani finally attracts...  
    ...                                                 ...  
    6229  This parody of first-person shooter games, mil...  
    6230  Marc Maron stars as Marc Maron, who interviews...  
    6231  Nursery rhymes and original music for children...  
    6232  Set during the Russian Revolution, this comic ...  
    6233  This hit sitcom follows the merry misadventure...  
    
    [6234 rows x 12 columns]>




```python
data3.head

```




    <bound method NDFrame.head of        show_id     type                                        title  \
    0     81145628    Movie      Norm of the North: King Sized Adventure   
    1     80117401    Movie                   Jandino: Whatever it Takes   
    2     70234439  TV Show                           Transformers Prime   
    3     80058654  TV Show             Transformers: Robots in Disguise   
    4     80125979    Movie                                 #realityhigh   
    ...        ...      ...                                          ...   
    6229  80000063  TV Show                                 Red vs. Blue   
    6230  70286564  TV Show                                        Maron   
    6231  80116008    Movie       Little Baby Bum: Nursery Rhyme Friends   
    6232  70281022  TV Show  A Young Doctor's Notebook and Other Stories   
    6233  70153404  TV Show                                      Friends   
    
                          director  \
    0     Richard Finn, Tim Maltby   
    1                          NaN   
    2                          NaN   
    3                          NaN   
    4             Fernando Lebrija   
    ...                        ...   
    6229                       NaN   
    6230                       NaN   
    6231                       NaN   
    6232                       NaN   
    6233                       NaN   
    
                                                       cast  \
    0     Alan Marriott, Andrew Toth, Brian Dobson, Cole...   
    1                                      Jandino Asporaat   
    2     Peter Cullen, Sumalee Montano, Frank Welker, J...   
    3     Will Friedle, Darren Criss, Constance Zimmer, ...   
    4     Nesta Cooper, Kate Walsh, John Michael Higgins...   
    ...                                                 ...   
    6229  Burnie Burns, Jason Saldaña, Gustavo Sorola, G...   
    6230  Marc Maron, Judd Hirsch, Josh Brener, Nora Zeh...   
    6231                                                NaN   
    6232  Daniel Radcliffe, Jon Hamm, Adam Godley, Chris...   
    6233  Jennifer Aniston, Courteney Cox, Lisa Kudrow, ...   
    
                                           country         date_added  \
    0     United States, India, South Korea, China  September 9, 2019   
    1                               United Kingdom  September 9, 2016   
    2                                United States  September 8, 2018   
    3                                United States  September 8, 2018   
    4                                United States  September 8, 2017   
    ...                                        ...                ...   
    6229                             United States                NaN   
    6230                             United States                NaN   
    6231                                       NaN                NaN   
    6232                            United Kingdom                NaN   
    6233                             United States                NaN   
    
          release_year    rating    duration  \
    0             2019     TV-PG      90 min   
    1             2016     TV-MA      94 min   
    2             2013  TV-Y7-FV    1 Season   
    3             2016     TV-Y7    1 Season   
    4             2017     TV-14      99 min   
    ...            ...       ...         ...   
    6229          2015        NR  13 Seasons   
    6230          2016     TV-MA   4 Seasons   
    6231          2016       NaN      60 min   
    6232          2013     TV-MA   2 Seasons   
    6233          2003     TV-14  10 Seasons   
    
                                                  listed_in  \
    0                    Children & Family Movies, Comedies   
    1                                       Stand-Up Comedy   
    2                                              Kids' TV   
    3                                              Kids' TV   
    4                                              Comedies   
    ...                                                 ...   
    6229  TV Action & Adventure, TV Comedies, TV Sci-Fi ...   
    6230                                        TV Comedies   
    6231                                             Movies   
    6232           British TV Shows, TV Comedies, TV Dramas   
    6233                     Classic & Cult TV, TV Comedies   
    
                                                description  
    0     Before planning an awesome wedding for his gra...  
    1     Jandino Asporaat riffs on the challenges of ra...  
    2     With the help of three human allies, the Autob...  
    3     When a prison ship crash unleashes hundreds of...  
    4     When nerdy high schooler Dani finally attracts...  
    ...                                                 ...  
    6229  This parody of first-person shooter games, mil...  
    6230  Marc Maron stars as Marc Maron, who interviews...  
    6231  Nursery rhymes and original music for children...  
    6232  Set during the Russian Revolution, this comic ...  
    6233  This hit sitcom follows the merry misadventure...  
    
    [6234 rows x 12 columns]>




```python
data3.index

```




    RangeIndex(start=0, stop=6234, step=1)




```python
data3.columns

```




    Index(['show_id', 'type', 'title', 'director', 'cast', 'country', 'date_added',
           'release_year', 'rating', 'duration', 'listed_in', 'description'],
          dtype='object')




```python

```
