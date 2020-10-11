# matplotlib-challenge
I was given a dataset of clinical trial data, where 9 treatment regimens were tested on mice to understand their effectiveness in treating squamous cell carcinoma (SCC). Using Pandas and Matplotlib I analyzed the data to find some trends and indications of which treatments are most effective. 

The data included basic information of the mice in the study such as sex, age, and weight. This was a well designed study with a large total number of subjects, N=249 mice.

The mice were split relatively evenly among the 9 treatment regimens and the placebo group, all of them had 25 mice at the start of the study (except for Stelasyn which had 24 mice).
The mice were also evely distriubted on sex, with 50.2% male and 49.8% female mice.
In general, if the tumor size was smaller, it can be an indication of an effective treatment. In addition, the longer the mice are able to survive on each treatment is another factor to consider when determining the effect of the treatment.

We were asked to consider the final tumor volume of mice on the following 4 treatment regimens - 'Capomulin','Ramicane','Infubinol','Ceftamin'.

Mice on Capomulin and Ramicane had smaller final tumor volumes than those on Infubinol and Ceftamin. The IQR was lowest for Capomulin and highest for Ceftamin, indicating that tumor volume was less variable among mice treated with Capomulin at their respective final timepoint. Infubinol had an outlier, and this needs to be taken into account if an significance testing will be done on that in the future.

Next I looked at a mouse on Capomulin, chosen at random, to see how tumor volume changed with timepoint. It showed a steady decrease which is a positive result.

Finally, concentrating just on Capomulin-treated mice, a plot of the average tumor volume versus average weight across for each mouse over the duration of the study revealed some interesting results.

Heavier mice generally had larger tumors, on average.
These factors have a strong postiive correlation of 0.84.
A linear regression line was appropriate for this data, and can be used to predict the average tumor volume of a mouse on Capomulin given it's weight.