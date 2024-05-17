# Theory

Zero-order hold (ZOH) devices convert sampled signals to continuoustime signals for analyzing sampled continuous-time systems. 
The zero-order hold discretization of a continuous-time LTI model is depicted in the Fig. 1.

<div align="center">
<img class="img-fluid"  src= "./images/ZOH block.jpg" alt="">

<figcaption style="color:black"> Fig.1. Block diagram of Zero-order hold </figcaption>
</div>

The ZOH device generates a continuous input signal u(t) by holding each sample value u[k] constant over one sample period. 

<img style="margin-left:auto;margin-right:auto;" src= "./images/u(t) = u(k).jpg">


First-order hold (FOH) differs from ZOH by the underlying hold mechanism.

To turn the input samples into a continuous input, FOH uses linear interpolation between samples.

<img style="margin-left:auto;margin-right:auto;" src= "./images/eq2.jpg">


The transfer functions for these circuits are given as 

For ZOH 

<img style="margin-left:auto;margin-right:auto;" src= "./images/ZOH.jpg">


For FOH  

<img style="margin-left:auto;margin-right:auto;" src= "./images/FOH.jpg">


Practical implementable transfer functions are obtained using approximations of exponential series. (Pade Approximations)


<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>