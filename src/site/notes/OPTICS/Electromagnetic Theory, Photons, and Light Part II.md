---
{"dg-publish":true,"cssclasses":["img-grid"],"permalink":"/OPTICS/Electromagnetic Theory, Photons, and Light Part II/","dgPassFrontmatter":true,"created":"2025-04-28T17:20:59.090+08:00","updated":"2025-04-28T17:33:00.000+08:00"}
---

# Energy and Momentum
To derive the energy density of an electric field using a capacitor, let the area of the pole plate $A$, the capacitance be $C$,the spacing be d, the voltage be $U$, and $C = \frac{{\varepsilon_{0} A}}{d}$. The magnetic field energy density is calculated from the inductance containing the current I. The cross-sectional area is $A$, the length is $l$, and there are $n$ turns wound per unit length, $L=\mu_{0}^2nIA$, $B = \mu_{0}nI$. Then we have:
$$
\begin{align}
&u_{E}=\frac{\frac{1}{2}CU^2}{Ad}=\frac{\frac{1}{2} \frac{{\varepsilon_{0} A}}{d}(Ed)^2}{Ad}\implies u_{E}=\frac{1}{2}\varepsilon_{0} E^2 \\
&u_{B}=\frac{\frac{1}{2}LI^2}{Al}=\frac{1}{2}\mu_{0}^2nIA {\frac{B}{\mu_{0}n}}^2\implies u_{B}=\frac{1}{2\mu_{0}}B^2 \\
&E=cB\implies u_{E}=u_{B} \\
&\implies u=u_{E}+u_{B}=\varepsilon EB=\frac{1}{\mu_{0}}EB
\end{align}
$$
We can further calculate the energy flow of electric and magnetic fields in space, the electromagnetic field flows in space, obviously this process is accompanied by the flow of energy, we can calculate the value of energy per unit volume in space using the energy that passes through the area $A$ during the time interval $t$:
$$
S=\frac{uc\Delta tA}{A\Delta t}\implies S=\frac{1}{\mu_{0}}EB\implies \vec{S}=\frac{1}{\mu_{0}}\vec{E}\times \vec{B}=\frac{1}{\mu_{0}}\vec{E}\times \vec{B}\cos^2(\vec{k}\cdot \vec{r}-\omega t)
$$
The direction of energy flow is the direction of wave propagation, and the energy changes so rapidly that it is generally described by a mean value.
![|400](https://i.imgur.com/kcV22X5.png)
$\text{sinc}u$ almost exclusively concentrated in the first few cycles. Now we can calculate the average energy:
$$
\begin{align}
<\cos^2 \omega t>_{T}=<\frac{(e^{i\omega t}+e^{-i\omega t})^2}{4}>_{T}=\frac{1}{2}[1+\text{sinc}\omega T\cos 2\omega T]
\end{align}
$$
![|500](https://i.imgur.com/Dc2beMg.png)

