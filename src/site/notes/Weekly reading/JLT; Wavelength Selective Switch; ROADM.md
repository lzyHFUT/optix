---
{"dg-publish":true,"cssclass":"img-grid","permalink":"/Weekly reading/JLT; Wavelength Selective Switch; ROADM/","dgPassFrontmatter":true,"created":"2025-06-22T21:50:01.000+08:00","updated":"2025-04-29T22:52:38.000+08:00"}
---

- Roelens, M. A., Frisken, S., Bolger, J. A., Abakoumov, D., Baxter, G., Poole, S., & Eggleton, B. J. (2008). Dispersion trimming in a reconfigurable wavelength selective switch. _Journal of Lightwave Technology_, _26_(1), 73-78.
# Introduction
**Reconfigurable optical add/drop multiplexers (ROADM) are key network elements that will enable more agile optical transmission systems.**
## What is ROADM?
- **Optical Network:** Data transmission via optical fiber enables higher bandwidths than electrical signals and avoids interference between signals. Lower loss is achieved by using total reflection for transmission through optical fibers[1-2]. 
- **ROADM:** Optical networks match protocols by the parameter of wavelength. Optical signals on a single ray of light are separated into multiple wavelengths by wavelength-division multiplexing (WDM) technology, and different wavelengths represent different communication channels, while reconfigurable optical divide-and-multiplexers(ROADM) are used to manage the signal paths with wavelength-selective functionality, which allows for the addition or removal of specific wavelengths in addition to amplifying and monitoring the signals[3-4].
## How is ROADM implemented?
- **MEMS:** This is achieved by controlling dispersion, which can be achieved through devices such as  MEMS, etc[5].
- **SLM+VIPA**
	- **VIPA:**[6] Virtual Imaging Phased Array is an optical structure in which the angle of the output beam varies with the wavelength, and the return angle of light of different wavelengths is different, which generates a delay, and the relationship between the delay and the wavelength depends on the shape of the mirror C. The desired delay is achieved by designing the mirror shape C.
	- The shape of the mirror is $c(y)=\frac{K}{8f^4}y^4+\frac{{K\Theta}}{2f^3}y^3+\frac{{K\Theta^2-(f-a)}}{2f^2}y^2$, and the slope of the graph can be represented by $-\frac{2n^4K}{c\lambda}$. The final system is designed to be regulated by adding a grating diffraction, where different wavelengths arrive at different positions after diffraction, and different positions have different shapes.
	- **SLM:** [7]First use VIPA to spectralize according to the wavelength, then use SLM to adjust the reflection angle.

