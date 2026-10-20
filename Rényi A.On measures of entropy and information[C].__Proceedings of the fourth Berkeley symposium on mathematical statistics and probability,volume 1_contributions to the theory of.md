# ON MEASURES OF ENTROPY AND INFORMATION

ALFRED RÉNYI
MATHEMATICAL INSTITUTE
HUNGARIAN ACADEMY OF SCIENCES

## 1. Characterization of Shannon's measure of entropy

Let $\mathcal{P} = (p_1, p_2, \cdots, p_n)$ be a finite discrete probability distribution, that is, suppose $p_k \geq 0 (k = 1, 2, \cdots, n)$ and $\sum_{k=1}^{n} p_k = 1$. The amount of uncertainty of the distribution $\mathcal{P}$, that is, the amount of uncertainty concerning the outcome of an experiment, the possible results of which have the probabilities $p_1, p_2, \cdots, p_n$, is called the entropy of the distribution $\mathcal{P}$ and is usually measured by the quantity $H[\mathcal{P}] = H(p_1, p_2, \cdots, p_n)$, introduced by Shannon [1] and defined by

$$
H (p _ {1}, p _ {2}, \dots , p _ {n}) = \sum_ {k = 1} ^ {n} p _ {k} \log_ {2} \frac {1}{p _ {k}}.\tag{1.1}
$$

Different sets of postulates have been given, which characterize the quantity (1.1). The simplest such set of postulates is that given by Fadeev [2] (see also Feinstein [3]). Fadeev's postulates are as follows.

(a) $H(p_{1}, p_{2}, \dots, p_{n})$ is a symmetric function of its variables for $n = 2, 3, \dots$.

(b) $H(p,1 - p)$ is a continuous function of $p$ for $0\leq p\leq 1$.

(c) $H(1 / 2,1 / 2) = 1$

$$
(\mathrm{d}) H [ t p _ {1}, (1 - t) p _ {1}, p _ {2}, \dots , p _ {n} ] = H (p _ {1}, p _ {2}, \dots , p _ {n}) + p _ {1} H (t, 1 - t)
$$

for any distribution $\mathcal{P} = (p_1, p_2, \cdots, p_n)$ and for $0 \leq t \leq 1$.

The proof that the postulates (a), (b), (c), and (d) characterize the quantity (1.1) uniquely is easy except for the following lemma, whose proofs up to now are rather intricate.

LEMMA. Let $f(n)$ be an additive number-theoretical function, that is, let $f(n)$ be defined for $n = 1, 2, \cdots$ and suppose

$$
f (n m) = f (n) + f (m), \quad \quad \quad n, m = 1, 2, \dots .\tag{1.2}
$$

Let us suppose further that

$$
\lim _ {n \to + \infty} [ f (n + 1) - f (n) ] = 0.\tag{1.3}
$$

Then we have

$$
f (n) = c \log n,\tag{1.4}
$$

where $c$ is a constant.

This lemma was first proved by Erdős [4]. In fact Erdős proved somewhat more, namely he supposed, as is usual in number theory, the validity of (1.2) only for n and m being relatively prime. Later the lemma was rediscovered by Fadeev. The proofs of both Erdős and Fadeev are rather complicated. In this section we give a new proof of the lemma, which is much simpler.

PROOF. Let $N > 1$ be an arbitrary integer and let us put

$$
g (n) = f (n) - \frac {f (N) \log n}{\log N}, \quad \quad \quad \quad \quad \quad \quad n = 1, 2, \dots .\tag{1.5}
$$

It follows evidently from (1.2) and (1.3) that

$$
g (n m) = g (n) + g (m), \quad \quad \quad n, m = 1, 2, \dots\tag{1.6}
$$

and that

$$
\lim _ {n \to + \infty} \left[ g (n + 1) - g (n) \right] = 0.\tag{1.7}
$$

We have further

$$
g (N) = 0.\tag{1.8}
$$

Let us now put $G(-1) = 0$ and

$$
G (k) = \max _ {N ^ {k} \leq n <   N ^ {k + 1}} | g (n) |, \quad k = 0, 1, \dots ,\tag{1.9}
$$

and further,

$$
\delta_ {k} = \max _ {N ^ {k} \leq n <   N ^ {k + 1}} | g (n + 1) - g (n) |, \quad k = 0, 1, \dots .\tag{1.10}
$$

Clearly we have

$$
\lim _ {k \to + \infty} \delta_ {k} = 0.\tag{1.11}
$$

Now we shall prove that

$$
\lim _ {n \to + \infty} \frac {g (n)}{\log n} = 0.\tag{1.12}
$$

Since for $N^k \leq n < N^{k+1}$, we have $|g(n)|/\log n \leq G(k)/k \log N$, in order to prove (1.12) it is clearly sufficient to prove that

$$
\lim _ {k \to + \infty} \frac {G (k)}{k} = 0.\tag{1.13}
$$

Now let $n$ be an arbitrary integer and let $k$ be defined by the inequalities $N^k \leq n < N^{k+1}$. Let us put $n' = N[n/N]$ where $[x]$ denotes the integral part of $x$; thus $n'$ is the greatest multiple of $N$ not exceeding $n$. Then we have evidently $0 \leq n - n' < N$ and thus

$$
\left| g (n) \right| \leq \left| g (n ^ {\prime}) \right| + \sum_ {l = n ^ {\prime}} ^ {n - 1} \left| g (l + 1) - g (l) \right| \leq \left| g (n ^ {\prime}) \right| + N \delta_ {k}.\tag{1.14}
$$

By (1.6) and (1.8) we have

$$
g (n ^ {\prime}) = g \left(\left[ \frac {n}{N} \right]\right) + g (N) = g \left(\left[ \frac {n}{N} \right]\right),\tag{1.15}
$$

and hence the inequalities $N^{k-1} \leq [n/N] < N^k$, together with (1.14), imply that (1.16) $G(k) \leq G(k-1) + N\delta_k, \quad k = 0, 1, \cdots$.

Adding the inequalities (1.16) for $k = 0, 1, \dots, m$, it follows that

$$
\frac {G (m)}{m} \leq N \left(\frac {\delta_ {0} + \delta_ {1} + \cdots + \delta_ {m}}{m}\right).\tag{1.17}
$$

Taking (1.11) into account, we obtain (1.13) and so (1.12). But clearly (1.12) implies

$$
\lim _ {n \to + \infty} \frac {f (n)}{\log n} = \frac {f (N)}{\log N}.\tag{1.18}
$$

As N was an arbitrary integer greater than 1 and the left side of (1.18) does not depend on N, it follows that, denoting by c the value of the limit on the left side of (1.18), we have

$$
f (N) = c \log N,\tag{1.19}
$$

$$
N = 2, 3, \dots .
$$

By (1.2) we have evidently $f(1) = 0$. Thus the lemma is proved.

With a slight modification the above proof applies also in the case when the validity of  $(1.2)$  is supposed only for relatively prime m and n. A previous version of the above proof has been given by the author in [5]. The version given above is somewhat simpler than in [5].

