# Quantitative Research Project: Verify Third-Order Markov Property

Let <img src="http://www.sciweavers.org/tex2img.php?eq=p_x%28t%29&bc=White&fc=Black&im=jpg&fs=12&ff=modern&edit=0" align="center" border="0" alt="p_x(t)" width="37" height="19" /> be the price of a cryptocurrency x at time t (where t has been converted into an integer index). There are 5 cryptocurrencies: AAA, BBB, CCC, DDD, and EEE.

Let the first-order price differential <br /> <img src="http://bit.ly/2WvYrMl" align="center" border="0" alt="\Delta p_x(t) = \left\{\begin{matrix} 1\textup{ if }p_x(t+1)-p_x(t) > 0\\ 0\textup{ if }p_x(t+1)-p_x(t) = 0\\ -1\textup{ if }p_x(t+1)-p_x(t) < 0 \end{matrix}\right." width="274" height="62" />

Let the second-order price differential <br /> <img src="http://www.sciweavers.org/tex2img.php?eq=%5CDelta%5E2%20p_x%28t%29%20%3D%20%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20%281%2C1%29%5Ctextup%7B%20if%20%7Dp_x%28t%2B2%29-p_x%28t-1%29%20%3E%200%5Ctextup%7B%20and%20%7Dp_x%28t%2B1%29-p_x%28t%29%20%3E%200%5C%5C%20%281%2C0%29%5Ctextup%7B%20if%20%7Dp_x%28t%2B2%29-p_x%28t-1%29%20%3D%200%5Ctextup%7B%20and%20%7Dp_x%28t%2B1%29-p_x%28t%29%20%3E%200%5C%5C%20%281%2C-1%29%5Ctextup%7B%20if%20%7Dp_x%28t%2B2%29-p_x%28t-1%29%20%3C%200%5Ctextup%7B%20and%20%7Dp_x%28t%2B1%29-p_x%28t%29%20%3E%200%5C%5C%20%5Ctextup%7Betc.%7D%20%5Cend%7Bmatrix%7D%5Cright.&bc=White&fc=Black&im=jpg&fs=12&ff=modern&edit=0" align="center" border="0" alt="\Delta^2 p_x(t) = \left\{\begin{matrix} (1,1)\textup{ if }p_x(t+2)-p_x(t-1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,0)\textup{ if }p_x(t+2)-p_x(t-1) = 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,-1)\textup{ if }p_x(t+2)-p_x(t-1) < 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ \textup{etc.} \end{matrix}\right." width="521" height="82" />

Let the third-order price differential <br /><a href="https://www.codecogs.com/eqnedit.php?latex=\Delta^3&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;(1,1,1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,0)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;=&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,-1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;<&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;etc.&space;\end{matrix}\right." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta^3&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;(1,1,1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,0)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;=&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,-1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;<&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;etc.&space;\end{matrix}\right." title="\Delta^3 p_x(t) = \left\{\begin{matrix} (1,1,1)\textup{ if }p_x(t+3)-p_x(t-2) > 0\textup{ and }p_x(t+2)-p_x(t+1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,1,0)\textup{ if }p_x(t+3)-p_x(t-2) = 0\textup{ and }p_x(t+2)-p_x(t+1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,1,-1)\textup{ if }p_x(t+3)-p_x(t-2) < 0\textup{ and }p_x(t+2)-p_x(t+1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ etc. \end{matrix}\right." /></a>

My hypothesis was that <a href="https://www.codecogs.com/eqnedit.php?latex=\Delta^3&space;p_x(t)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta^3&space;p_x(t)" title="\Delta^3 p_x(t)" /></a> is a Markov chain, i.e.,
<a href="https://www.codecogs.com/eqnedit.php?latex=\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1},\Delta^3&space;p_x(t-2)&space;=&space;k_{t-2},...,&space;\Delta^3&space;p_x(0)&space;=&space;k_{0}&space;\right&space;)&space;\\\indent&space;=&space;\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1}\right&space;)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1},\Delta^3&space;p_x(t-2)&space;=&space;k_{t-2},...,&space;\Delta^3&space;p_x(0)&space;=&space;k_{0}&space;\right&space;)&space;\\\indent&space;=&space;\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1}\right&space;)" title="\mathbb{P} \left (\Delta^3 p_x(t) = k_t | \Delta^3 p_x(t-1) = k_{t-1},\Delta^3 p_x(t-2) = k_{t-2},..., \Delta^3 p_x(0) = k_{0} \right ) \\\indent = \mathbb{P} \left (\Delta^3 p_x(t) = k_t | \Delta^3 p_x(t-1) = k_{t-1}\right )" /></a><br /> More specifically, that 3 is the smallest n for which <a href="https://www.codecogs.com/eqnedit.php?latex=\Delta^n&space;p_x(t)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta^n&space;p_x(t)" title="\Delta^n p_x(t)" /></a> is a Markov chain.

A short Python script, `get_diff_time_series.ipynb` was written to generate these a time series of these price change directions, in the first, second, third, and fourth order. Then, a short R script, `verify_markov_property.R`  was used to verify the Markov property in these time series using the markovchain package, which did not have an equivalent in Python. My hypothesis will indeed be true if the test for first order and second order fails, but the test for the third order passes and continues to pass for higher orders.

The null hypothesis is that the diff time series is not a Markov chain, and this null hypothesis is rejected with a p-value greater than 0.05. As we will see, the test produces a p-value of 0 for first and second order, and a p-value of 1 for third order. We verify the fourth-order diff time series as well, just to empirically verify that the results are consistent with what they should theoretically be (which is that if third order is Markov, all higher orders should be as well, by property of Markov chains). These results hold for all 5 coins.
