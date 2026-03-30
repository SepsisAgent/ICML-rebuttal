# ICML-rebuttal

### Table 1

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Test</th>
      <th>Method</th>
      <th>WIS (95% IC)</th>
      <th>WPDIS (95% IC)</th>
      <th>DR (95% IC)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="5">IV-4k</td>
      <td>Clinician</td>
      <td>5.25 [4.8, 5.7]</td>
      <td>10.62 [8.6, 12.5]</td>
      <td>5.44 [3.9, 7.1]</td>
    </tr>
    <tr>
      <td>AI Clinician</td>
      <td>9.99 [2.6, 13.6]</td>
      <td>10.01 [3.7, 15.0]</td>
      <td><strong>9.90 [4.4, 14.6]</strong></td>
    </tr>
    <tr>
      <td>DDQN</td>
      <td>6.19 [-4.8, 5.7]</td>
      <td>15.14 [2.0, 32.5]</td>
      <td>8.41 [-5.0, 22.4]</td>
    </tr>
    <tr>
      <td>WD3QNE</td>
      <td><ins>11.11 [5.2, 14.7]</ins></td>
      <td><strong>24.00 [19.4, 29.6]</strong></td>
      <td>7.86 [3.4, 12.5]</td>
    </tr>
    <tr>
      <td><strong>SepsisAgent(ours)</strong></td>
      <td><strong>13.05 [12.0, 13.6]</strong></td>
      <td><ins>23.53 [12.1, 32.9]</ins></td>
      <td><ins>9.50 [7.6, 11.2]</ins></td>
    </tr>
    <tr>
      <td rowspan="5">III-2862 (OOD)</td>
      <td>Clinician</td>
      <td>5.77 [5.2, 6.3]</td>
      <td>14.92 [13.3, 16.7]</td>
      <td>5.90 [4.3, 7.6]</td>
    </tr>
    <tr>
      <td>AI Clinician</td>
      <td>6.39 [-9.5, 12.8]</td>
      <td>14.25 [-2.9, 29.4]</td>
      <td><ins>9.91 [7.3, 13.0]</ins></td>
    </tr>
    <tr>
      <td>DDQN</td>
      <td>6.03 [1.0, 10.3]</td>
      <td>14.56 [9.9, 20.1]</td>
      <td>7.03 [-11.6, 19.5]</td>
    </tr>
    <tr>
      <td>WD3QNE</td>
      <td><ins>9.16 [-1.4, 12.8]</ins></td>
      <td><strong>18.67 [8.4, 27.9]</strong></td>
      <td>6.40 [-1.5, 13.3]</td>
    </tr>
    <tr>
      <td><strong>SepsisAgent(ours)</strong></td>
      <td><strong>11.50 [2.6, 14.0]</strong></td>
      <td><ins>16.22 [6.2, 26.7]</ins></td>
      <td><strong>10.08 [3.1, 17.5]</strong></td>
    </tr>
  </tbody>
</table>

### Table 2

|WorldModel|Method|Sinsrvival(%)|Avg Reward|
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