Let us add some remarks on the set of postulates (a) to (d). Let us denote  $\mathcal{P} = (p_{1}, p_{2}, \cdots, p_{m})$  and  $\mathcal{Q} = (q_{1}, q_{2}, \cdots, q_{n})$  as two probability distributions. Let us denote by  $P * Q$  the direct product of the distributions P and Q, that is, the distribution consisting of the numbers  $p_{j}q_{k}$  with  $j = 1, 2, \cdots, m; k = 1, 2, \cdots, n$ . Then we have from (1.1)

$$
H [ \wp * \mathbb {Q} ] = H [ \wp ] + H [ \mathbb {Q} ],\tag{1.20}
$$

which expresses one of the most important properties of entropy, namely, its additivity: the entropy of a combined experiment consisting of the performance of two independent experiments is equal to the sum of the entropies of these two experiments. It is easy to see that one cannot replace the postulate (d) by (1.20) because (1.20) is much weaker. As a matter of fact there are many quantities other than (1.1) which satisfy the postulates (a), (b), (c), and (1.20). For instance, all the quantities

$$
H _ {\alpha} (p _ {1}, p _ {2}, \dots , p _ {n}) = \frac {1}{1 - \alpha} \log_ {2} \left(\sum_ {k = 1} ^ {n} p _ {k} ^ {\alpha}\right),\tag{1.21}
$$

where  $\alpha > 0$  and  $\alpha \neq 1$  have these properties. The quantity  $H_{\alpha}(p_{1}, p_{2}, \cdots, p_{n})$  defined by (1.21) can also be regarded as a measure of the entropy of the distribution  $\mathcal{P} = (p_{1}, \cdots, p_{n})$ . In what follows we shall call

$$
H _ {\alpha} (p _ {1}, p _ {2}, \dots , p _ {n}) = H _ {\alpha} [ \mathcal {O} ]
$$

the entropy of order $\alpha$ of the distribution $\wp$. We shall deal with these quantities in the next sections. Here we mention only that, as is easily seen,

$$
\lim _ {\alpha \to 1} H _ {\alpha} (p _ {1}, p _ {2}, \dots , p _ {n}) = \sum_ {k = 1} ^ {n} p _ {k} \log_ {2} \frac {1}{p _ {k}}.\tag{1.22}
$$

Thus Shannon's measure of entropy is the limiting case for $\alpha\to1$ of the measure of entropy $H_{\alpha}[\varnothing]$. In view of (1.22) we shall denote in what follows Shannon's measure of entropy (1.1) by $H_{1}(p_{1},\cdots,p_{n})$ and call it the measure of entropy of order 1 of the distribution. Thus we put

$$
H _ {1} [ \varnothing ] = H _ {1} (p _ {1}, p _ {2}, \dots , p _ {n}) = \sum_ {k = 1} ^ {n} p _ {k} \log_ {2} \frac {1}{p _ {k}}.\tag{1.23}
$$

There are besides the quantities (1.22) still others which satisfy the postulates (a), (b), (c), and (1.20). For instance, applying a linear operation on $H_{\alpha}[\varphi]$ as a function of $\alpha$ we get again such a quantity. In the next section we shall show what additional postulate is needed besides (a), (b), (c), and (1.20) to characterize the entropy of order 1. We shall see that in order to get such a characterization of Shannon's entropy, it is advantageous to extend the notion of a probability distribution, and define entropy for these generalized distributions.

## 2. Characterization of Shannon's measure of entropy of generalized probability distributions

The characterization of measures of entropy (and information) becomes much simpler if we consider these quantities as defined on the set of generalized probability distributions. Let $[\Omega, \mathfrak{B}, P]$ be a probability space, that is, $\Omega$ an arbitrary nonempty set, called the set of elementary events; $\mathfrak{B}$ a $\sigma$-algebra of subsets of $\Omega$, containing $\Omega$ itself, the elements of $\mathfrak{B}$ being called events; and $P$ a probability measure, that is, a nonnegative and additive set function for which $P(\Omega) = 1$, defined on $\mathfrak{B}$. Let us call a function $\xi = \xi(\omega)$ which is defined for $\omega \in \Omega_1$ where $\Omega_1 \in \mathfrak{B}$ and $P(\Omega_1) > 0$, and which is measurable with respect to $\mathfrak{B}$, a generalized random variable. If $P(\Omega_1) = 1$ we call $\xi$ an ordinary (or complete) random variable, while if $0 < P(\Omega_1) < 1$ we call $\xi$ an incomplete random variable. Clearly, an incomplete random variable can be interpreted as a quantity describing the result of an experiment depending on chance which is not always observable, only with probability $P(\Omega_1) < 1$. The distribution of a generalized random variable will be called a generalized probability distribution. In particular, in the case when $\xi$ takes on only a finite number of different values $x_1, x_2, \cdots, x_n$, the distribution of $\xi$ consists of the set of numbers $p_k = P\{\xi = x_k\}$ for $k = 1, 2, \cdots, n$. Thus a finite discrete generalized probability distribution is simply a sequence $p_1, p_2, \cdots, p_n$ of nonnegative numbers such that putting $\mathfrak{P} = (p_1, p_2, \cdots, p_n)$ and

$$
W (\wp) = \sum_ {k = 1} ^ {n} p _ {k},\tag{2.1}
$$

we have

$$
0 <   W (\mathcal {P}) \leq 1.\tag{2.2}
$$

We shall call $W(\mathcal{P})$ the weight of the distribution. Thus the weight of an ordinary distribution is equal to 1. A distribution which has a weight less than 1 will be called an incomplete distribution.

Let $\Delta$ denote the set of all finite discrete generalized probability distributions, that is, $\Delta$ is the set of all sequences $\mathcal{P} = (p_1, p_2, \cdots, p_n)$ of nonnegative numbers such that $0 < \sum_{k=1}^{n} p_k \leq 1$. We shall characterize the entropy $H[\mathcal{P}]$ (of order 1) of a generalized probability distribution $\mathcal{P} = (p_1, \cdots, p_n)$ by the following five postulates.

POSTULATE 1. $H[\mathcal{P}]$ is a symmetric function of the elements of $\mathcal{P}$.

POSTULATE 2. If $\{p\}$ denotes the generalized probability distribution consisting of the single probability $p$ then $H[\{p\}]$ is a continuous function of $p$ in the interval $0 < p \leq 1$. Note that the continuity of $H[\{p\}]$ is supposed only for $p > 0$, but not for $p = 0$.

POSTULATE 3. $H[\{1 / 2\}] = 1$

POSTULATE 4. For $\mathcal{P} \in \Delta$ and $\mathcal{Q} \in \Delta$ we have $H[\mathcal{P} * \mathcal{Q}] = H[\mathcal{P}] + H[\mathcal{Q}]$.

