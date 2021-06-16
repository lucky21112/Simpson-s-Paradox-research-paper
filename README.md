# Simpson's Paradox-research-paper
In this research paper i have  explained what is Simpson's Paradox is abnd how it can be detected and i have used Covid-19 Dataset of USA and try to find why Black Non-Hispanic race is having higher case fatility in subgrouped data as compared to aggregated data.


I have used 3 different Statistical methods for handling these problems:-

1 ##Randomization Block Design: - It is a method in which experimental subjects are divided into blocks and then treatment are assigned to these random blocks. But in the blocks, it is necessary to put subjects which are similar. By using this method we can reduce the variability of confounding variables For example in the UC Berkeley example suppose we have 1200 applicants we are going to divide gender variable which contains males and females into two different blocks each having 600 applicants as we can see from Fig. 4 and then put males into 6 groups randomly with each group having 100 applicants as there are 6 departments one group for each department and similarly for female and the group count should be equal for all men and for all women. Now our problem of men applying in departments that has high acceptance rate and female applying into departments that has low acceptance rate will be solved as there are equal number of subjects for all departments. Hence the variation in the confounding variable department would be solved. 
   
   
2 ##Restriction:-Restriction is another method that can be used during the design phase. One of the main reasons of occurring Simpson’s paradox is an unequal distribution of confounding variables and that’s what the restriction method will try to eliminate and hence reduce Simpson’s paradox. Restriction method will restrict the sample by only including those subjects who have the same value of confounding variables. For example in our UC Berkeley example, we have already identified that department was confounding variable as it was unequally distributed as for some departments like A, B men were more applying as their acceptance rate was high while for department E and F women were applying though their acceptance rate is less. By using restriction we can eliminate this problem by restricting confounding variable department. If we restrict department and consider only department A and B in our dataset and then calculate aggregated data then in both aggregated an subgroup it will show women were getting discriminated then our problem will be solved while if we consider department E and F then we would be clear that men were getting discriminated hence our confusion would be solved by choosing one of the two. As we can also see from Fig. 5 that that men were getting discriminated in total and also in subgrouped data if we choose departments A and B only.
 

3 ##Stratification is very similar to random sampling except that in stratification the data is divided into subgroups called strata instead of blocks in randomization block design and then we have to decide and choose sample size and calculate stratified sample calculation which is done by this formula:- Sample Size of strata=(size of sample/population size) *layer size. In this formula, layer size represent count in strata and then random sampling is done based on the ratio of a group to the total population. Hence it will produce groups in which confounding variables do not vary. This method is used in the analysis phase and is specially used when we have less number of confounding variables. For example, let us suppose we have 1000 population of males and female and we divide the population into two strata of 700 male and 300 female applicants and there are 6 departments they can apply and then we choose sample size let us assume we choose sample size 100 and now we are going to calculate the sample size of strata.

For males we will have (100/1000)*700 = 70 sample size of strata while for females we will have (100/1000)*300=30. After that we just need to use random sampling and produce groups for each department in that way variation of confounding variable is reduced. The whole process has been shown in Fig.  6 along with the group samples for each department.



After that we have implement all these 3 methods and found out that Black Non-Hispanic race was the race with higher case fatility rate as compared to White.
