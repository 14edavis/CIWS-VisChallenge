# CIWS-VisChallenge (Household Residential Data)

Basilisk reads a csv file of household residential Intelligent Water Supply Data
and creates two lists: timestamps and water pulses.
On these lists, the item at index *n* of the timestamps list corresponds with index *n* of the water pulse list.
The timestamp list utilize a datetime object, allowing for various time-related manipulations.
    
Basilisk has 3 types of functions--*filtering*, *totaling*, and *averaging* functions--exemplified by the sample graphs. 
It aids both water consumers and providers, who would want graphs showing patterns and trends, 
as well as water researchers that might want to analyze and manipulate data on a more detailed level. 
Along with creating graphs, passing data through the functions creates data sets that researchers can use for further analysis.

## Sample Graphs

Basilisk makes use of datetime timestamps to visualize residential water usage through various averaging and filtering functions. 
For example, it can graph average water usage throughout the day.

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_AverageHour1.png)

Using the same method, it can also compare water usage on the weekend to weekdays.

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_AverageHour2.png) 

Want more detail? Graph average water usage for each individual day of the week. Water consumers can use a similar graph to identify what times of the week they use the most water and then used this tailored information to reduce their own water usage. 

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_AverageHour3.png)

 
You can also view the typical week as a whole by averaging the water usage by weekday.

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_Week1.png) 


Or get creative, and tack together your hourly-average data into a more detailed graph.

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_Week2.png) 
 
Speaking of creative, what happens if you average water usage by the minute-stamp? 
(i.e. all the water pulses at 1:43, 2:43, 3:43, 4:43, etc. belong to the same group) 
Turns out that this unusual analysis shows a pattern. Now we can see that Monday/Wednesday/Friday all have a similar schedule. 
So do Tuesday/Thursday. The averaging by minute-stamp gives an interesting facet (*faucet?*) for water researchers to explore. 

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_Minute.png)  

What if you don't want averages, but a simple timeline instead? Just pick a timeframe and the appropriate filter and resolution.

Watch daily water usage over a month.

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_Total1.png) 

Compare the hourly use to the minute-by-minute use for a particular day.
 
![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_Total2.png)  
 
Or show the maximum resolution, water pulse counts every 4 seconds, for a given morning.

![alt text](https://raw.githubusercontent.com/14edavis/CIWS-VisChallenge/master/doc/images/graph_Total3.png)  

These examples just scratch the surface.
Whether you use Basilisk "as is" or as a template for more complicated projects, 
Basilisk provides the scaffolding you need to visualize household residential water usage.

**_Graphs generated by the_ sample\_analysis() _function in Basilisk.py_**

# Troubleshooting

If Basilisk won't load a _.csv_ file, try saving the data as a _.txt_ file instead.

