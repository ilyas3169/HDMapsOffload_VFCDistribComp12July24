# matlabVehicularComputingoffloading
## Augmenting Vehicular Edge and Fog enabled Computation offloading framework using temporal segmentation and heuritic method
## DESCRIPTION AND CONTENTS OF THE MATLAB CODE
### Purpose of MATLAB Code:
This MATLAB code quantitively analyses our proposed computation offloading framework. We used Key Performance Indicator (KPIs) and reference methods to evaluate our approach.
### Used Key Performance Indicators (KPIs):
The KPIs that we used for analysis are:
	Time response (in milliseconds) during computation-tasks’ offloading process using respective offloading and scheduling frameworks.
	Number of different configurations. Each configuration is a set of unique parameters that specify the orientation of the under-observation computation offloading framework using the Intelligent Transportation System (ITS) as its test-bed. The total number of different configurations used are twelve (12) for each type of scheduling method. As we fixed the scheduling method as one of the basic factors that is unique to each baseline approach that we used to analyze our approach. 
### Used Baseline Methods:
These baseline approaches are:
	First Come First Serve (FCFS)
	Search based approach
	Time response-based approach
	Minimum time response approach
	Maximum time response approach
### First Come First Serve (FCFS):
The "FCFS", or First in, First Out (FIFO), is a canonical scheduling method and its working criteria is evident from its name [54].  Several recently published computations offloading proposals, as in articles referenced [55] and [33], have FCFS as one of their baseline precedents. We are using it for its simplicity. We employed FCFS by allocating the requested computation tasks at RSU to the first available member fog-vehicle (SV). However, unlike several other scheduling method as in table III, FCFS do not rely on estimating transmission time, queueing delay, and task execution latency of computation.
Apart from simple technique like FCFS, this baseline method depends on proactive measurement of total-response time. It has further two (02) types.
##Maximum Completion Time based
This method first identifies and isolates the tasks with the maximum expected completion time among a set of tasks during a time-period, symbolized in our model as "T". This is the type of scheduling used as the baseline in the computation offloading method in the article referenced as [33]. 
### Minimum Completion-Time based
This approach is the evil-twin of the above "Maximum" completion time-based scheduling method. It identifies the tasks with expected minimum completion time among a set of tasks within time-period ’T’. And like its other counterpart “Maximum” completion-time based scheduling, it also does not depend on constraints as mentioned in (11) but requires substantial amount of control information dissemination during operation. However its estimator depends on the transmission time from TV/CU to RSU, symbolized in our model as “ t_(TV|CU⇔RSU)  ” as in (5) and, transmission time from RSU to SV, “ t_(RSU⇔SV)” as in (6), execution time by SV or RSU, ’ t_ⅇx^(SV|RSU)’ as in (7), and waiting time, symbolized as "〖wait〗_(sν|RSU)^time ". In our simulations’ runs, with “minimum completion time-based scheduling” method, we accumulated the results in form of pareto chart as shown in Fig. 7. This scheduling procedure too can hardly fulfill the computation-offloading requirement of sub-hundred milliseconds; a requirement of any highly latency-sensitive vehicular network application as can be seen in Fig. 7.  This can be confirmed by from Fig. 7 as it shows that overall, the scheduled tasks by this method experienced delay of at least 383.8409 milliseconds. And the prioritized maximum number of tasks have latency in the range of 753.840 milliseconds and 1123.8409 milliseconds. 
#### Note: 
Please find the associated mathematical model equations and mathematical formulations along with relevant descriptions, definitions using flowchart diagrams in our article titled “Fog computing augmentation for advanced ITS applications employing temporal segregation-based computation offloading framework”
