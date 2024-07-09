# Problem 

A box contains 7 indistinguishable green balls, 5 indistinguishable white balls, and 6 indistinguishable black balls. Suppose balls are drawn using simple random sampling with replacement until balls of all colours are obtained. Let $N$ denote the minimum number of draws needed to achieve this.
* (a) For each nonnegative integer $n$, calculate $\mathbb{P}(N>n)$.
* (b) Using (a) or otherwise, compute $\mathbb{E}(N)$.

# Solution

* $N$ is the minimum number of draws needed to get at least one ball of each colour.
* You can observe that the minimum number of draws needed is 3, and the maximum number of draws needed is $7+6+1 = 14$. Therefore $3 \leq N \leq 14$. It is important to note, that whenever you want to find the distribution of a random variable, the first thing, you should note is the range of the random variable.
* The problem asks you to find the probability distribution of $N$, and therefore find $\mathbb{P}(N>n)$, and $\mathbb{E}(N)$.


```math
\mathbb{P}(N_{G} = k) = 
\begin{cases} 
\frac{\binom{11}{k-1} - \binom{5}{k-1} - \binom{6}{k-1}}{\binom{18}{k-1}} \times \frac{7}{19-k} & \text{if } 3 \le k \le 6 \\ 
\frac{\binom{11}{k-1} - 1}{\binom{18}{k-1}} \times \frac{7}{19-k} & \text{if } k = 7 \\
\frac{\binom{11}{k-1}}{\binom{18}{k-1}} \times \frac{7}{19-k} & \text{if } 8 \le k \le 12 
\end{cases}
```

```math
\mathbb{P}(N_{B} = k) = 
\begin{cases} 
\frac{\binom{12}{k-1} - \binom{5}{k-1} - \binom{7}{k-1}}{\binom{18}{k-1}} \times \frac{6}{19-k} & \text{if } 3 \le k \le 6 \\ 
\frac{\binom{12}{k-1} - 1}{\binom{18}{k-1}} \times \frac{6}{19-k} & \text{if } 7 \leq k \leq 8 \\
\frac{\binom{12}{k-1}}{\binom{18}{k-1}} \times \frac{6}{19-k} & \text{if } 9 \leq k \leq 13 
\end{cases}
```

```math
\mathbb{P}(N_{W} = k) = 
\begin{cases} 
\frac{\binom{13}{k-1} - \binom{6}{k-1} - \binom{7}{k-1}}{\binom{18}{k-1}} \times \frac{5}{19-k} & \text{if } 3 \le k \le 7 \\ 
\frac{\binom{13}{k-1} - 1}{\binom{18}{k-1}} \times \frac{5}{19-k} & \text{if } k = 8 \\
\frac{\binom{13}{k-1}}{\binom{18}{k-1}} \times \frac{5}{19-k} & \text{if } 9 \leq k \leq 14
\end{cases}
```
