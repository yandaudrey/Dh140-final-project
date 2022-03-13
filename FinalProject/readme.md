# Network analysis of Tower Theatre and Los Angeles Theatre 

<em>Click [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/yandaudrey/Dh140-final-project.git/HEAD) to explore datasets and interactive Jyupter nootbook</em>


### Introduction
My project focuses on newspaper articles in <em>The Los Angeles News</em> published between 1927–1931 surrounding Tower Theatre and Los Angeles Theatre in downtown LA. Both theaters, located in Historic Core, were originally owned by entrepreneur H. L. Gumbiner (1879-1952) and designed by architect S. Charles Lee (1899-1990) in 1927 and 1931, respectively. These two theaters demonstrated a multiplicity of innovations and represented a peak of Los Angeles movie palaces in the 1920s and the beginning of the 1930s. 

With the decline of downtown LA and the increased competition of chain movie theaters, both Tower Theatre and Los Angeles Theatre were unable to survive through the end of the twentieth century. Tower Theatre changed its name to Newsreel Theatre and permanently closed in 1988. In 2021, Apple renovated the building and rebranded it as Apple Tower Theatre, reviving the landmark architecture and transforming the old movie palace into an Apple store. Los Angeles Theatre, once considered the best movie theatre in the world, stopped selling movie tickets in 1994. Currently, it serves as a film shoot location.

In this project, I would like to explore a network of the architect, theater owners, investors, and other technicians to understand network influences on the completion of these two buildings. 

- Tower Theatre: [802 S Broadway, Los Angeles, CA 90014](https://goo.gl/maps/bg9eiUr46CwzkTSp7)
- Los Angeles Theatre: [615 S Broadway, Los Angeles, CA 90014](https://goo.gl/maps/gqFpS5J8X6oTYthr8)

<figure>
    <img src="https://www.apple.com/newsroom/images/environments/stores/apple_nso-tower-theater-la_street-view_06222021_Full-Bleed-Image.jpg.large_2x.jpg"
         alt="Tower Theatre (2022)">
    <figcaption>Today's Tower Theatre</figcaption>
</figure>


<figure>
    <img src="https://losangelestheatre.com/img/homeimage_latheatre_lobby.jpg"
         alt="Los Angeles Theatre">
    <figcaption>The auditorium of Los Angeles Theatre</figcaption>
</figure>


My project is in progress. It already contains [blueprint annotations](https://bjkeith.humspace.ucla.edu/LAandTower/blueprints/) and a partial demonstration of [3D modeling](https://bjkeith.humspace.ucla.edu/LAandTower/vectorworks/). But there is a shortage of qualitative analyses, such as text analysis and network analysis to make this project more comprehensive. If I can integrate network analysis into this project, it will help readers understand how the completion of these two buildings associated the fields of cinema, business, architecture, and science. 

A challenge of this project is a limitation of archival research. Due to the limited  time, I can only collect data from <em>The Los Angeles News</em>. However, there are still a lot of newspaper articles surrounding these two buildings that I am not able to explore this quarter. 

### Methods
My data sources were newspaper articles published in <em>The Los Angeles News</em> between 1927 to 1931. I exported important articles that I collected from Zotero as CSV files. I also manually collected the names of figures appearing in the articles and created multiple datasets for Python to further clean my data, generating a list that exhibits all of the names relevant to these two buildings without repetition. Furthermore, based on these articles, I listed the source and the target as a dataset for Python to further calculate the composition of communities surrounding Tower and Los Angeles Theatres.  

### Results 
1. In total, there were 22 people highly relevant to the building process and the opening of Tower Theatre and Los Angeles Theatre. But most of the people were only involved in Los Angeles Theatre. Among them, H. L. Gumbiner and S. Charles Lee were only two figures playing significant roles in both Theatres. Gumbiner was the owner of two theaters; Lee was their architect.
2. The network of Tower Theatre and Los Angeles Theatre showed that there were four communities: 1) the actor community, leading with Charlie Chaplin, 2) the scientists community, such as Dr. Pease and Prof. Einestein, 3) the theater buildings' manager and architect, such as Gumbiner and Lee, and 4) other figures that were relatively marginal during this process. 

### Discussion
In this coding project, I first calculated how many people were involved in these two theatres in 1927 and 1931, respectively. I used for loop to iterate through names that I collected from archives, resulting in a list that consists of names without repetition. This list shows how many people were related to the establishment of these two theatres. However, not everyone played an equally significant role during this process. In order to better understand each person's individual significance within this network, I imported the python libraries NLTK, Pandas, and Numpy to calculate the frequency of these names and plot the frequeucy of them, showcasing who are more influential than others. 

Additionally, I created a list with people's names that exhibits the source and the target, and then I used the Python library, Bokeh, to plot two interactive images of the social network between people who were involved in these two buildings. The first image plainly shows the network among the source and the target. For the second image, with the color distinguishing different communities, the image ultimately shows that there were four communities surrounding the building process and the gala opening of Tower Theatre and Los Angeles Theatre. 