Before stating our last postulate we introduce some notation. If we denote  $\mathcal{P} = (p_{1}, p_{2}, \cdots, p_{m})$  and  $\mathcal{Q} = (q_{1}, q_{2}, \cdots, q_{n})$  as two generalized distributions such that  $W(\mathcal{P}) + W(\mathcal{Q}) \leq 1$ , we put

$$
\mathcal {P} \cup \mathcal {Q} = (p _ {1}, p _ {2}, \dots , p _ {m}, q _ {1}, q _ {2}, \dots , q _ {n}).\tag{2.3}
$$

If $W(\mathcal{P}) + W(\mathcal{Q}) > 1$ then $\mathcal{P} \cup \mathcal{Q}$ is not defined. Now we can state our last postulate.

POSTULATE 5. If $\mathcal{P} \in \Delta$, $\mathfrak{Q} \in \Delta$, and $W(\mathcal{P}) + W(\mathfrak{Q}) \leq 1$, we have

$$
H [ \mathcal {P} \cup \mathcal {Q} ] = \frac {W (\mathcal {P}) H [ \mathcal {P} ] + W (\mathcal {Q}) H [ \mathcal {Q} ]}{W (\mathcal {P}) + W (\mathcal {Q})}.\tag{2.4}
$$

Postulate 5 may be called the mean-value property of entropy; the entropy of the union of two incomplete distributions is the weighted mean value of the entropies of the two distributions, where the entropy of each component is weighted with its own weight. One of the advantages of defining the entropy for generalized distributions, and not merely for ordinary (complete) distributions, is that this mean-value property is much simpler in the general case.

We now prove

THEOREM 1. If $H[\mathcal{P}]$ is defined for all $\mathcal{P} \in \Delta$ and satisfies the postulates 1, 2, 3, 4, and 5, then $H[\mathcal{P}] = H_1[\mathcal{P}]$, where

$$
H _ {1} [ \varphi ] = \frac {\sum_ {k = 1} ^ {n} p _ {k} \log_ {2} \frac {1}{p _ {k}}}{\sum_ {k = 1} ^ {n} p _ {k}}.\tag{2.5}
$$

PROOF. The proof is very simple. Let us put

$$
h (p) = H [ \{p \} ],\tag{2.6}
$$

$$
0 <   p \leq 1,
$$

where  $\{p\}$  again denotes the generalized distribution consisting of the single probability p. We have by postulate 4

$$
h (p q) = h (p) + h (q) \quad \text {for} 0 <   p \leq 1; \quad 0 <   q \leq 1.\tag{2.7}
$$

By postulate 2, $h(p)$ is continuous for $0 < p \leq 1$ and by postulate 3 we have $h(1/2) = 1$. Thus it follows that

$$
h (p) = H [ \{p \} ] = \log_ {2} \frac {1}{p}.\tag{2.8}
$$

Now it follows from postulate 5 by induction that if $\mathcal{P}_s, \mathcal{P}_2, \dots, \mathcal{P}_n$ are incomplete distributions such that $\sum_{k=1}^{n} w(\mathcal{P}_k) \leq 1$, then

$$
\begin{array}{r l} H [ \wp_ {1} \cup \wp_ {2} \cup \dots \cup \wp_ {n} ] \\ & = \frac {w (\wp_ {1}) H [ \wp_ {1} ] + w (\wp_ {2}) H [ \wp_ {2} ] + \cdots + w (\dot {\wp} _ {n}) H [ \wp_ {n} ]}{w (\wp_ {1}) + w (\wp_ {2}) + \cdots + w (\wp_ {n})}. \end{array}\tag{2.9}
$$

As any generalized distribution  $\mathcal{P} = (p_{1}, p_{2}, \cdots, p_{n})$  can be written in the form

$$
\mathcal {P} = \{p _ {1} \} \cup \{p _ {2} \} \cup \dots \cup \{p _ {n} \},\tag{2.10}
$$

the assertion of theorem 1 follows from (2.9) and (2.10).

An advantage of the above introduction of the notion of entropy is that the term  $\log_{2}(1/p_{k})$  in Shannon's formula is interpreted as the entropy of the generalized distribution consisting of the single probability  $p_{k}$  and thus it becomes evident that (1.1) is really a mean value. This point of view was emphasized previously by some authors, especially by G. A. Barnard [6].

The question arises of what other quantity is obtained if we replace in postulate 5 the arithmetic mean by some other mean value. The general form of a mean value of the numbers $x_{1}, x_{2}, \cdots, x_{n}$ taken with the weights $w_{1}, w_{2}, \cdots, w_{n}$, where $w_{k} > 0$ and $\sum_{k=1}^{n} w_{k} = 1$, is usually written in the form (for example, see [7])

$$
g ^ {- 1} \left[ \sum_ {k = 1} ^ {n} w _ {k} g (x _ {k}) \right],\tag{2.11}
$$

where  $y = g(x)$  is an arbitrary strictly monotonic and continuous function and  $x = g^{-1}(y)$  denotes the inverse function of  $y = g(x)$ . The function  $g(x)$  is called the Kolmogorov-Nagumo function corresponding to the mean value (2.10). Thus we are led to replace postulate 5 by

POSTULATE 5'. There exists a strictly monotonic and continuous function $y = g(x)$ such that if $\mathcal{P} \in \Delta, \mathbb{Q} \in \Delta$, and $w(\mathcal{P}) + w(\mathbb{Q}) \leq 1$, we have

$$
H [ \mathcal {P} \cup \mathbb {Q} ] = g ^ {- 1} \bigg [ \frac {w (\mathcal {P}) g (H [ \mathcal {P} ]) + w (\mathbb {Q}) g (H [ \mathbb {Q} ])}{w (\mathcal {P}) + w (\mathbb {Q})} \bigg ].\tag{2.12}
$$

It is an open question which choices of the function $g(x)$ are admissible, that is, are such that postulate $5'$ is compatible with 4. Clearly, if $g(x) = ax + b$ with $a \neq 0$, then postulate $5'$ reduces to 5. Another choice of $g(x)$ which is admissible is to choose $g(x)$ to be an exponential function. If $g(x) = g_{\alpha}(x)$ where $\alpha > 0$, $\alpha \neq 1$, and

$$
g _ {\alpha} (x) = 2 ^ {(\alpha - 1) x},\tag{2.13}
$$

then postulates 1, 2, 3, 4, and $5'$ characterize the entropy of order $\alpha$. In other words the following theorem is valid.

THEOREM 2. If $H[\mathcal{O}]$ is defined for all $\mathcal{O} \in \Delta$ and satisfies postulates 1, 2, 3, 4, and $5'$ with $g(x) = g_{\alpha}(x)$, where $g_{\alpha}(x)$ is defined by (2.13), $\alpha > 0$, and $\alpha \neq 1$, then $H[\mathcal{O}] = H_{\alpha}[\mathcal{O}]$, where, putting $\mathcal{O} = (p_1, p_2, \cdots, p_n)$, we have

