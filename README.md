# ee5251---problem-set-3-solved
**TO GET THIS SOLUTION VISIT:** [EE5251 – PROBLEM SET #3 Solved](https://www.ankitcodinghub.com/product/ee5251-problem-set-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117077&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EE5251 - PROBLEM SET #3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Problem 1

Do Problem 4.4 in your text. The point of this problem is to show you how to convert a

continuous-time model (as you would derive from laws of physics) to a discrete-time model you can simulate on a computer. It is based on the example on page 20 of the text. You will have to do all the calculations by hand because we expect your answers to be in terms of k, i and T (the sampling interval). You can check your answer using MATLAB’s command c2d(A,B), for example, for a specific T.

Problem 2

The purpose of this problem is to drive home the concepts of state prediction and covariance propagation. To that end, let us consider the following dynamic system:

x˙ = w, E [w] = 0, E [w(t)w(τ)] = Qcδ (t − τ), Qc = 1

a) Write down the A and B matrix for the state-space realization of this system.

b) Calculate the F and G matrices for the discrete version of this system when the sampling interval is T = 1 seconds.

c) Evaluate the discrete process noise covariance Q.

√

d) Simulate the system for 0 ≤ t ≤ 50 seconds with T = 1 seconds. Since σwk = Q, you an generate a history for wk in MATLAB as follows:

&gt;&gt; T = 1;

&gt;&gt; t = 0:T:50;

&gt;&gt; N = length(t);

&gt;&gt; w_k = sqrt(Q)*randn(N,1);

The output of your simulation will be a history of xk for k = 0,1,2,…,N − 1 where x0 = 0. Repeat this simulation 100 times and plot. Plot all 100 of the time series on the same graph of tk vs. xk. Now that you have 100 different traces, calculate the ensemble standard deviation at tk = 5, tk = 25 and tk = 50 seconds. What you just did is called a Monte Carlo simulation.

e) Now calculate the state prediction error covariance assuming you have perfect knowledge of the state (no uncertainty in the estimate) at k = 0. Plot the +σ and −σ on the same graph as the one in part (d) above. What are the values of σ at tk = 5 and tk = 10 seconds? This is called covariance analysis.

f) If you did things correctly, the standard deviation estimated by the Monte Carlo simulation should be very close to those predicted by the covariance analysis. So, now imagine that you are highly-paid consultant (because you took AEM 5451/EE 5251) and asked to design an estimator for a system that is going to be used in a safetycritical application (e.g., medical device design, commercial aviation, nuclear power generation, etc). You must prove that the uncertainty in your state estimate is very small. Which approach would you use–Monte Carlo or covariance analysis? Why?

Problem 3

Do problem 5.9 in your text including the following additional question:

c) Is your solution in part a) consistent with your understanding or engineer’s intuition about how Kalman Filters should work? Why or why not? What about your answer in part b)?

Problem 4

Do problem 5.11 in your text. Note that part c) of this problem is asking you the same thing that you were asked in Problem 2, d) &amp; e). The term “theoretical standard deviation” means the standard deviation you would calculate by doing a covariance analysis.

Problem 5

Do problem 9.17 in your text. In this problem you are designing a smoother for the system you worked with in Problem 4 above.

Problem 6

A rather common problem that appears regularly in signal processing is that of estimating the total phase ϕk = 2πftk + θ. The frequency of the signal f is known and, thus, the

2

dynamic model is ˙ϕ = 2πf. The measurement model relates a measurement of its amplitude yk to ϕk as follows:

yk = sinϕk + vk, vk ∼ N(0,Rk)

This is a nonlinear measurement model. What we want to show in this problem is how a nonlinear measurement model results in a predicted measurement ˆyk with a distribution that is very different from that of a priori one or that of the measurement y.

a) Derive an analytical expression for fYb(y)sinϕ when ϕ ∼ U(0,π)?

b) Determine ) and when ϕ ∼ U(0,π).

c) Using MATLAB draw 10,000 samples of ϕ and run a simple Monte Carlo experiment to generate samples of ˆy. Using the generated data approximate E(Yb) and (you can use the MATLAB commands mean and var). Also plot a histogram-based approximation of fY (y). To do this, use the hist command in MATLAB (use at least 50 bins with hist). How well do the Monte Carlo results for and fYb(y)sinϕ agree to the analytical results?

d) Use the analytical approach or a Monte Carlo simulation (your choice) to determine

E(Yb), σY2b and fYb(y)sinϕ when ϕ ∼ N(0,1). Which approach did you use (analytical or Monte Carlo)? Why?

3
