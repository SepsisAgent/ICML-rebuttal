# ICML-rebuttal

|Test|Method|WIS|WPDIS|DR|
|---|---|---|---|---|
|IV-4k|Clinician|5.25[4.8,5.7]|10.62[8.6,12.5]|5.44[3.9,7.1]|
||AI Clinician|9.99[2.6,13.6]|10.01[3.7,15.0]|**9.90[4.4,14.6]\#1**|
||DDQN|6.19[-4.8,5.7]|15.14[2.0,32.5]|8.41[-5.0,22.4]|
||WD3QNE|11.11[5.2,14.7]\#2|**24.00[19.4,29.6]\#1**|7.86[3.4,12.5]|
||SepsisAgent(ours)|**13.05[12.0,13.6]\#1**|23.53[12.1,32.9]\#2|9.50[7.6,11.2]\#2|
|III-2862(OOD)|Clinician|5.77[5.2,6.3]|14.92[13.3,16.7]|5.90[4.3,7.6]|
||AI Clinician|6.39[-9.5,12.8]|14.25[-2.9,29.4]|9.91[7.3,13.0]\#2|
||DDQN|6.03[1.0,10.3]|14.56[9.9,20.1]|7.03[-11.6,19.5]|
||WD3QNE|9.16[-1.4,12.8]\#2|**18.67[8.4,27.9]\#1**|6.40[-1.5,13.3]|
||SepsisAgent(ours)|**11.50[2.6,14.0]\#1**|16.22[6.2,26.7]\#2|**10.08[3.1,17.5]\#1**|


|WorldModel|Method|Survival(%)|Avg Reward|
|---|---|---:|---:|
|GRU|SepsisAgent(StageI:Alignment)|54.07|1.73|
||SepsisAgent(StageII:BehaviorCloning)|55.72|2.38|
||SepsisAgent(StageIII:RL)|60.41|3.73|
|LSTM|SepsisAgent(StageI:Alignment)|60.28|3.37|
||SepsisAgent(StageII:BehaviorCloning)|65.06|5.14|
||SepsisAgent(StageIII:RL)|65.66|5.15|
|Transformer|SepsisAgent(StageI:Alignment)|67.45|5.93|
||SepsisAgent(StageII:BehaviorCloning)|68.14|6.33|
||SepsisAgent(StageIII:RL)|70.44|7.01|
