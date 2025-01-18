---
{"dg-publish":true,"permalink":"/Studies/Maths/Taylor series expansions/"}
---

$$
\begin{flalign}

f(x) &= f(a) + \dfrac{f'(a)}{1!}(x-a) + \dfrac{f''(a)}{2!}(x-a)^{2} + \dfrac{f'''(a)}{3!}(x-a)^{3} + \dots &
\\
&= \sum _{n=0}^{\infty }\dfrac{f^{(n)}(a)}{n!}(x-a)^{n}
\\
f(x) &= f(0) + \dfrac{f'(0)}{1!}x + \dfrac{f''(0)}{2!}x^2 + \dots + \dfrac{f^{(n)}(0)}{n!}x^n
\\
&= \displaystyle \sum_{k=0}^{n} \dfrac{f^{(k)}}{n!}x^n

\end{flalign}
$$

# Trigonometry

$$
\begin{flalign}

\sin(x) &= x - \dfrac{x^3}{3!} + \dfrac{x^5}{5!} - \dfrac{x^7}{7!} + \dots &
\\
&= \sum_{n=0}^{\infty} \dfrac{(-1)^n x^{2n+1}}{(2n+1)!}
\\
\cos(x) &= 1 - \dfrac{x^2}{2!} + \dfrac{x^4}{4!} - \dfrac{x^6}{6!} + \dots
\\
&=  \sum_{n=0}^{\infty} \dfrac{(-1)^n x^{2n}}{(2n)!}
\\
\tan(x) &= x + \dfrac{x^3}{3} + \dfrac{2x^5}{15} + \dots
\\
&= \sum_{n=0}^{\infty} a_n x^{2n+1}
\\
\cot(x) &=  \dfrac{1}{x} - \dfrac{x}{3} + \dfrac{x^3}{45} - \dfrac{2x^5}{945} - \dots
\\
&= \sum_{n=0}^{\infty} (-1)^n \dfrac{B_{2n} (2x)^{2n-1}}{(2n)!} & |x| < \pi
\\
\\
\arcsin x &= x + \dfrac{x^3}{6} + \dfrac{3x^5}{40} + \dots
\\
&=  \sum_{n=0}^{\infty} \dfrac{(2n)!}{2^{2n}(n!)^2(2n+1)} x^{2n+1} & |x| \leq 1
\\
\arccos(x) &= \dfrac{\pi}{2} - x - \dfrac{x^3}{6} - \dots
\\
&= \dfrac{\pi}{2} - \sum_{n=0}^{\infty} \dfrac{(2n)!}{2^{2n}(n!)^2(2n+1)} x^{2n} & |x| < 1
\\
\arctan(x) &= x - \dfrac{x^3}{3} + \dfrac{x^5}{5} - \dots
\\
&= \sum_{n=0}^{\infty} (-1)^n \dfrac{x^{2n+1}}{2n+1} & |x| < 1
\\
\operatorname{arccot}(x) &= 1 - \dfrac{x^2}{3} + \dfrac{x^4}{5} - \dots
\\
&= \sum_{n=0}^{\infty} (-1)^n \dfrac{x^{2n}}{2n+1} & |x| < 1

\end{flalign}
$$

# Power

$$
\begin{flalign}

e^x &= 1 + x + \dfrac{x^2}{2!} + \dfrac{x^3}{3!} + \dfrac{x^4}{4!} + \dots &
\\
&=  \sum_{n=0}^{\infty} \dfrac{x^n}{n!}
\\
\ln(1+x) &= x - \dfrac{x^2}{2} + \dfrac{x^3}{3} - \dfrac{x^4}{4} + \dots
\\
&= \sum_{n=1}^{\infty} (-1)^{n-1} \dfrac{x^n}{n}, \quad (-1 < x \leq 1)
\\
\ln(1-x) &= -\left(x + \dfrac{x^2}{2} + \dfrac{x^3}{3} + \dots\right)
\\
&= -\sum_{n=1}^{\infty} \dfrac{x^n}{n} & |x| < 1
\\
(1+x)^n &= 1 + nx + \dfrac{n(n-1)}{2!}x^2 + \dfrac{n(n-1)(n-2)}{3!}x^3 + \dots
\\
&= \sum_{k=0}^{\infty} \binom{n}{k} x^k & |x| < 1
\\
\sqrt{1+x} &= 1 + \dfrac{x}{2} - \dfrac{x^2}{8} + \dfrac{3x^3}{16} - \dots
\\
&= \sum_{n=0}^{\infty} \binom{\tfrac{1}{2}}{n} x^n & |x| < 1

\end{flalign}
$$

# Geometric

$$
\begin{flalign}

\dfrac{1}{1-x} &= 1 + x + x^2 + x^3 + x^4 + \dots &
\\
&= \sum_{n=0}^{\infty} x^n & |x| < 1
\\
\dfrac{1}{1+x} &= 1 - x + x^2 - x^3 + x^4 - \dots
\\
&= \sum_{n=0}^{\infty} (-1)^n x^n & |x| < 1

\end{flalign}
$$