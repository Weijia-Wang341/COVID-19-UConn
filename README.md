# Spatial Modeling of COVID-19 Lockdown Strategies - UConn

## Introduction
In the United States, the number of cases of the COVID-19 is increasing constantly. Until Oct 28, 2020, according to John Hopkins Coronavirus Resource Center, there were 8,856,413 confirmed cases in the United States and 72,183 cases reported in one single day. After a few months of the lockdown in March, most of the states are reopening, including retail stores, restaurants, and recreation. As a college student, COVID-19 is affecting normal student life, residence life, and so on. 

According to the CDC, seasonal influenza viruses are common during the late fall, and peak between December to February [1]. There are some explanations about why flu season usually spreads in the winter. First, people spend more time indoors which increases the chance to have closer contact with others who might be carrying the virus. Students, for example, would prefer using public transportation, such as buses, instead of walking to class. Second, in the short days of the winter, people may run low on Vitamin D and weaken our immune system [2]. UConn is located in the northeast of the United States, the temperature is low during the fall and winter. Students and the university need to be prepared and prevent the new wave from spreading. Typically, international students and out-of-state students are more vulnerable to get infected due to limited access to testing [3].

In this studyarticle, we are focusing on building a mathematical model, Susceptible-Infected-Recovered (SIR) model, and estimate the infectious rate and recovery rate at the University of Connecticut (UConn), Storrs. The model generates the number of cases from August 16th, the date when students who live on campus check-in, to September 7th. After finding out the parameters using SIR, we are using Agent-Based Modeling (ABM) to simulate different cases to predict and evaluate the risks of different places on campus. 

UConn, located in Storrs, has approximately 5,000 students living on campus. This would increase the chances of interaction between students in public places such as academic buildings, dining halls, grocery stores, residential halls, and apartments. Before the semester began, UConn had already announced reopening policies. Most of the classes are moving online or distance learning to prevent spreading of disease. In-person classes require students wearing a mask and maintaining at least six feet of physical distancing from others. Dining halls are switching to take-out and limited dining models. However, for those students who live in residential halls, even though UConn policy requires one person per dorm room, they are still sharing bathrooms. For those who live in apartments or off-campus, students have approximately one to four roommates which increase the chance of infection. 

Our primary goal is to extend the SIR model into the spatial form and using QGIS and NetLogo to visualize the spreading. This paper is focusing on a specific area, rather than a state or a country, with a smaller population size. We are using the data to predict the cases and infection rate in the next few months, evaluating each building’s risk and ranking the risk that has a higher chance to get infected. Based on the policies that have been implemented at UConn, we are also making some suggestions to the University about forestalling the new wave coming in winter. 

## Methodology
To simulate the spreading of epidemics, we are building the SIR model. The SIR model was first introduced by Kermack and McKendrick by separating people into three different categories: susceptible (S), infected (I), and recovered (R) [4]. In this case, the population in Storrs is susceptible (S). Individuals who get infected move from susceptible stage to infected stage (I). Eventually, people who were removed from the infected stage recovered (R). The SIR model using the parameters β, the infection rate, and γ, the recovery rate, can be presented by the ordinary differential equation (ODE). 

The agent-based modeling (ABM) is modeled by a set of autonomous agents who make decisions based on a series of rules we set [5]. Each agent-based model can simulate a real-world situation, which provides important information. In this article, we are creating Ssix public places where that have higher risks of interactions between people were created, including school, church, office, bus, café, and sub.  In the program, the number of susceptible individuals in the initial population is 1,000 people compared to the approximately 5,000 who are living on campus. The ratio of parameters and the real population is 1:5. We set the two parameters, β and γ, constant which β equals to 0.602 and γ equals to 0.527. Three scenarios are created based on varying restrictions. The baseline scheme means that all restrictions will be enforced (This is the link of the interface of the baseline scenario). The second scenario is obtained by implementing 50% of its regular indoor capacity (link). The third scenario follows the Phase 3 Reopen Rules by Sector in Connecticut, which is 50% capacity of religious gatherings, and 75% indoor capacity of restaurants (link) [6]. 

