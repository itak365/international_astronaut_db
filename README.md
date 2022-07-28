# Python Data Analysis of Major Spaceflight Milestones
## A Python Project by Ian Takaoka

## Introduction
This project seeks to demonstrate Python on publicly available data on human spaceflight from 1961 to early 2020, as a final project for Code Kentucky's Data Analysis Course 1. For the interests of simulating a "real-world" research project that I would do in academia, the Jupyter Notebook and the project at large are formatted around the data itself, rather than a laundry list of the below features.  It seeks to use Python's data science capabilities to derive meaning from quantitative data regarding human spaceflight, allowing me to highlight and research particular milestones more interesting than "firsts." 

## Technical Notes and Requirements to Run:
This Jupyter Notebook was created with VSCode in an Anaconda environment. Those users with Anaconda should already have the relevant packages installed- to download and run this locally, you will need to ensure that your Python environment has access to Pandas, Numpy, and Matplotlib. I have also used local Jupyter Notebook/IPython settings to disable soft warnings regarding chained assignment. 

The Wikipedia module should be installed prior to use, as I make extensive use of it throughout the project. In your local Python terminal, you simply need to input:  

``` pip install wikipedia ```

or 

```conda install wikipedia ```

And the module will be downloaded. 
## Features:
1) The pandas module was used to read in a publicly-available .csv file. 
2) Pandas was also used to run arithmetic on several variations of this .csv in several transformed dataframes. I used these functions to calculate spaceflight milestones: specifically, the ages of the oldest and youngest astronauts and astronaut candidates, the highest number of spaceflight hours, and the total time engaged in extravehicular activity (EVA). I also derived demographic information on the nationalities of astronauts, and the duration of spaceflight for non-International Space Station astronauts.
4) The above values are all visualized using matplotlib (or Pandas' built-in functionality for data visualization). 
5) This project also features full integration of the Wikipedia module, allowing me to return the summary paragraphs (with a specified number of sentences) from the Wikipedia pages of specific astronauts and cosmonauts when I want the user to read about the person in question. 

## Limitations
This dataset only has years and not calendar dates, leaving me with limited capability to show change over time (This can be seen in the scatterplots which are very vertical). The dataset also does not include spaceflight statistics after January 2020. As the Soviet Union did not distinguish between nationalities within its borders, the USSR/Russia field may include cosmonauts from other Soviet Republics and not specifically from the Russian SFSR. Additionally, no commercial astronauts are listed except for space tourists Dennis Tito and Richard Garriott, as SpaceX's Crew Dragon Demo-2, the first manned commercial spaceflight, did not launch until May 2020. 

## Wishlist for Code KY Phase 2 and Beyond: 
In future versions, I hope to incorporate the CyrTranslit module to make use of local Python transliteration functionality. I also would like to make use of the actual Wikipedia API with the requests module, in order to import Wikipedia main page images for returned results. This was actually attempted several times, but I wasn't able to find a smooth way to include it, so I instead made use of the wikipedia module. I also would like to find more accurate temporal data and merge it into this dataset for more exact arithmetic. 