$$
H _ {\alpha} [ \wp ] = \frac {1}{1 - \alpha} \log_ {2} \left[ \frac {\sum_ {k = 1} ^ {n} p _ {k} ^ {\alpha}}{\sum_ {k = 1} ^ {n} p _ {k}} \right].\tag{2.14}
$$

The quantity (2.14) will be called the entropy of order  $\alpha$  of the generalized distribution P. Clearly if P is an ordinary distribution, (2.14) reduces to (1.21). It is also easily seen that

$$
\lim _ {\alpha \to 1} H _ {\alpha} [ \varphi ] = H _ {1} [ \varphi ],\tag{2.15}
$$

where $H_{1}[\mathcal{P}]$ is defined by (2.5).

The fact that $H_{\alpha}[\mathcal{P}]$ is characterized by the same properties as $H_{1}[\mathcal{P}]$, with only the difference that instead of the arithmetic mean value in postulate 5 we have an exponential mean value in $5'$, and the fact that $H_{1}[\mathcal{P}]$ is a limiting case of $H_{\alpha}[\mathcal{P}]$ for $\alpha \to 1$, both indicate that it is appropriate to consider $H_{\alpha}[\mathcal{P}]$ also as a measure of entropy of the distribution $\mathcal{P}$. In the next section we shall show that if we formulate the problem in a more general form, the only admissible choices of the function $g(x)$ are those considered above. That is, that $g(x)$ has to be either a linear or an exponential function.

## 3. Characterization of the amount of information $\mathrm{I}(\mathbb{Q}|\mathbb{P})$

The entropy of a probability distribution can be interpreted not only as a measure of uncertainty but also as a measure of information. As a matter of fact, the amount of information which we get when we observe the result of an experiment (depending on chance) can be taken numerically equal to the amount of uncertainty concerning the outcome of the experiment before carrying it out.

There are however also other amounts of information which are often considered. For instance we may ask what is the amount of information concerning a random variable $\xi$ obtained from observing an event $E$, which is in some way connected with the random variable $\xi$. If $\mathcal{P}$ denotes the original (unconditional) distribution of the random variable $\xi$ and $\mathcal{Q}$ the conditional distribution of $\mathfrak{Z}$ under the condition that the event $E$ has taken place, we shall denote a measure of the amount of information concerning the random variable $\xi$ contained in the observation of the event $E$ by $I(\mathcal{Q}|\mathcal{P})$. Clearly $\mathcal{Q}$ is always absolutely continuous with respect to $\mathcal{P}$; thus the quantity $I(\mathcal{Q}|\mathcal{P})$ will be defined only if $\mathcal{Q}$ is absolutely continuous with respect to $\mathcal{P}$. Denoting by $h = d\mathcal{Q}/d\mathcal{P}$ the Radon-Nikodym derivative of $\mathcal{Q}$ with respect to $\mathcal{P}$, a possible measure of the amount of information in question is

$$
\left| I _ {1} (\mathbb {Q} | \mathcal {P}) = \int_ {\Omega} \log_ {2} h d \mathbb {Q} = \int_ {\Omega} h \log_ {2} h d \mathcal {P}. \right.\tag{3.1}
$$

In the case when the random variable $\xi$ takes on only a finite number of different values $x_{1}, x_{2}, \cdots, x_{n}$ and we put $P\{\xi = x_{k}\} = p_{k}$ and $P\{\xi = x_{k}|E\} = q_{k}$ for $k = 1, 2, \cdots, n$, then (3.1) reduces to

$$
I _ {1} (\mathbb {Q} | \mathcal {P}) = \sum_ {k = 1} ^ {n} q _ {k} \log_ {2} \frac {q _ {k}}{p _ {k}}.\tag{3.2}
$$

It should however be added that other interpretations of the quantity (3.1) or of (3.2) have also been given (see Kullback [8], where further literature is also indicated). Notice that the quantity (3.2) is defined for two finite discrete probability distributions  $\mathcal{P} = (p_{1}, \cdots, p_{n})$  and  $\mathcal{Q} = (q_{1}, \cdots, q_{n})$  only if  $p_{k} > 0$  for  $k = 1, 2, \cdots, n$  (among the  $q_{k}$  there may be zeros) and if there is given a one-to-one correspondence between the elements of the distribution P and Q, which must therefore consist of an equal number of terms. It follows easily from Jensen's inequality (see, for example, [7]) that the quantities (3.1) or (3.2) are always nonnegative, and they are equal to 0 if and only if the distributions P and Q are identical.

While many systems of postulates have been given to characterize the entropy, it seems that a similar characterization of the quantity (3.2) has not been attempted. In this section we shall characterize the quantity (3.2) by certain intuitively evident postulates. At the same time we shall consider also other possible measures of the amount of information in question. It turns out that the only alternative quantities are the quantities

$$
I _ {\alpha} (\mathbb {Q} | \varPhi) = \frac {1}{\alpha - 1} \log_ {2} \left(\sum_ {k = 1} ^ {n} \frac {q _ {k} ^ {\alpha}}{p _ {k} ^ {\alpha - 1}}\right),\tag{3.3}
$$

where $\alpha \neq 1$. Evidently we have

$$
\lim _ {\alpha \to 1} I _ {\alpha} (\mathfrak {Q} | \mathcal {P}) = I _ {1} (\mathfrak {Q} | \mathcal {P}).\tag{3.4}
$$

We shall call the quantity (3.3) the information of order $\alpha$ contained in the observation of the event $E$ with respect to the random variable $\xi$ or, for the sake of brevity, the information of order $\alpha$ obtained if the distribution $\mathcal{P}$ is replaced by the distribution $\mathcal{Q}$. We shall give a system of postulates, analogous to the postulates for entropy considered in section 2, which characterize the quantities $I_{\alpha}(\mathcal{Q}|\mathcal{P})$, including the case $\alpha = 1$.

As in the case of entropy, it is advantageous to consider the quantity $I(\mathfrak{Q}|\mathcal{P})$ for generalized probability distributions, not only for complete distributions. We suppose that, associated with any generalized probability distribution $\mathcal{P} = (p_1, p_2, \cdots, p_n)$ such that $p_k > 0$ for $k = 1, 2, \cdots, n$, and any generalized probability distribution  $\mathcal{Q} = (q_{1}, q_{2}, \cdots, q_{n})$  whose terms are given in a one-to-one correspondence with those of P (as determined by their indices), there corresponds a real number  $I(\mathcal{Q}|\mathcal{P})$  which satisfies the following postulates.

POSTULATE 6. $I(\mathbb{Q}|\mathbb{P})$ is unchanged if the elements of $\mathbb{P}$ and $\mathbb{Q}$ are rearranged in the same way so that the one-to-one correspondence between them is not changed.

POSTULATE 7. If $\mathcal{O} = (p_1, p_2, \cdots, p_n)$ and $\mathcal{Q} = (q_1, q_2, \cdots, q_n)$, and $p_k \leq q_k$ for $k = 1, 2, \cdots, n$ then $I(\mathcal{Q}|\mathcal{O}) \geq 0$; while if $p_k \geq q_k$ for $k = 1, 2, \cdots, n$ then $I(\mathcal{Q}|\mathcal{O}) \leq 0$.

