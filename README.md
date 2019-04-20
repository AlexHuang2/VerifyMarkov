# Quantitative Research Project: Verify Third-Order Markov Property

Let <a href="https://www.codecogs.com/eqnedit.php?latex=p_x(t)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?p_x(t)" title="p_x(t)" /></a> be the price of a cryptocurrency x at time t (where t has been converted into an integer index). There are 5 cryptocurrencies: AAA, BBB, CCC, DDD, and EEE.

Let the first-order price differential <br /> <a href="https://www.codecogs.com/eqnedit.php?latex=\Delta&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;1\textup{&space;if&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;0\textup{&space;if&space;}p_x(t&plus;1)-p_x(t)&space;=&space;0\\&space;-1\textup{&space;if&space;}p_x(t&plus;1)-p_x(t)&space;<&space;0&space;\end{matrix}\right." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;1\textup{&space;if&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;0\textup{&space;if&space;}p_x(t&plus;1)-p_x(t)&space;=&space;0\\&space;-1\textup{&space;if&space;}p_x(t&plus;1)-p_x(t)&space;<&space;0&space;\end{matrix}\right." title="\Delta p_x(t) = \left\{\begin{matrix} 1\textup{ if }p_x(t+1)-p_x(t) > 0\\ 0\textup{ if }p_x(t+1)-p_x(t) = 0\\ -1\textup{ if }p_x(t+1)-p_x(t) < 0 \end{matrix}\right." /></a>

Let the second-order price differential <br /> <a href="https://www.codecogs.com/eqnedit.php?latex=\Delta^2&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;(1,1)\textup{&space;if&space;}p_x(t&plus;2)-p_x(t-1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,0)\textup{&space;if&space;}p_x(t&plus;2)-p_x(t-1)&space;=&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,-1)\textup{&space;if&space;}p_x(t&plus;2)-p_x(t-1)&space;<&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;etc.&space;\end{matrix}\right." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta^2&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;(1,1)\textup{&space;if&space;}p_x(t&plus;2)-p_x(t-1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,0)\textup{&space;if&space;}p_x(t&plus;2)-p_x(t-1)&space;=&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,-1)\textup{&space;if&space;}p_x(t&plus;2)-p_x(t-1)&space;<&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;etc.&space;\end{matrix}\right." title="\Delta^2 p_x(t) = \left\{\begin{matrix} (1,1)\textup{ if }p_x(t+2)-p_x(t-1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,0)\textup{ if }p_x(t+2)-p_x(t-1) = 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,-1)\textup{ if }p_x(t+2)-p_x(t-1) < 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ etc. \end{matrix}\right." /></a>

Let the third-order price differential <br /><a href="https://www.codecogs.com/eqnedit.php?latex=\Delta^3&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;(1,1,1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,0)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;=&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,-1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;<&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;etc.&space;\end{matrix}\right." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta^3&space;p_x(t)&space;=&space;\left\{\begin{matrix}&space;(1,1,1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,0)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;=&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;(1,1,-1)\textup{&space;if&space;}p_x(t&plus;3)-p_x(t-2)&space;<&space;0\textup{&space;and&space;}p_x(t&plus;2)-p_x(t&plus;1)&space;>&space;0\textup{&space;and&space;}p_x(t&plus;1)-p_x(t)&space;>&space;0\\&space;etc.&space;\end{matrix}\right." title="\Delta^3 p_x(t) = \left\{\begin{matrix} (1,1,1)\textup{ if }p_x(t+3)-p_x(t-2) > 0\textup{ and }p_x(t+2)-p_x(t+1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,1,0)\textup{ if }p_x(t+3)-p_x(t-2) = 0\textup{ and }p_x(t+2)-p_x(t+1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ (1,1,-1)\textup{ if }p_x(t+3)-p_x(t-2) < 0\textup{ and }p_x(t+2)-p_x(t+1) > 0\textup{ and }p_x(t+1)-p_x(t) > 0\\ etc. \end{matrix}\right." /></a>

My hypothesis was that <a href="https://www.codecogs.com/eqnedit.php?latex=\Delta^3&space;p_x(t)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta^3&space;p_x(t)" title="\Delta^3 p_x(t)" /></a> is a Markov chain, i.e.,
<a href="https://www.codecogs.com/eqnedit.php?latex=\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1},\Delta^3&space;p_x(t-2)&space;=&space;k_{t-2},...,&space;\Delta^3&space;p_x(0)&space;=&space;k_{0}&space;\right&space;)&space;\\\indent&space;=&space;\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1}\right&space;)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1},\Delta^3&space;p_x(t-2)&space;=&space;k_{t-2},...,&space;\Delta^3&space;p_x(0)&space;=&space;k_{0}&space;\right&space;)&space;\\\indent&space;=&space;\mathbb{P}&space;\left&space;(\Delta^3&space;p_x(t)&space;=&space;k_t&space;|&space;\Delta^3&space;p_x(t-1)&space;=&space;k_{t-1}\right&space;)" title="\mathbb{P} \left (\Delta^3 p_x(t) = k_t | \Delta^3 p_x(t-1) = k_{t-1},\Delta^3 p_x(t-2) = k_{t-2},..., \Delta^3 p_x(0) = k_{0} \right ) \\\indent = \mathbb{P} \left (\Delta^3 p_x(t) = k_t | \Delta^3 p_x(t-1) = k_{t-1}\right )" /></a><br /> More specifically, that 3 is the smallest n for which <a href="https://www.codecogs.com/eqnedit.php?latex=\Delta^n&space;p_x(t)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Delta^n&space;p_x(t)" title="\Delta^n p_x(t)" /></a> is a Markov chain.

A short Python script was written to generate these a time series of these price change directions, in the first, second, third, and fourth order. Then, a short R script was used to verify the Markov property in these time series using the markovchain package, which did not have an equivalent in Python. My hypothesis will indeed be true if the test for first order and second order fails, but the test for the third order passes and continues to pass for higher orders.
