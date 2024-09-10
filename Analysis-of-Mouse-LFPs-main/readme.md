Neural Activity Analysis in Navigational Behavior

Overview
This project explores the neural dynamics of a rat navigating a three-arm maze, focusing on the hippocampus and medial prefrontal cortex's activity. Using a comprehensive dataset, we investigate how specific brain activities, particularly Sharp Wave Ripples (SWRs), correlate with the animal's navigational behavior and trial progression within the maze.

Dataset
The dataset comprises four sessions of a rat running through a three-arm maze, involving distinct behavioral conditions: running along the track, collecting water rewards while still, and running on a stationary wheel. Electrical signals were recorded in the hippocampus and medial prefrontal cortex using up to 6 arrays, capturing both LFPs and neuronal spikes at high resolution. This rich dataset allows for an in-depth analysis of place cells and interneurons' activity under different environmental conditions.

Methodology
Employed linear regression using Ordinary Least Squares (OLS) from the statsmodel library, with a data split of 80-20 for training and testing. The hypothesis was that as the trial number increases, both the number of SWRs per second and the average duration of SWR per trial would decrease.

Findings
R² Value: The OLS model resulted in an R² of 5.1%, indicating that about 5.1% of the variance in the trial number can be explained by our predictors (average ripples per second and average duration of ripples per trial).
Statistical Significance: The variables and the entire model were found to be statistically insignificant, suggesting that there is no strong relationship between the predictors (average ripple per second per trial, the average duration of a ripple per trial) and the trial number.
Data Processing: We employed a high sampling frequency rate of 625 Hz, necessary to capture the range of frequencies in which ripples occur (150-250 Hz).

Technologies Used
Python
Libraries: Pandas, NumPy, SciPy, Matplotlib, Seaborn, Scikit-learn

Results and Conclusion
Our findings indicate there is no significant relationship between the number of SWRs per second, the average duration of SWRs per trial, and the trial number. This result suggests that the frequency and duration of SWRs are not strong predictors of the trial number in this particular setting. \

Future Directions
Further research could explore other potential predictors (like the amplitude of the SWRs) or different aspects of neural activity that might correlate with behavioral states or trial progression. Additionally, increasing the computational capacity to include more channels or sessions might provide more insights, since the channel we used might not have been the optimal channel.

Acknowledgments
Special thanks to Tommy Lu, Morris Vasser, and Professor Gautum Agarwal.

Contact Information
For further inquiries or discussions, please contact Luke Feng at lukefengf2@gmail.com