POSTULATE 8. $I(\{1\} |\{1 / 2\}) = 1.$

POSTULATE 9. If $I(\mathbb{Q}_1|\mathbb{P}_1)$ and $I(\mathbb{Q}_2|\mathbb{P}_2)$ are defined, and if $\mathbb{P} = \mathbb{P}_1 * \mathbb{P}_2$ and $\mathbb{Q} = \mathbb{Q}_1 * \mathbb{Q}_2$ and the correspondence between the elements of $\mathbb{P}$ and $\mathbb{Q}$ is that induced by the correspondence between the elements of $\mathbb{P}_1$ and $\mathbb{Q}_1$, and those of $\mathbb{P}_2$ and $\mathbb{Q}_2$, then

$$
I (\mathbb {Q} | \mathcal {P}) = I (\mathbb {Q} _ {1} | \mathcal {P} _ {1}) + I (\mathbb {Q} _ {2} | \mathcal {P} _ {2}).\tag{3.5}
$$

POSTULATE 10. There exists a continuous and strictly increasing function $y = g(x)$ defined for all real $x$, such that denoting by $x = g^{-1}(y)$ its inverse function, if $I(\mathbb{Q}_1|\mathbb{P}_1)$ and $I(\mathbb{Q}_2|\mathbb{P}_2)$ are defined, and $0 < w(\mathbb{P}_1) + w(\mathbb{P}_2) \leq 1$ and $0 < w(\mathbb{Q}_1) + w(\mathbb{Q}_2) \leq 1$, and the correspondence between the elements of $\mathbb{P}_1 \cup \mathbb{P}_2$ and $\mathbb{Q}_1 \cup \mathbb{Q}_2$ is that induced by the correspondence between the elements of $\mathbb{P}_1$ and $\mathbb{Q}_1$ and those of $\mathbb{P}_2$ and $\mathbb{Q}_2$, then we have

$$
I (\mathbb {Q} _ {1} \cup \mathbb {Q} _ {2} | \mathcal {P} _ {1} \cup \mathcal {P} _ {2}) = g ^ {- 1} \left\{\frac {w (\mathbb {Q} _ {1}) g [ I (\mathbb {Q} _ {1} | \mathcal {P} _ {1}) ] + w (\mathbb {Q} _ {2}) g [ I (\mathbb {Q} _ {2} | \mathcal {P} _ {2}) ]}{w (\mathbb {Q} _ {1}) + w (\mathbb {Q} _ {2})} \right\}.\tag{3.6}
$$

Let us mention that if $\bar{g}(x) = ag(x) + b$ where $a \neq 0$, then the right side of (3.6) remains unchanged if we replace $g(x)$ by $\bar{g}(x)$. Thus if postulate 10 holds with $g(x)$ it holds also for $\bar{g}(x)$ instead of $g(x)$. We now prove

THEOREM 3. Suppose that the quantity $I(\mathbb{Q}|\mathcal{P})$ satisfies the postulates 6, 7, 8, 9, and 10. Then the function $g(x)$ in 10 is necessarily either a linear or an exponential function. In the first case $I(\mathbb{Q}|\mathcal{P}) = I_1(\mathbb{Q}|\mathcal{P})$, where

$$
I _ {1} (\mathbb {Q} | \mathcal {P}) = \frac {\sum_ {k = 1} ^ {n} q _ {k} \log_ {2} \frac {q _ {k}}{p _ {k}}}{\sum_ {k = 1} ^ {n} q _ {k}},\tag{3.7}
$$

while in the second case $I(\mathbb{Q}|\mathcal{P}) = I_{\alpha}(\mathbb{Q}|\mathcal{P})$ with some $\alpha \neq 1$, where

$$
I _ {\alpha} (\mathcal {Q} | \mathcal {P}) = \frac {1}{\alpha - 1} \log_ {2} \frac {\sum_ {k = 1} ^ {n} \frac {q _ {k} ^ {\alpha}}{p _ {k} ^ {\alpha - 1}}}{\sum_ {k = 1} ^ {n} q _ {k}}.\tag{3.8}
$$

REMARK. If $\mathcal{P}$ and $\mathbb{Q}$ are complete distributions then clearly the formulas (3.7) and (3.8) reduce respectively to the formulas (3.2) and (3.3).

Proof. Let us put

$$
f (q, p) = I (\{q \} | \{p \}),\tag{3.9}
$$

$$
0 <   p \leq 1, \quad 0 <   q \leq 1.
$$

It follows from postulate 9 that

$$
f (q _ {1} q _ {2}, p _ {1} p _ {2}) = f (q _ {1}, p _ {1}) + f (q _ {2}, p _ {2}).\tag{3.10}
$$

Putting $q_{1} = q_{2} = 1$ in (3.10), we get

$$
f (1, p _ {1} p _ {2}) = f (1, p _ {1}) + f (1, p _ {2}),\tag{3.11}
$$

while for $q_{1} = p_{2} = 1$, $p_{1} = p$, $q_{2} = q$ we get from (3.10)

$$
f (q, p) = f (1, p) + f (q, 1).\tag{3.12}
$$

On the other hand, it follows from postulate 7 that $I(\mathcal{P}|\mathcal{P}) = 0$ for any $\mathcal{P}$, and thus

$$
f (1, p) + f (p, 1) = 0.\tag{3.13}
$$

Hence we obtain from (3.12)

$$
f (q, p) = f (1, p) - f (1, q).\tag{3.14}
$$

Now, according to postulate 7, it follows from (3.14) that $f(1, p)$ is a decreasing function of $p$, and by taking postulate 8 into account it follows from (3.11) that

$$
f (1, p) = \log_ {2} {\frac {1}{p}}.\tag{3.15}
$$

Thus from (3.14) we obtain

$$
f (q, p) = I (\{q \} | \{p \}) = \log_ {2} \frac {q}{p}, \quad 0 <   p \leq 1, \quad 0 <   q \leq 1.\tag{3.16}
$$

Using now postulate 10, considering the decompositions $\mathcal{P} = \{p_1\} \cup \{p_2\} \cup \cdots \cup \{p_n\}$ and $\mathcal{Q} = \{q_1\} \cup \{q_2\} \cup \cdots \cup \{q_n\}$ and applying induction we obtain

$$
I (\mathbb {Q} | \mathcal {P}) = g ^ {- 1} \left[ \frac {\sum_ {k = 1} ^ {n} q _ {k} g \left(\log_ {2} \frac {q _ {k}}{p _ {k}}\right)}{\sum_ {k = 1} ^ {n} \zeta_ {k}} \right].\tag{3.17}
$$

Now let us consider what possible choices of the function $g(x)$ are compatible with postulate 9. It follows from postulate 9 that for any $\lambda \geq 0$ and $\mu \geq 0$ we have

