---
{"dg-publish":true,"cssclasses":["img-grid"],"permalink":"/OPTICS/Electromagnetic Theory Part II/","dgPassFrontmatter":true,"created":"2025-06-22T21:39:32.000+08:00","updated":"2025-07-12T15:20:59.662+08:00"}
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
$\vec{S}$ is known as the slope-printing vector and represents the power per unit area across a surface perpendicular to $\vec{S}$.
The direction of energy flow is the direction of wave propagation, and the energy changes so rapidly that it is generally described by a mean value.
![|400](https://i.imgur.com/kcV22X5.png)
$\text{sinc}u$ almost exclusively concentrated in the first few cycles. Now we can calculate the average energy:
$$
\begin{align}
<\cos^2 \omega t>_{T}=<\frac{(e^{i\omega t}+e^{-i\omega t})^2}{4}>_{T}=\frac{1}{2}[1+\text{sinc}\omega T\cos 2\omega T]
\end{align}
$$
![|500](https://i.imgur.com/Dc2beMg.png)
# Irradiance
Irradiance $I$: energy falling on a unit area per unit of time. Obviously we do:
$$
I=<S>_{T}=c\varepsilon_{0}^2|\vec{E}\times \vec{B}|<\cos^2(\vec{k}\cdot \vec{r}-\omega t)=\frac{c^2\varepsilon_{0}}{2}|\vec{E}\times \vec{B}|_{T\gg \tau}=\frac{c\varepsilon_{0}}{2}E_{0}^2
$$
Although substitution is possible based on the relationship between $\vec{E}$ and $\vec{B}$, since the electric field is more efficient at doing work on the charge, we generally use only equations containing $E_{0}$ and make $\vec{E}$ the light field.
$$
\begin{cases}
I=\varepsilon v<E^2>_{T} \\
I=\frac{c\varepsilon_{0}}{2}E_{0}^2
\end{cases}
$$
The energy per unit area of light received or emitted is the radiant flux density or outgoing flux density.
The irradiance of a point light source is inversely proportional to the square of the distance $r$. Defining the stereoscopic angle $\Omega=\iint_{S}\sin \theta d\theta d\varphi$ as  clearly gives:
$$
\frac{E}{S}=\frac{I\Omega t}{4\pi r^2}=\frac{4\pi It}{4\pi r^2}\implies \frac{E}{S} \propto \frac{1}{r^2}
$$
# Photons
Photons are stable, elementary particles with zero mass and no charge. Photons belong to bosons, while electrons belong to fermions, and Einstein believed that the electromagnetic field is quantized and consists of a single photon. Different plane monochromatic waves represent different states of the photon, and the average photon flux can be calculated by the following equation:
$$
\begin{align}
\Phi=\frac{AI}{h\nu_{0}}=\frac{P}{h\nu_{0}}
\end{align}
$$
$\frac{I}{h\nu_{0}}$ is the average photon flux density, $A$ is the monochromatic light cross-section area, $P$ is the laser power.
# Radiation Pressure and Momentum
$$
\begin{align}
&\mathcal{P}=\frac{S(t)}{c}\implies<\mathcal{P}>_{T}=\frac{I}{c} \\
&A\mathcal{P}=\frac{\Delta p}{\Delta t}=\frac{p_{V}c\Delta tA}{\Delta t} \implies p_{V}=\frac{S}{c^2}
\end{align}
$$
$p_{V}$ is the bulk density of electromagnetic momentum.
# Radiation
First of all, consider what kind of electrons radiate, obviously stationary electrons do not excite the magnetic field and do not radiate energy externally. The uniform velocity of the electron, if we change the coordinate system, and the electron together with the movement, and the uniform velocity of the electron is no different, and therefore also does not radiate externally. Therefore, only the non-uniformly moving electrons radiate energy externally.