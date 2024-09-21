---
{"dg-publish":true,"permalink":"/Studies/University/Year 1/MI1111 - Calculus I/Day 02.2/"}
---

Hàm ngược: $y = f(x) \Longrightarrow x = g(y) \Longrightarrow$ Hàm ngược $y = g(x)$
VD:

$$
\begin{flalign}

&y = f(x) = x + e^x &
\\
&\Rightarrow f^{-1}(1) = a
\\
&\Rightarrow f(a) = 1
\\
&\Rightarrow a + e^a = 1
\\
&\Rightarrow e^a = 1-a
\\
&VT \nearrow, VP \searrow 
\\
&\Rightarrow a = 0 \text{ có nghiệm duy nhất}
\\
&\Rightarrow f^{-1}(1) = 0

\end{flalign}
$$

## 1.5. Giới hạn hàm số. Hai định nghĩa tương đương. Các phép toán và tính chất. Giới hạn của hàm hợp. Giới hạn 1 phía. Giới hạn ở vô cực 
### Định nghĩa điểm tụ
- $x_0$ được gọi là điểm tụ của $x$ nếu $\forall U_{\epsilon}(x_0) \setminus \{ x_0 \} \cap X \neq \varnothing$
- $U_{\epsilon} = \{ x \ | \ x_0 - \epsilon < x < x_0 + \epsilon \}$ 
### Định nghĩa giới hạn của hàm số
- Cho $x_0$ là điểm tụ của $D$, $f : D \subset \mathbb{R} \longmapsto \mathbb{R}$. Ta nói $f(x)$ có giới hạn là $a$ khi $x$ tiến tới $x_0$, viết $\displaystyle \lim_{x \to x_0} f(x) = a$ 
- $\Leftrightarrow \forall \epsilon > 0$ bé tuỳ ý, $\exists \delta(\epsilon)$ sao cho $|x - x_0| < \delta$ thì $|f(x) - a| < \epsilon$ 
### Định nghĩa giới hạn của hàm số theo dãy
- $\displaystyle \lim_{x \to x_0} f(x) = a \Leftrightarrow \forall \text{dãy } x_{n} \rightarrow x_0$ thì $f(x_{n}) \rightarrow a$, $n \rightarrow \infty$, $x \rightarrow x_0$
- Chú ý:
	- Hai định nghĩa trên là tương đương
	- Định nghĩa giới hạn hàm số theo dãy thường sử dụng bằng cách chọn 2 dãy $\overline{x_n}$ và $\widetilde{x_n}$ sao cho $\left\{\begin{array}{l} \overline{x_n} = x_0 \\ \widetilde{x_n} = x_0 \end{array}\right.$
- VD: Tìm $\displaystyle \lim_{x \to 0} \sin\frac{1}{x}$ 

$$
\begin{flalign}

& \text{Chọn} \quad

\begin{array}{l}

\overline{x_n} = \quad\quad \dfrac{1}{2n\pi}
&\text{ có }
\displaystyle \lim_{n \to 0} \overline{x_n} = 0
&\Rightarrow \displaystyle \lim_{n \to 0} \sin(\quad\quad 2n\pi) &= 0

\\

\widetilde{x_n} = \dfrac{1}{\dfrac{\pi}{2} + 2n\pi} 
&\text{ có }
\displaystyle \lim_{n \to 0} \widetilde{x_n} = 0
&\Rightarrow \displaystyle \lim_{n \to 0} \sin(\dfrac{\pi}{2} + 2n\pi) &= 1

\end{array} &

\end{flalign}
$$

### Giới hạn vô cực
- $\displaystyle \lim_{x \to x_0} f(x) = \infty \Leftrightarrow \forall \epsilon > 0, \exists k > 0 : |x - x_0| < \epsilon$ thì  $|f(x)| > k$
- $\displaystyle \lim_{x \to \infty} f(x) = a \Leftrightarrow \forall N > 0, \exists \delta > 0 : |x_n| > N$ thì  $|f(x) - a| < \delta$
- $\displaystyle \lim_{x \to \infty} f(x) = \infty \Leftrightarrow \forall k > 0, \exists N > 0 : |x_n| > N$ thì  $|f(x)| > k$
### Tính chất về phép toán
- Giới hạn nếu tồn tại thì là duy nhất
- $f(x) \leq g(x)$ và $\displaystyle \lim_{x \to x_0} f(x) = L_1$, $\displaystyle \lim_{x \to x_0} g(x) = L_2$ $\Rightarrow L_1 < L_2$
### Phép toán
- Nếu  $\displaystyle \lim_{x \to x_0} f(x) = a$, $\displaystyle \lim_{x \to x_0} g(x) = b$ thì $\displaystyle \lim_{x \to x_0} f(x) \odot g(x) = a \odot b$
### Giới hạn của hàm hợp
- Nếu $\displaystyle \lim_{x \to x_0} u(x) = u_o$, $\displaystyle \lim_{x \to u_0} f(x) = a$ $\Rightarrow$ $\displaystyle \lim_{x \to x_0} f(x) = a$
### Giới hạn 1 phía
- $x \rightarrow x^{-}_0$ nghĩa là $\left\{\begin{array}{l} x \rightarrow x_0 \\ x < x_0 \end{array}\right.$ 
- $x \rightarrow x^{+}_0$ nghĩa là $\left\{\begin{array}{l} x \rightarrow x_0 \\ x > x_0 \end{array}\right.$ 
- $x \rightarrow x^{-}_0$ nghĩa là $\left\{\begin{array}{l} x \rightarrow x_0 \\ x < x_0 \end{array}\right.$ 
- Giới hạn trái: $\displaystyle \lim_{x \to x^{-}_0} f(x) = a$  $\Leftrightarrow$ $\forall \epsilon > 0, \exists \delta > 0 : 0 < x_0 - x < \delta$ thì $|f(x) - a| < 0$
- Giới hạn phải: $\displaystyle \lim_{x \to x^{+}_0} f(x) = a$  $\Leftrightarrow$ $\forall \epsilon > 0, \exists \delta > 0 : 0 < x_0 - x < \delta$ thì $|f(x) - a| < \epsilon$
- Định lí: $\displaystyle \lim_{x \to x_0} f(x) = L$ $\Leftrightarrow$ $\left\{\begin{array}{l} \displaystyle \lim_{x \to x^{-}_0} f(x) = L \\ \displaystyle \lim_{x \to x^{+}_0} f(x) = L \end{array}\right.$
- VD: Tìm $\displaystyle \lim_{x \to 0} f(x) = \dfrac{|x|}{x}$

$$
\begin{flalign}

&f(x) = \dfrac{|x|}{x} =

\left \{
\begin{array}{l}
\dfrac{x}{x} &= 1 &\forall x > 0
\\
\dfrac{-x}{x} &= -1 &\forall x < 0
\end{array}
\right. &

\\

&\displaystyle \lim_{x \to 0^{-}} f(x) = -1
\\
&\displaystyle \lim_{x \to 0^{+}} f(x) = 1
\\
&\Rightarrow \displaystyle \lim_{x \to 0} f(x) \text{ không tồn tại}

\end{flalign}
$$

### Một số dạng giới hạn cơ bản
- $\infty$, $-\infty$ : nhân liên hợp
- $\dfrac{0}{0}$, $\dfrac{\infty}{\infty}$: L'Hospital
- $0 \times \infty$
- $0^0$, $1^\infty$, $\infty^0$

## 1.6. Khái niệm vô cùng bé, vô cùng lớn. So sánh vcb, vcl. Tính chất và quy tắc ngắt bỏ
### Vô cùng bé, vô cùng lớn
- $\alpha(x)$ vcb khi $x \rightarrow x_0 \Leftrightarrow \displaystyle \lim_{x \to x_0} \alpha(x) = 0$
- $\beta(x)$ vcl khi $x \rightarrow x_0 \Leftrightarrow \displaystyle \lim_{x \to x_0} |\beta(x)| = \infty$
### So sánh vcb, vcl
- $\alpha(x)$, $\beta(x)$ vcb khi $x \rightarrow x_0$. Khi đó

$$
\begin{flalign}

\displaystyle \lim_{x \to 0}\dfrac{\alpha(x)}{\beta(x)} = 

\left [
\begin{array}{l}
0, \alpha(x) \text{ là vcb bậc cao hơn } \beta(x)
\\
A, \alpha(x) \text{ và } \beta(x) \text{ cùng bậc với } \alpha(x) \sim \beta(x)
\\
\infty, \alpha(x) \text{ là vcb bậc thấp hơn } \beta(x)
\end{array}
\right. &

\end{flalign}
$$

### Quy tắc bỏ vcb tương đương
- Nếu $\left\{\begin{array}{l} \alpha(x) \sim \alpha_1(x) \\ \beta(x) \sim \beta_1(x) \end{array}\right.$ thì $\displaystyle \lim_{x \to x_0} \dfrac{\alpha(x)}{\beta(x)} = \lim_{x \to x_0} \dfrac{\alpha_1(x)}{\beta_1(x)}$
- Chú ý: có thể thay thế các vcb tương đương bằng phép nhân, chia $\displaystyle \lim_{x \to x_0} \dfrac{\alpha(x)\beta(x)}{\gamma(x)\delta(x)} = \lim_{x \to x_0} \dfrac{\alpha_1(x)\beta_1(x)}{\gamma_1(x)\delta_1(x)}$
### Quy tắc bỏ vcb bậc cao

> [!warning] TBA

## Hàm liên tục. Liên tục 1 phía, liên tục đều. Tính chất. Điểm gián đoạn, phân loại điểm gián đoạn. Hàm liên tục khác
### Định nghĩa hàm liên tục
- $f(x)$ liên tục tại $x_0$ nếu $f(x)$ xác định tại lân cận $x_0$, bao gồm $x_0$, và $\displaystyle \lim_{x \to x_0} f(x) = f(x)$ $\Leftrightarrow$ $\displaystyle \lim_{x \to x^{-}_0} f(x) = \lim_{x \to x^{+}_0} f(x) = f(x)$
- Liên tục trái: $\displaystyle \lim_{x \to x^{-}_0} f(x) = f(x)$
- Liên tục phải: $\displaystyle \lim_{x \to x^{+}_0} f(x) = f(x)$
- Nếu $f(x)$ không liên tục tại $x_0$ thì $x_0$ là điểm gián đoạn $f(x)$
- Các hàm sơ cấp liên tục trên TXĐ
### Phân loại điểm gián đoạn
- Loại 1: $x_0$ là điểm gián đoạn, $\exists \displaystyle \lim_{x \to x^{-}_0} f(x), \lim_{x \to x^{+}_0} f(x)$
	- Loại 1 khử được: $\displaystyle \lim_{x \to x^{-}_0} f(x) = \lim_{x \to x^{+}_0} f(x)$
- Loại 2: còn lại
### Tính chất
- $f(x)$ liên tục trên $[a, b]$ $\Rightarrow$ bị chặn trên $[a, b]$ ($\exists M > 0$ sao cho $|f(x)| \leq M \forall x \in [a, b]$)
- $f(x)$ liên tục trên $[a, b]$, giả sử $\max f(x) = M$, $\min f(x) = N$, $c \in [N, M]$ $\Rightarrow$ $\exists x_0 \in [a, b]$ sao cho $f(x_0) = c$
### Liên tục đều
- $f(x)$, $\forall \epsilon > 0$, $\exists \delta(\epsilon)$ bé tuỳ ý sao cho $\forall x_1, x_2 : |x_1 - x_2| < \delta$ thì $|f(x_1) - f(x_2)| < \epsilon$
- Hàm số liên tục đều thì liên tục
- $f(x)$ liên tục trên $(a, b)$ $\Rightarrow$ liên tục đều trên $(a, b)$
### Liên tục từng khúc
- $f(x)$ liên tục từng khúc trên $[a, b]$ nếu $[a, b]$ được chia thành hữu hạn các đoạn con, và $f(x)$ liên tục trên mỗi đoạn con này