$$
I (\mathcal {Q} * \{e ^ {- \lambda} \} | \mathcal {P} * \{e ^ {- \mu} \}) = I (\mathcal {Q} | \mathcal {P}) + \mu - \lambda .\tag{3.18}
$$

Thus, putting $\mu -\lambda = y$, we see that for an arbitrary real $y$ we have

$$
g ^ {- 1} \left[ \frac {\sum_ {k = 1} ^ {n} q _ {k} g \left(\log_ {2} \frac {q _ {k}}{p _ {k}} + y\right)}{\sum_ {k = 1} ^ {n} q _ {k}} \right] = g ^ {- 1} \left[ \frac {\sum_ {k = 1} ^ {n} q _ {k} g \left(\log_ {2} \frac {q _ {k}}{p _ {k}}\right)}{\sum_ {k = 1} ^ {n} q _ {k}} \right] + y.\tag{3.19}
$$

Now if $w_1, w_2, \cdots, w_n$ is any sequence of positive numbers such that $\sum_{k=1}^{n} w_k = 1$ and $x_1, x_2, \cdots, x_n$ is any sequence of real numbers, we may choose the generalized distributions $\mathcal{P}$ and $\mathcal{Q}$ in such a way that

$$
\frac {q _ {k}}{\sum_ {k = 1} ^ {n} q _ {k}} = w _ {\varepsilon} \quad \text {and} \quad \log_ {2} \frac {q _ {k}}{p _ {k}} = x _ {k}, \quad k = 1, 2, \dots , n.\tag{3.20}
$$

As a matter of fact, we can choose $q_{k} = \rho w_{k}$ and $p_{k} = \rho w_{k} 2^{-x_{k}}$ for $k = 1, 2, \cdots, n$, where $\rho > 0$ is so small that $\sum_{k=1}^{n} p_{k} \leq 1$ and $\sum_{k=1}^{n} q_{k} \leq 1$. Thus we obtain from (3.19) the result that for any such sequences $w_{k}$ and $x_{k}$ and for any real $y$ we have

$$
g ^ {- 1} \bigg [ \sum_ {k = 1} ^ {n} w _ {k} g (x _ {k} + y) \bigg ] = g ^ {- 1} \bigg [ \sum_ {k = 1} ^ {n} w _ {k} g (x _ {k}) \bigg ] + y.\tag{3.21}
$$

Now (3.21) can be expressed in the following form. If

$$
g _ {y} (x) = g (x + y),\tag{3.22}
$$

then we have

$$
g _ {y} ^ {- 1} \left[ \sum_ {k = 1} ^ {n} w _ {k} g _ {y} (x _ {k}) \right] = g ^ {- 1} \left[ \sum_ {k = 1} ^ {n} w _ {k} g (x _ {k}) \right].\tag{3.23}
$$

That is, the functions  $g(x)$  and  $g_{y}(x)$  generate the same mean value. According to a theorem of the theory of mean values (see theorem 83 in [7]) this is possible only if  $g_{y}(x)$  is a linear function of  $g(x)$, that is, if there exist constants  $a(y) \neq 0$  and  $b(y)$  such that

$$
g _ {y} (x) = g (x + y) = a (y) g (x) + b (y).\tag{3.24}
$$

Without restricting the generality we may suppose $g(0) = 0$. Thus we obtain $b(y) = g(y)$, that is,

$$
g (x + y) = a (y) g (x) + g (y).\tag{3.25}
$$

But (3.25) is true for any $x$ and $y$. Thus we may interchange the roles of $x$ and $y$ and we get

$$
g (x + y) = a (x) g (y) + g (x).\tag{3.26}
$$

Thus if $x \neq 0$ and $y \neq 0$ we obtain, comparing (3.25) and (3.26),

$$
\frac {a (y) - 1}{g (y)} = \frac {a (x) - 1}{g (x)}.\tag{3.27}
$$

It follows from (3.27) that there exists a constant $k$ such that

$$
a (x) - 1 = k g (x)\tag{3.28}
$$

for all real $x$. Now we have to distinguish two cases. If $k = 0$ then $a(x) \equiv 1$ and thus by (3.25) we obtain for $g(x)$ the functional equation

$$
g (x + y) = g (x) + g (y)\tag{3.29}
$$

for any real $x$ and $y$. As $g(x)$ is by supposition monotonic it follows that $g(x) = cx$ where $c \neq 0$ is a constant. In this case we see from (3.17) that $I(\mathbb{Q}|\mathcal{P}) = I_1(\mathbb{Q}|\mathcal{P})$, where $I_1(\mathbb{Q}|\mathcal{P})$ is defined by (3.7). In the second case, when $k \neq 0$, the substitution of (3.28) into (3.25) yields

$$
a (x + y) = a (x) a (y)\tag{3.30}
$$

for any real $x$ and $y$. Now (3.28) shows that $a(x)$ is monotonic and hence it follows that $a(x)$ is an exponential function, and so it can be written in the form

$$
a (x) = c 2 ^ {(\alpha - 1) x},\tag{3.31}
$$

where $\alpha \neq 1$ and $c\neq 0$ are constants. It follows from (3.28) that

$$
g (x) = \frac {c 2 ^ {(\alpha - 1) x} - 1}{k}.\tag{3.32}
$$

Substituting (3.32) into (3.17) we obtain the result that $I(\mathbb{Q}|\mathcal{P}) = I_{\alpha}(\mathbb{Q}|\mathcal{P})$, where $I_{\alpha}(\mathbb{Q}|\mathcal{P})$ is defined by (3.8). Thus theorem 3 is proved. (The last part of the proof is essentially identical with the proof of theorem 84 of [7].)

Notice that our postulates do not demand that $I(\mathbb{Q}|\mathcal{P})$ should be a continuous function of the variables $p_k, q_k$ for $k = 1, 2, \dots, n$. Instead of continuity we have postulated a certain sort of monotony by means of postulate 7. This is the reason why the quantities $I_\alpha(\mathbb{Q}|\mathcal{P})$ with $\alpha \leq 0$ are not excluded by the postulates. However $I_\alpha(\mathbb{Q}|\mathcal{P})$ can be considered to be a reasonable measure of information only if $\alpha > 0$. Thus to exclude the quantities $I_\alpha(\mathbb{Q}|\mathcal{P})$ with $\alpha \leq 0$ we have to add a postulate of continuity. For instance, we may add

POSTULATE 11. $\lim_{\epsilon \to +0}[(p,\epsilon)|(p,p)] = 0$ for some $p$ with $0 < p < 1/2$.

Clearly postulates 6 through 11 characterize the quantities $I_{\alpha}(\mathbb{Q}|\mathcal{P})$ with $\alpha >0$.

It remains to characterize $I_1(\mathbb{Q}|\mathcal{P})$ instead of all $I_{\alpha}(\mathbb{Q}|\mathcal{P})$. Of course this can be done by replacing postulate 10 by another postulate which demands that $I(\mathbb{Q}_1 \cup \mathbb{Q}_2|\mathcal{P}_1 \cup \mathcal{P}_2)$ be the weighted arithmetic mean of $I(\mathbb{Q}_1|\mathcal{P}_1)$ and $I(\mathbb{Q}_2|\mathcal{P}_2)$, that is, by

