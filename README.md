# Spatial Modeling of COVID-19 Lockdown Strategies - UConn

## Abstract
In the United States, the number of cases of the COVID-19 is increasing constantly. After a few months of the lockdown in March, most of the states are reopening, including retail stores, restaurants, and recreation. As a college student, COVID-19 is affecting normal student life, residence life, and so on. 

UConn is located in the northeast of the United States, the temperature is low during the fall and winter. Students and the university need to be prepared and prevent the new wave from spreading. Typically, international students and out-of-state students are more vulnerable to get infected due to limited access to testing.

In this study, we are focusing on building a mathematical model, Susceptible-Infected-Recovered (SIR) model, and estimate the infectious rate and recovery rate at the University of Connecticut (UConn), Storrs. After finding out the parameters using SIR, we are using Agent-Based Modeling (ABM) to simulate different cases to predict and evaluate the risks of different places on campus. 

UConn, located in Storrs, has approximately 5,000 students living on campus. This would increase the chances of interaction between students in public places such as academic buildings, dining halls, grocery stores, residential halls, and apartments. Before the semester began, UConn had already announced reopening policies. Most of the classes are moving online or distance learning to prevent spreading of disease. In-person classes require students wearing a mask and maintaining at least six feet of physical distancing from others. Dining halls are switching to take-out and limited dining models. However, for those students who live in residential halls, even though UConn policy requires one person per dorm room, they are still sharing bathrooms. For those who live in apartments or off-campus, students have approximately one to four roommates which increase the chance of infection. 

Our primary goal is to extend the SIR model into the spatial form and using QGIS and NetLogo to visualize the spreading. This paper is focusing on a specific area with a smaller population size, rather than a state or a country. We are using the data to predict the cases and infection rate in the next few months, evaluating each building’s risk and ranking the risk that has a higher chance to get infected. In the Netlogo program, the number of susceptible individuals in the initial population is 1,000 people compared to the approximately 5,000 who are living on campus. The ratio of parameters and the real population is 1:5. We set the two parameters, β and γ, constant which β equals to 0.602 and γ equals to 0.527. Three scenarios are created based on varying restrictions. The baseline scheme means that all restrictions will be enforced (link of the baseline scenario: https://github.com/Weijia-Wang341/COVID-19-UConn/issues/1#issue-732845238). The second scenario is obtained by implementing 50% of its regular indoor capacity (link: https://github.com/Weijia-Wang341/COVID-19-UConn/issues/2#issue-732854930). The third scenario follows the Phase 3 Reopen Rules by Sector in Connecticut, which is 50% capacity of religious gatherings, and 75% indoor capacity of restaurants (link: https://github.com/Weijia-Wang341/COVID-19-UConn/issues/3#issue-732855606).
