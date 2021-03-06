# INFO6205_527
## Genetic algorithms for the TSP problem  
#### Name:	Weiyi Lan 001822514  
#### Wen Zhong 001495774  
#### Advisor: Dr. Robin Hillyard  
### Problem description:  
The travelling salesman problem (TSP ) asks the following question: "Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city and returns to the origin city?" It is an NP-hard problem in combinatorial optimization, important in operations research and theoretical computer science.
The travelling purchaser problem and the vehicle routing problem are both generalizations of TSP.

### Program structure:
![image](https://github.com/zhongwenn1/INFO6205_527/blob/master/image/Project_Overview.png)  
#### 4 java file and one test case:  
![image](https://github.com/zhongwenn1/INFO6205_527/blob/master/image/GA.PNG)  
![image](https://github.com/zhongwenn1/INFO6205_527/blob/master/image/GAData.PNG)  
![image](https://github.com/zhongwenn1/INFO6205_527/blob/master/image/GA.PNG)  
![image](https://github.com/zhongwenn1/INFO6205_527/blob/master/image/Population.PNG)

#### Structure in each java file  
### Code Analysis:
#### GAData.java:
Set the parameters and the cityPosition map.
#### Individual.java:
Set the gene, distance and the fitness.
Use the greedy algorithm
 
#### Population.java:
Set the head point and the species number.  
#### GA algorithm java:
1.run:run the algorithm  
2.createBeginningSpecies:create the species  
3.calRate:calculate the rate of each species to be chosen  
4.select:roulette strategy for choosing the species with high fitting.  
5.crossover:chromosome crossover  
6.mutate:chromosome mutation  
7.getBest:get the most suitable species  

#### User Guide:
	static int CITY_NUM; // number of citys  
	static final int SPECIES_NUM = 200; // number of species  
	static final int GENERATE_NUM = 10000; // number of generation  
	static final float pcl=0.6f, pch = 0.95f; // number of crossover  
	static final float pm=0.4f; // number of mutation  
	static final float[][] disMap; // data of map  

We can set the parameters to get the different results.  
 
Then set the city position, just like the coordinate, take 10 cities as an example, we set the 10 different positions into an array and get to result.  We can also write these data into a file and use the data with IO inputStream.  

We can also get random map
![image](https://github.com/zhongwenn1/INFO6205_527/blob/master/image/RndomMap.PNG)

#### Test Result:  
 
Find the shorest path.