![|350](https://i.imgur.com/9Jgskqi.png)![|350](https://i.imgur.com/VMlpwk7.png)

![|325](https://i.imgur.com/SLUoIZR.png) ![|350](https://i.imgur.com/DgN5tlp.png)

![|500](https://i.imgur.com/AYqzs1o.png)
## The solution to this article
Using LCOS as a Wavelength Selection Switch
![|400](https://i.imgur.com/MnnRqXD.png)

# Methods
## What is LCoS?
LCoS is based on liquid crystal materials and utilizes the birefringence of liquid crystal molecules to modulate the polarization state of light for amplitude or phase modulation[13].
### LCoS-Twisted Nematic Configuration
When a voltage is loaded to a pixel and the polarization direction of the incident light is parallel to the direction of the incident polarizer of the LCoS, the liquid crystal molecules rotate under the applied voltage, and the rotation changes the polarization characteristics of the incident light[14].
![c9646184e54a7981f8686dd1e2826b30.gif|450](/img/user/Weekly%20reading/c9646184e54a7981f8686dd1e2826b30.gif)

### LCoS-Zero Twisted Configuration
The phase of light can be regarded as the relative position of light in space[15]. The liquid crystal molecules are deflected after applying a voltage, and the refractive indices of the long and short axes of the liquid crystal molecules are different, resulting in a phase delay[16].
![83fbde62965c86b431ac9ff9db7858f2.gif|475](/img/user/Weekly%20reading/83fbde62965c86b431ac9ff9db7858f2.gif)
**Vertically, the light diverges so that the signal overlaps a large number of pixels (typically about 400).**
Light is fed from the array fiber, polarization separation is performed to maximize the diffraction efficiency [8], using reflection gratings, different light arrives at different positions of the LCOS, dispersion on the arc-vector plane, light recombination on the meridian plane, and the phase delay is controlled by switching the LCOS.
$$\begin{cases}
\tau=\frac{d\phi}{d\omega }=\frac{d\phi}{d\lambda }\frac{d\lambda}{d\omega } \\
\lambda=c \frac{2\pi}{\omega }
\end{cases}\implies \tau=-\frac{\lambda^2}{2\pi c}\frac{d\phi}{dx} \frac{dx}{d\lambda}$$
$D=\frac{d\lambda}{dx}$ is the dispersion on the x-axis of the LCOS. It can be seen that the delay depends on the wavelength and the position of $x$.
# Results
![|330](https://i.imgur.com/1Z7a0mF.png)![|340](https://i.imgur.com/1P69KgG.png)

Obviously, compared with the previous solution using VIPA, it can be more finely controlled.[@shrivastavDesignConsiderationsLimitations2023]
# Discussion
This article is relatively old, most of the solutions have been replaced by digital micromirror devices (DMD), and we can find some reasons for using DMDs instead of LCOS in the related literature [9-11]. Moreover, the application point of this article is only in optical networks, and in fact similar techniques can be applied in more directions such as [11-12].
# Reference
[1]Mukherjee, B., Tomkos, I., Tornatore, M., Winzer, P., & Zhao, Y. (Eds.). (2020). _Springer handbook of optical networks_. Springer Nature.
[2]Ramaswami, R., Sivarajan, K., & Sasaki, G. (2009). _Optical networks: a practical perspective_. Morgan Kaufmann.
[3]N. Networks, “What Is Fibre Optics & How Does It Work?,” 01-Jan-2023. url:https://neosnetworks.com/resources/blog/fibre-optics-what-is-it-and-how-does-it-work/
[4]Richardson, D. J., Fini, J. M., & Nelson, L. E. (2013). Space-division multiplexing in optical fibres. _Nature photonics_, _7_(5), 354-362.
[5]Wu, M. C., Solgaard, O., & Ford, J. E. (2007). Optical MEMS for lightwave communication. _Journal of Lightwave Technology_, _24_(12), 4433-4454.
[6]Shirasaki, M., & Cao, S. (2001, March). Compensation of chromatic dispersion and dispersion slope using a virtually imaged phased array. In _Optical Fiber Communication Conference_ (p. TuS1). Optica Publishing Group.
[7]Lee, G. H., Xiao, S., & Weiner, A. M. (2006). Optical Dispersion Compensator With $≫ $4000-ps/nm Tuning Range Using a Virtually Imaged Phased Array (VIPA) and Spatial Light Modulator (SLM). _IEEE photonics technology letters_, _18_(17), 1819-1821.
[8]“衍射效率·不同偏振光下的衍射效率 | 岛津中国.” https://www.shimadzu.com.cn/optical/guide/diffraction/08.html. 
[9]Gao, Y., Chen, X., Chen, G., Tan, Z., Chen, Q., Dai, D., ... & Yu, C. (2019). Programmable spectral filter in c-band based on digital micromirror device. _Micromachines_, _10_(3), 163.
[10]Faustov, A. R., Webb, M. R., & Walt, D. R. (2010). Note: toward multiple addressable optical trapping. _Review of Scientific Instruments_, _81_(2).
[11]Xue Dong, Xingchen Xiao, Yining Pan, Guangyao Wang, and Yiting Yu, "DMD-based hyperspectral imaging system with tunable spatial and spectral resolution," Opt. Express **27**, 16995-17006 (2019)
[12]Y. Zhang, Y. Fu, Q. Liu, L. Wang, S. Yang, S. Liang, J. Zhang, J. Zhong, B. Zhao, and Y. Meng, “Large dynamic range stellar radiation simulation optical system,” 19-Jan-2024. 
[13]Vettese, D. (2010). Liquid crystal on silicon. _Nature Photonics_, _4_(11), 752-754.
[14]Lazarev, G., Hermerschmidt, A., Krüger, S., & Osten, S. (2012). LCOS spatial light modulators: trends and applications. _Optical Imaging and Metrology: Advanced Technologies_, 1-29.
[15]Michalkiewicz, A., Kujawinska, M., Kozacki, T., Wang, X., & Bos, P. J. (2004, August). Holographic three-dimensional displays with liquid crystal on silicon spatial light modulator. In _Interferometry XII: Techniques and Analysis_ (Vol. 5531, pp. 85-94). SPIE.
[16]Zhang, Z., You, Z., & Chu, D. (2014). Fundamentals of phase-only liquid crystal on silicon (LCOS) devices. _Light: Science & Applications_, _3_(10), e213-e213.