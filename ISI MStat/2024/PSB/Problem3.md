# Problem 

A box contains 7 indistinguishable green balls, 5 indistinguishable white balls, and 6 indistinguishable black balls. Suppose balls are drawn using simple random sampling with replacement until balls of all colours are obtained. Let $N$ denote the minimum number of draws needed to achieve this.
* (a) For each nonnegative integer $n$, calculate $\mathbb{P}(N>n)$.
* (b) Using (a) or otherwise, compute $\mathbb{E}(N)$.

# Solution

* $N$ is the minimum number of draws needed to get at least one ball of each colour.
* You can observe that the minimum number of draws needed is 3, and the maximum number of draws needed is $7+6+1 = 14$. Therefore $3 \leq N \leq 14$. It is important to note, that whenever you want to find the distribution of a random variable, the first thing, you should note is the range of the random variable.
* The problem asks you to find the probability distribution of $N$, and therefore find $\mathbb{P}(N>n)$, and $\mathbb{E}(N)$.
* 
