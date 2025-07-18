---
{"dg-publish":true,"cssclass":"img-grid","permalink":"/OPTICS/Wave Motion/","dgPassFrontmatter":true,"created":"2025-06-22T21:39:33.000+08:00","updated":"2025-06-22T21:39:33.000+08:00"}
---

# What is WAVES?
According to books on the subject, waves can be thought of as a means of transferring energy[1]or as interactions between particle[2]. We can simply imagine a scenario where a rope is jiggled up and down, and because the two neighboring masses are closely connected, the first mass falls while driving the second mass, and so on, and the motion is gradually transferred to the farther side, a process accompanied by the transfer of energy. Clearly, the wave is a self-sustaining perturbation in the medium, **and we can know that the perturbation moves forward and the medium does not move forward**.
# How to Descirbe?
Obviously, there are two kinds of waves, one is the rope example just given, the displacement of the medium is perpendicular to the direction of motion of the wave, this is a longitudinal wave, light is a longitudinal wave. The other can be imagined as a spring, the direction of motion of the medium is in a straight line with the direction of motion of the wave, which is a transverse wave. Here, we will focus on longitudinal waves.
![|250](https://i.imgur.com/wDtIJG5.png)![|350](https://i.imgur.com/lqP5bai.png)
## One-Dimensional Waves
Taking the previously discussed rope as an example, imagine taking a picture of a desktop at a certain point in time; some part of him should show a specific waveform. This waveform can be described by taking the forward direction of the wave as the x-axis. Obviously, this waveform is related to both the time $t$ and the displacement $x$. If the energy loss in the transfer process is not considered, then this waveform does not change. 
Now we try to describe this functional relationship $\psi=f(x,t)$. Binary variables are always less easy to deal with so we try to fix a value to make the discussion simple, time always passes so we try to fix $x$. Imagine if there is a new coordinate system moving along with this wave, then $\psi$ is only affected by time.
![|325](https://i.imgur.com/TD3K37Z.png)

Clearly we have:
$$\psi=f(x-vt)$$
The symbols reflect the direction of motion. It is important to note here that $\psi$ as a whole represents the wave, not that the function value of a point on $f(x-vt)$ represents the wave, and that the function value represents the position of the prime at $(x,t)$. Obviously different waveforms correspond to different mappings $f$, so we cannot rely on the form $\psi=f(x,t)$ to describe the wave. Considering that both $x$ and $t$ are constants, we try to find the relation between $\psi$, $x$, and $t$. To make the computation easy we can make $x' = x-vt$ and then derive it by chain rule. In fact this is the same idea of fixing one variable as stated before. We have the following treatment:
$$\begin{align}\frac{{\partial \psi}}{\partial x}=\frac{{\partial f}}{\partial x'} \frac{{\partial x'}}{\partial x} &\implies\frac{{\partial^2 \psi}}{\partial x^2}=\frac{{\partial \frac{{\partial f}}{\partial x} }}{\partial x'} \frac{{\partial x'}}{\partial x}=\frac{{\partial^2 f}}{\partial x^2} \\ \frac{{\partial \psi}}{\partial t}=\frac{{\partial f}}{\partial x'} \frac{{\partial x'}}{\partial t} &\implies\frac{{\partial^2 \psi}}{\partial x^2}=\frac{{\partial (-v\frac{{\partial f}}{\partial x} )}}{\partial x'} \frac{{\partial x'}}{\partial t}=v^2 \frac{{\partial^2 f}}{\partial x^2}  \\&\implies \frac{{\partial^2 \psi}}{\partial x^2}=v^2\frac{{\partial^2 \psi}}{\partial x^2}\end{align}$$
From this, we get a way to describe the wave.
## Harmonic Waves
The vibration of a spring can be described by the unit circle, and the sinusoidal waves derived from the unit circle are called harmonics. The unit circle reflects the amplitude and phase of the wave.
And here, since the independent variable in sine $sin x$ is dimensionless and must be in radians or angles, and since $x$ in the fluctuation equation in our previous discussion represents the displacement of the wave, which has units, we must introduce a propagation number, $k$, that converts the displacement to radians or angles. Then we have$\psi(x,t)=A \sin k(x-vt)$
![|275](https://i.imgur.com/64DJUvd.png)

As mentioned earlier, harmonics can be derived from the rotation of a circle, and it is clear that the waveform repeats for every $2\pi$ of rotation, so we can define the range $(0,2\pi)$ to be a wave, and we define the displacement in this time to be the length of the wave, $\lambda$, then we have:
$$\psi(x+\lambda,t)=\psi(x,t)\implies k=\frac{2\pi}{\lambda}$$
In addition we consider the following parameters: the time of the process $\tau$, the speed of rotation of the circle $\omega$, the number of waves in 1 second $\nu$
$$\begin{align}\tau&=\frac{\lambda}{v} \\\omega &=\frac{2\pi}{\tau} \\\nu&=\frac{1}{\tau}\end{align}$$
# Phase and Its Speed
We examine the independent variable $kx-\omega t$ of the harmonics such that $\varphi = kx-\omega t$. It is clear that $\varphi$ is also affected by $x$ and $t$. The significance of this value is the angle between the radius of the circle and the x-axis. Imagine that the parameters of the circle are determined, then the position $x$ of the wave at moment $t$ is also determined and its phase angle is also determined, which explains why $\varphi$ is affected by $x$ and $t$. If initially the radius does not coincide with the x-axis, the action on the wave at this point will always be there, which we call the initial phase $\varphi$. According to the very beginning we said that the perturbation moves forward, the medium does not move forward, and for a point on the perturbation it remains fixed, moving forward with the wave, and therefore its phase-fixed state moves at the same rate as the wave. Of course, we can also arrive at this conclusion by derivation:
$$\begin{align}
\frac{{\partial \varphi}}{{\partial t}}=w ,\frac{{\partial \varphi}}{{\partial x}}=k \\
\implies\left( \frac{{\partial x}}{{\partial t}} \right)_{\varphi}=\frac{\omega }{k}=v
\end{align}$$
The effect of $t$ on $\varphi$ is reflected in $\varphi=\omega t$, and $x$ is reflected in $\varphi=kx$
# Plural Pepresentation
According to Euler's formula, we have:
$$\psi(x,t)=\mathrm{Re}(Ae^{i(kx-\omega t+\varepsilon)})$$
# Plane Wave
Consider such a group of lights, consisting of multiple waves that are parallel to each other and moving in the same direction. We can derive its specific direction from the wavefront, as we said at the beginning, light is a longitudinal wave, and the direction of motion of the medium is perpendicular to the direction of the wave. We connect the resulting surfaces with the same phase on each wave to become the wavefront, which is obviously the surface where the medium is moving, so the direction of the wave is perpendicular to this surface.
![|250](https://i.imgur.com/NQx23R6.png)

Considering again the previous role of $k$ in the case of a one-dimensional wave: to convert $x$ to phase, in fact, we have $kx=\vec{k}\vec{x}$, and $\vec{x}$ is the wave's direction of advancement, so $\vec{k}$ also has the role of indicating the wave's direction of advancement. So here, $\vec{k}$ should be perpendicular to the wavefront, then we have:
$$\begin{align}
&\vec{k}(\vec{r}-\vec{r_{0}})=0\implies k_{x}x+k_{y}y+k_{z}z=k_{x}x_{0}+k_{y}y_{0}+k_{z}z_{0}=a \\
&\implies \psi (\vec{r})=Ae^{i \vec{k} \vec{r}}
\end{align}
$$
![|300](https://i.imgur.com/Wkx31eS.png) ![|350](https://i.imgur.com/A1CNDXW.png)

It can be seen that $k_{x},k_{y},k_{z}$ indicate the direction of propagation.And obviously at this point we have:
$$
\begin{align}
&v^2\frac{{\partial^2 \psi}}{\partial (\vec r)^2}=\frac{{\partial^2 \psi}}{\partial t^2} \\
&\implies v^2\nabla^2 \psi=\frac{{\partial^2 \psi}}{\partial t^2}
\end{align}
$$

# Reference
[1]. 赵凯华. & 赵凯华. 新概念物理教程, 光学. (高等教育出版社, Bei jing, 2004).
[2]. 普通物理学_程守洙江之永.