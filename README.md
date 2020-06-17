# Graphics Lies, Misleading Visuals

This study is part of an assignment of "Applied Data Science with Python" by the University of Michigan which references heavily on Alberto Cairo’s book, ***The Truthful Art.***

The instructions for this assignment were to:
1) Locate and identify a visual that displays misleading information.
2) Interpret the features of the visual in order to identify the mechanism(s) that is/are used by the "encoder" to mislead the "decoder."
    - Hiding relevant data.
    - Displaying too much data and obscuring reality.
    - Distorting data through graphic forms.
3) For each mechanism identified, an explanation of how it was used to mislead.

The following visual Figure 1, that I have for analysis was obtained from [businessinsider.com](https://www.businessinsider.com/the-27-worst-charts-of-all-time-2013-6#welcome-to-fox-where-the-line-graphs-are-made-up-and-the-points-dont-matter-12) depicting an issue regarding job loss presented from Fox News.

![Figure 1](https://github.com/kaichua/Graphics-Lies-Misleading-Visuals/blob/master/Figure_1.PNG)

<ins>**Figure 1: Job Loss By Quarter Line Graph**</ins>

The intended audience of Figure 1 should be the general public of the United States. This is because Fox News is an exclusive American cable television news channel based in the United States, hence it would only make sense that it is only made accessible to those living in the United States.

At first glance, the encoder can be seen to have adopted several mechanisms.

Firstly, there might be relevant data hidden to highlight what benefits us. The title clearly states "Job Loss By Quarter" but the x-axis says otherwise. One can find gaps of 6 months between September 2008 to March 2009 and gaps of 9 months between December 2007 and September 2008 in the data. 

Next, the encoder also might have used graphic forms in inappropriate ways. The truncated y-axis with missing labels might give decoders a false sense of the linear growth in the number of job losses. Additionally, the inconsistency of the data's month range mentioned previously might fall into this category as one might assume the data was plotted quarterly correctly.

To understand the news correctly, I visited the Bureau of Labor Statistics to look for the data presented. I started by searching the archive by year backward from 2010 to 2007, and to my surprise, I could not find the statistics that were stated in the line graph. 

The closest I could find was Figure 2, which fits the description. The visual shown below was obtained from [Bureau of Labor Statistics](https://www.bls.gov/opub/ted/images/2011/ted_20110505.png), depicting the gross quarterly job losses and gains from the years 2000 to 2010. 

![Figure 2](https://github.com/kaichua/Graphics-Lies-Misleading-Visuals/blob/master/Figure_2.PNG)

<ins>**Figure 2: Gross Job Gains & Losses From March 2000 to September 2010**</ins>

At a glance, the highest possible y-axis was only at 9 million with the gross job losses peaking only at around 8.8 million in the second quarter of 2001. The figures indicated in Figure 1 was nowhere to be found.

Therefore, I proceeded to perform a reverse image search on Figure 1, and I discovered that the title was misrepresented and instead refer to the "Total Unemployed" shown in Figure 3.

![Figure 3](https://github.com/kaichua/Graphics-Lies-Misleading-Visuals/blob/master/Figure_3.PNG)

<ins>**Figure 3: Corrected Title Showing "Total Unemployed"**</ins>

This invalids the initial analysis of the encoder purposefully skipping ranges between the data to hide relevant data to highlight what benefits us and changes my analysis from "Job Losses" to "Unemployment".

To err is human, hence using the corrected title, I continued with my analysis by visiting the Bureau of Labor Statistics once again but instead focusing on the topic of unemployment. I compiled the figures for unemployment from June 2010 to December 2007 to see if I could recreate the graph shown in Figure 3. 

Figure 4 shows the entire timeline of unemployment from June 2010 to December 2007. In Figure 4, one can infer an increase in unemployment rates from December 2007 up till June 2009, after which the rate of unemployment starts to stabilize between July 2009 to June 2010. 

![Figure 4](https://github.com/kaichua/Graphics-Lies-Misleading-Visuals/blob/master/Figure_4.png)

<ins>**Figure 4: Number Of Unemployment From December 2007 To June 2010**</ins>
 
The encoder chose to omit the fact that there was a decrease in unemployment from September 2009 to June 2010 but rather showcase an increase in unemployment from March 2009 to June 2010. 

This clearly shows that the encoder was trying to hide relevant data to highlight an issue of worrying increase of unemployment since December 2007 instead of an improvement shown from September 2009 onward which might be due to certain policies being enforced by the government.

Figure 5 shows the timeline of unemployment matching Figure 3. 

![Figure 5](https://github.com/kaichua/Graphics-Lies-Misleading-Visuals/blob/master/Figure_5.png)

<ins>**Figure 5: Replicated Graph Displaying Selected Months For The Number Of Unemployed**</ins>

Figure 5 does not show a linear growth unlike the one shown in Figure 3. The graph shown in Figure 5 indicates that the rate of unemployment was growing at differing rates and not increasing at a constant pace shown in Figure 3. This supports my analysis that the encoder had used graphic forms in inappropriate ways to misinform the decoders. 

It is also to note that Figure 3 rounds figure inconsistently with figures in December 2007 and September 2008  rounded down to the nearest million whereas figures in March 2009 and June 2010 rounded up to the nearest 500 thousand.
