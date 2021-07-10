# TIME SERIES ANALYSIS

Effective Method for analyzing Time Series Data


## 1. Bursty Process vs. Random Process

There is a generalized queuing process, using a parameter ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn.gif) in Barabasi's Burst paper.
</br> ("The origin of bursts and heavy tails in human dynamics, 2005" : https://www.nature.com/articles/nature03459).

 * ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn.gif) : Control Parameter of Priority array's components' exponent. (like as fitness of node or task.)

 * ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(1).gif) : Random Process.
 * ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(2).gif) : Bursty Process. (Or Deterministic Process)


### Event & Inter Event Time (IET) & Inter Event Time Distribution (IETD)

1. Event : Clear definition of event is needed. (eg. In restaurant, food coming out can be defined as an event.)
2. Inter Event Time (IET) : The time interval between events defined above.
3. Inter Event Time Distribution (IETD) : The time interval between events defined above.

</br>For more details, please refer to the following paper : ("The origin of bursts and heavy tails in human dynamics, 2005" : https://www.nature.com/articles/nature03459)


### How to analyze time series data from this theory.

1. Prepare time-series data with clear definition of events.
2. Calculate IET & IETD from prepared data.
3. If IETD follows power-law distribution, measure exponent of IETD. If it follows exponential distribution, this time-seris data might be a randomly generated data from iid.
4. If you want to classify time-series data by generating method of data, it might be okay to compare exponents.


## 2. Record Statistics

There is a Good statistics for analyzing time series data. (If time series data is generated by probability density function) : Record Statistics
</br> If you want to see universal result of record statistics for random walk time series, see</br> : "_Universal record statistics for random walks and Lévy flights with a nonzero staying probability_, Satya N Majumdar, Philippe Mounaix and Grégory Schehr, 2021"
</br>(https://iopscience.iop.org/article/10.1088/1751-8121/ac0a2f/meta?casa_token=A6gUJFqk4dcAAAAA:l7Ou2iTFRK2j7ADeCi9SXsRETYH41F9bomll9YAkt3x7Dlt-hY1Pvm56UjCWRf0suhsEOM1imMU)


### Definition of Record Event

Time Series Data Set : ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(6).gif)
</br> For each ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(5).gif), when ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(8).gif) at timing ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(9).gif), a Record Event occurs.


### Some Important Variables for Record Statistics

* ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(12).gif) : Binary Indicator for Record Event Occurs.</br></br>
* ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(11).gif) : Record Number (The number of Record Events occurred)</br></br>
* ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(10).gif) : Average Record Number (The mean value of Record Number for many time series samples)</br></br>
* ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(13).gif) : Record Rate (Average Binary Indicator for Record Event Occurs).</br></br>

* ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(16).gif) : Variance of Record Number
* ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(17).gif) : Fano Factor
* ![math](https://github.com/IDAH-BITBOX/TIME_SERIES_ANALYSIS/blob/main/math_img/CodeCogsEqn%20(18).gif) : Connected Two-time Correlation Function
