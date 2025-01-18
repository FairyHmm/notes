---
{"dg-publish":true,"permalink":"/Studies/University/Year 1/MI1111 - Calculus I/Days/Day 13.2/"}
---

- Hàm nhiều biến: ánh xạ $\mathbb{R}^n \longrightarrow \mathbb{R}$
- Giới hạn hàm nhiều biến
	- $M_n(x_n, y_n) \rightarrow M_0(x_0, y_0) \Leftrightarrow \begin{cases} x_n \rightarrow x_0 \\ y_n \rightarrow y_0 \end{cases}$
	- $\displaystyle \lim_{ (x, y) \to (x_0, y_0) } f(x, y) = I$ $\Leftrightarrow$ $\forall \varepsilon > 0, \exists \delta > 0 : \rho\Big( (x, y), (x_0, y_0) \Big) < \delta \Rightarrow |f(x, y) - I| < \varepsilon$ $\Leftrightarrow$ $\forall\, \text{dãy } M_n(x_n, y_n) \rightarrow M_0(x_0, y_0) \text{ thì } \displaystyle \lim_{ n \to \infty } f(M_0) = I$
- Hàm liên tục: $f(x, y)$ liên tục tại $M_0(x_0, y_0) \Leftrightarrow \displaystyle \lim_{ (x, y) \to (x_0, y_0) } = f(x_0, y_0)$ 
- Đạo hàm riêng: $\displaystyle \dfrac{\partial f}{\partial x}(x, y) = f_x'(x, y) = \lim_{ \vartriangle x \to 0 } \dfrac{f(x + \vartriangle x, y) - f(x, y)}{\vartriangle x}$

---
# Chương 3: Hàm số nhiều biến số `.centered`
## 3.2. Đạo hàm riêng và vi phân `.centered`
### Vi phân toàn phần cấp 1
- Vi phân cấp 1: $z = f(x, y) \rightarrow dz = f_x'\ dx + f_y'\ dy = f_x' \vartriangle x + f_y' \vartriangle y$
- Sử dụng vi phân cấp 1 để tính gần đúng
### Hàm hợp:
- $z = f(x, y), \begin{cases} x = x(t) \\ y = y(t) \end{cases}$. $z_t' = \dfrac{dz}{dt} = z_x' x_t' + z_y' y_t' = \dfrac{\partial z}{\partial x} \dfrac{dz}{dt} + \dfrac{\partial z}{\partial y} \dfrac{dy}{dt}$
- $z = f(u), u = u(x, y)$. $z_x' = \dfrac{\partial z}{\partial x} = z_u' u_z' = \dfrac{dz}{du} \dfrac{\partial u}{\partial x}$
- $z = f(u, v), \begin{cases} u = u(x, y) \\ v = v(x, y) \end{cases}$. $z_x' = \dfrac{\partial z}{\partial x} = z_u' u_z' + z_v' v_x' = \dfrac{\partial z}{\partial u} \dfrac{\partial u}{\partial x} + \dfrac{\partial z}{\partial v} \dfrac{\partial v}{\partial x}$
### Hàm ẩn:
- $F(x, y) = 0$ xác định 1 hay nhiều hàm ẩn $y = y(x)$. Khi đó $y_x' = - \dfrac{F_x'}{F_y'}$
- $F(x, y, z) = 0$, xác định 1 hay nhiều hàm ẩn $z = z(x, y)$. $z_x' = - \dfrac{F_x'}{F_z'}$, $z_y' = - \dfrac{F_y'}{F_z'}$
- $\begin{cases} F(x, y, z, u, v) = 0 \\ G(x, y, z, u, v) = 0 \end{cases}$, xác định cặp $\begin{cases} u(x, y, z) \\ v(x, y, z) \end{cases}$. Đặt $D = \dfrac{D(F, G)}{D(u, v)} = \begin{vmatrix} F_u' & F_v' \\ G_u' & G_v' \end{vmatrix} = F_u' G_v' - F_v' G_u'$. $u_x' = -\dfrac{1}{D} \dfrac{D(F, G)}{D(x, u)}$, $v_x' = -\dfrac{1}{D} \dfrac{D(F, G)}{D(u, x)}$
### Đạo hàm riêng và vi phân cấp cao
- $z = f(x, y)$
- ${} f_{xx}'' = f_{x^2}'' = \dfrac{\partial}{\partial x}\left( \dfrac{\partial f}{\partial x} \right) = \dfrac{\partial^2 f}{\partial x^2} {}$
- $f_{xy}'' = \dfrac{\partial}{\partial y}\left( \dfrac{\partial f}{\partial x} \right) = \dfrac{\partial^2 f}{\partial y\ \partial x}$
- Định lí Schwartz: $z = f(x, y)$. $f_{xy}''$, $f_{yx}''$ trong lân cận $M_0{x_0, y_0}$ liên tục tại đó thì $f_{xy}'' = f_{yx}''$

---

#### Câu 7: Cho hàm ẩn $y = y(x)$ xác định bởi $x^3 + y^5 + 6xy - 8 = 0$. Tính $y'(1)$

$$
\begin{flalign}

& F(x, y) = x^3 + y^5 + 6xy - 8 = 0 &
\\
\Rightarrow& y_x' = - \dfrac{F_x'}{F_y'} = \dfrac{3x^2 + 6y}{5y^4 + 6x}
\\
& x = 1 \Rightarrow y^5 + 6y - 7 = 0
\\
\Rightarrow& y_x'(1) = \dfrac{9}{11}

\end{flalign}
$$