POSTULATE $10'$. If $I(\mathfrak{Q}_1|\mathfrak{P}_1)$ and $I(\mathfrak{Q}_2|\mathfrak{P}_2)$ are defined, and $w(\mathfrak{P}_1) + w(\mathfrak{P}_2) \leq 1$ and $w(\mathfrak{Q}_1) + w(\mathfrak{Q}_2) \leq 1$, and if the correspondence between the elements of $\mathfrak{P}_1 \cup \mathfrak{P}_2$ and $\mathfrak{Q}_1 \cup \mathfrak{Q}_2$ is that induced by the correspondence between the elements of $\mathfrak{P}_1[P_2]$ and $\mathfrak{Q}_1[\mathfrak{Q}_2]$, then we have

$$
I (\mathbb {Q} _ {1} \cup \mathbb {Q} _ {2} | \mathcal {P} _ {1} \cup \mathcal {P} _ {2}) = \frac {w (\mathbb {Q} _ {1}) I (\mathbb {Q} _ {1} | \mathcal {P} _ {1}) + w (\mathbb {Q} _ {2}) I (\mathbb {Q} _ {2} | \mathcal {P} _ {2})}{w (\mathbb {Q} _ {1}) + w (\mathbb {Q} _ {2})}.\tag{3.33}
$$

The proof of theorem 3 contains the proof of

THEOREM 4. If $I(\mathbb{Q}|\mathcal{P})$ satisfies postulates 6, 7, 8, 9, and $10'$, then $I(\mathbb{Q}|\mathcal{P}) = I_1(\mathbb{Q}|\mathcal{P})$, where $I_1(\mathbb{Q}|\mathcal{P})$ is defined by (3.7).

Another way of characterizing $I_1(\mathbb{Q}|\mathcal{P})$ is to retain postulate 10 but add

POSTULATE 12. If $\mathcal{P} = (p_1, p_2, \cdots, p_n)$, $\mathcal{Q} = (q_1, q_2, \cdots, q_n)$, and $\mathfrak{R} = (r_1, r_2, \cdots, r_n)$ are generalized distributions such that

$$
\frac {r _ {k}}{q _ {k}} = \frac {q _ {k}}{p _ {k}},\tag{3.34}
$$

$$
k = 1, 2, \dots , n,
$$

then we have

$$
I (\mathbb {Q} | \mathcal {P}) + I (\mathbb {Q} | R) = 0.\tag{3.35}
$$

It is easy to see that only $I(\mathbb{Q}|\mathcal{P}) = I_1(\mathbb{Q}|\mathcal{P})$ satisfies postulates 6, 7, 8, 9, 10, and 12.

## 4. Information-theoretical proof of a limit theorem on Markov chains

The idea of using measures of information to prove limit theorems of probability theory is due to Linnik [9]. In this section we shall show how this method works in a very simple case.

Let us consider a stationary Markov chain with a finite number of states. Let  $p_{jk}$  for  $j, k = 1, 2, \cdots, N$  denote the transition probability in one step and  $p_{jk}^{(n)}$  the transition probability in n steps from state j to state k. We restrict ourselves to the simplest case when all transition probabilities  $p_{jk}$  are positive. In this case, as is well known, we have

$$
\lim _ {n \to + \infty} p _ {j k} ^ {(n)} = p _ {k}, \quad j, k = 1, 2, \dots , N,\tag{4.1}
$$

where the limits $p_k$ are all positive and satisfy the equations

$$
\sum_ {j = 1} ^ {N} p _ {j} p _ {j k} = p _ {k}, \quad k = 1, 2, \dots , N,\tag{4.2}
$$

and

$$
\sum_ {k = 1} ^ {N} p _ {k} = 1.\tag{4.3}
$$

Our aim is to give a new proof of (4.1) by the use of the measure of information $I_1(\mathbb{Q}|\varphi)$. The fact that the system of equations (4.2) and (4.3) has a solution $(p_1, p_2, \cdots, p_N)$ consisting of positive numbers can be deduced by a well-known theorem of matrix theory. In proving (4.1) we shall take it for granted that such numbers $p_k$ exist. Let us put $\varphi = (p_1, p_2, \cdots, p_N)$ and $\varphi_j^{(n)} = (p_{j1}^{(n)}, p_{j2}^{(n)}, \cdots, p_{jN}^{(n)})$ and consider the amounts of information

$$
I _ {1} (\mathcal {P} _ {j} ^ {(n)} | \mathcal {P}) = \sum_ {k = 1} ^ {N} p _ {j k} ^ {(n)} \log_ {2} \frac {p _ {j k} ^ {(n)}}{p _ {k}}.\tag{4.4}
$$

According to the definition of transition probabilities, we have

$$
p _ {j k} ^ {(n + 1)} = \sum_ {l = 1} ^ {N} p _ {j l} ^ {(n)} p _ {l k}.\tag{4.5}
$$

Now let us introduce the notation

$$
\pi_ {l k} = \frac {p _ {l} p _ {l k}}{p _ {k}}.\tag{4.6}
$$

The probabilistic meaning of the numbers  $\pi_{lk}$  is clear:  $\pi_{lk}$  is the conditional probability for the chain's being in state l, under the condition that at the next step it will be in state k, provided that the initial distribution is the stationary distribution given by the numbers  $p_{1}, p_{2}, \cdots, p_{N}$ . The conditional probabilities  $\pi_{lk}$  are often called the “backward” transition probabilities of the Markov chain. Now we have clearly  $\sum_{l=1}^{N} \pi_{lk} = 1$  for  $k = 1, 2, \cdots, N$  and by (4.5)

$$
I _ {1} (\mathcal {P} _ {j} ^ {(n + 1)} | \mathcal {P}) = \sum_ {k = 1} ^ {N} p _ {k} \left[ \sum_ {l = 1} ^ {N} \pi_ {l k} \left(\frac {p _ {j l} ^ {(n)}}{p _ {l}}\right) \right] \log_ {2} \left[ \sum_ {l = 1} ^ {N} \pi_ {l k} \left(\frac {p _ {j l} ^ {(n)}}{p _ {l}}\right) \right].\tag{4.7}
$$

Applying Jensen's inequality [7] to the convex function $x \log_2 x$, for each value of $k$, we obtain from (4.7)

$$
I _ {1} (\mathcal {P} _ {j} ^ {(n + 1)} | \mathcal {P}) \leq \sum_ {k = 1} ^ {N} p _ {k} \sum_ {l = 1} ^ {N} \pi_ {l k} \frac {p _ {j l} ^ {(n)}}{p _ {l}} \log_ {2} \frac {p _ {j l} ^ {(n)}}{p _ {l}}.\tag{4.8}
$$

Taking into account the fact that

$$
\sum_ {k = 1} ^ {N} p _ {k} \pi_ {l k} = p _ {l},\tag{4.9}
$$

it follows from (4.8) that

$$
I _ {1} (\mathcal {G} _ {j} ^ {(n + 1)} | \mathcal {P}) \leq I _ {1} (\mathcal {G} _ {j} ^ {(n)} | \mathcal {P}).\tag{4.10}
$$

Thus the sequence $I_{1}(\mathcal{G}_{j}^{(n)}|\mathcal{P})$ is decreasing, and as $I_{1}(\mathcal{G}_{j}^{(n)}|\mathcal{P}) \geq 0$, the limit

$$
L = \lim _ {n \to + \infty} I _ {1} (\mathcal {P} _ {j} ^ {(n)} | \mathcal {P})\tag{4.11}
$$

exists. We shall show now that L = 0 and simultaneously that (4.1) holds. As the number of states is finite, we can find a sequence  $n_{1} < n_{2} < \cdots < n_{s} < \cdots$  of positive integers, such that the limits

$$
\lim _ {s \to + \infty} p _ {j k} ^ {(n _ {s})} = q _ {j k},\tag{4.12}
$$

$$
k = 1, 2, \dots , N,
$$

exist. As $\sum_{k=1}^{N} p_{jk}^{(n)} = 1$, we have evidently

$$
\sum_ {k = 1} ^ {N} q _ {j k} = 1.\tag{4.13}
$$

Let us put further

$$
q _ {j k} ^ {\prime} = \sum_ {l = 1} ^ {N} q _ {j l} p _ {l k},\tag{4.14}
$$

$$
k = 1, 2, \dots , N,
$$

and put for the sake of brevity  $\mathfrak{Q}_{j} = (q_{j1}, q_{j2}, \cdots, q_{jN})$  and  $\mathfrak{Q}_{j}' = (q_{j1}', q_{j2}', \cdots, q_{jN}')$ . Clearly we have

$$
\lim _ {s \to + \infty} I _ {1} (\mathcal {P} _ {j} ^ {(n _ {*})} | \mathcal {P}) = I _ {1} (\mathfrak {Q} _ {j} | \mathcal {P}) = L\tag{4.15}
$$

and

$$
\lim _ {s \rightarrow + \infty} I _ {1} \left(\varphi_ {j} ^ {\left(n _ {s} + 1\right)} \mid \varphi\right) = I _ {1} \left(\mathfrak {Q} _ {j} ^ {\prime} \mid \varphi\right) = L.\tag{4.16}
$$

Again using Jensen's inequality, exactly as in proving (4.10), we have

$$
I _ {1} \left(\mathbb {Q} _ {j} ^ {\prime} \mid \mathcal {P}\right) = \sum_ {l = 1} ^ {N} p _ {k} \left[ \sum_ {l = 1} ^ {N} \pi_ {l k} \left(\frac {q _ {j l}}{p _ {l}}\right) \right] \log_ {2} \left[ \sum_ {l = 1} ^ {N} \pi_ {l k} \left(\frac {q _ {j l}}{p _ {l}}\right) \right] \leq I _ {1} \left(\mathbb {Q} _ {j} \mid \mathcal {P}\right)\tag{4.17}
$$

with equality holding in (4.17) only if  $q_{l}/p_{l}=c$  for  $l=1,2,\cdots,N$ , where c is a constant. But by (4.16) it follows that there is equality in (4.17), and thus we have

$$
q _ {j l} = c p _ {l},\tag{4.18}
$$

$$
l = 1, 2, \dots , N.
$$

Notice that here we have made essential use of the supposition that all $p_{jk}$ and thus all $\pi_{lk}$ are positive. In view of (4.3) and (4.13) the constant $c$ in (4.18) is equal to 1, and therefore $\mathfrak{Q}_j = \mathcal{P}$. It follows from (4.15) that

$$
L = I _ {1} (\mathcal {P} ^ {\prime} \mathcal {P}) = 0.\tag{4.19}
$$

We have incidentally proved that (4.1) holds, as we have shown that if for an arbitrary subsequence $n_s$ we have (4.12) then necessarily $q_{jl} = p_l$ for $l = 1, 2, \cdots, N$. But if (4.1) were false, we could find a subsequence $n_s$ of integers such that (4.12) holds with $q_{jl} \neq p_l$.

It is clear from the above proof that instead of the quantities (4.4) we could have used the analogous sums

$$
\sum p _ {j k} ^ {(n)} f \left(\frac {p _ {j k} ^ {(n)}}{p _ {k}}\right),\tag{4.20}
$$

where $f(x)$ is any function such that $xf(x)$ is strictly convex. Thus for instance we could have taken $f(x) = x^{\alpha - 1}$ with $\alpha > 1$ or $f(x) = -x^{\alpha - 1}$ with $0 < \alpha < 1$. This means that instead of the measure of information of the first order, we could have used the measure of information of any order $\alpha > 0$, and deduce (4.1) from the fact that $\lim_{n \to +\infty} I_{\alpha}(\mathcal{P}_j^{(n)}|\mathcal{P}) = 0$.

In proving limit theorems of probability theory by considering measures of information, it is usually an advantage that one can choose between different measures. In the above simple case each measure $I_{\alpha}(\mathbb{Q}|\mathcal{P})$ was equally suitable, but in other cases the quantity $I_{2}(\mathbb{Q}|\mathcal{P})$, for example, is more easily dealt with than the quantity $I_{1}(\mathbb{Q}|\mathcal{P})$. The author intends to return to this question, by giving a simplified version of Linnik's information-theoretical proof of the central limit theorem, in another paper.

## REFERENCES

[1] C. E. SHANNON and W. WEAVER, The Mathematical Theory of Communication, Urbana, University of Illinois Press, 1949.

[2] D. K. FADEEV, “Zum Begriff der Entropie einer endlichen Wahrscheinlichkeitsschemas,” Arbeiten zur Informationstheorie I, Berlin, Deutscher Verlag der Wissenschaften, 1957, pp. 85–90.

[3] A. FEINSTEIN, Foundations of Information Theory, New York, McGraw-Hill, 1958.

[4] P. Erdős, “On the distribution function of additive functions,” Ann. of Math., Vol. 47 (1946), pp. 1–20.

[5] A. RÉNYI, “On a theorem of Erdős and its application in information theory,” Mathematica, Vol. 1 (1959), pp. 341–344.

[6] G. A. BARNARD, “The theory of information,” J. Roy. Statist. Soc., Ser. B, Vol. 13 (1951), pp. 46–64.

[7] G. H. HARDY, J. E. LITTLEWOOD, and G. PÓLYA, Inequalities, Cambridge, Cambridge University Press, 1934.

[8] S. KULLBACK, Information Theory and Statistics, New York, Wiley, 1959.

[9] YU. V. LINNIK, “An information theoretical proof of the central limit theorem on Lindeberg conditions,” Teor. Veroyatnost. i Primenen., Vol. 4 (1959), pp. 311–321. (In Russian.)