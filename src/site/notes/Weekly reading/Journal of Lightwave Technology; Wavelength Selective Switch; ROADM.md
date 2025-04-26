---
{"dg-publish":true,"cssclass":"img-grid","permalink":"/Weekly reading/Journal of Lightwave Technology; Wavelength Selective Switch; ROADM/","dgPassFrontmatter":true,"created":"2025-04-25T22:27:07.540+08:00","updated":"2025-04-26T13:10:28.000+08:00"}
---

- M. A. F. Roelens et al., “Dispersion Trimming in a Reconfigurable Wavelength Selective Switch,” Journal of Lightwave Technology, vol. 26, no. 1, pp. 73–78, Jan. 2008, doi: [10.1109/JLT.2007.912148](https://doi.org/10.1109/JLT.2007.912148).
# Introduction
**Reconfigurable optical add/drop multiplexers (ROADM) are key network elements that will enable more agile optical transmission systems.**
## What is ROADM?
- **Optical Network:** Data transmission via optical fiber enables higher bandwidths than electrical signals and avoids interference between signals. Lower loss is achieved by using total reflection for transmission through optical fibers[1-3]. 
- **ROADM:** Optical networks match protocols by the parameter of wavelength. Optical signals on a single ray of light are separated into multiple wavelengths by wavelength-division multiplexing (WDM) technology, and different wavelengths represent different communication channels, while reconfigurable optical divide-and-multiplexers(ROADM) are used to manage the signal paths with wavelength-selective functionality, which allows for the addition or removal of specific wavelengths in addition to amplifying and monitoring the signals[3-4].
## How is ROADM implemented?
- **MEMS:** This is achieved by controlling dispersion, which can be achieved through devices such as  MEMS, etc[5].
- **SLM+VIPA**
	- **VIPA:**[6] Virtual Imaging Phased Array is an optical structure in which the angle of the output beam varies with the wavelength, and the return angle of light of different wavelengths is different, which generates a delay, and the relationship between the delay and the wavelength depends on the shape of the mirror C. The desired delay is achieved by designing the mirror shape C.
		- ![|425](https://i.imgur.com/9Jgskqi.png)
![|375](https://i.imgur.com/VMlpwk7.png)

- The shape of the mirror is $c(y)=\frac{K}{8f^4}y^4+\frac{{K\Theta}}{2f^3}y^3+\frac{{K\Theta^2-(f-a)}}{2f^2}y^2$, and the slope of the graph can be represented by $-\frac{2n^4K}{c\lambda}$. The final system is designed to be regulated by adding a grating diffraction, where different wavelengths arrive at different positions after diffraction, and different positions have different shapes.
![|350](https://i.imgur.com/SLUoIZR.png)
![|350](https://i.imgur.com/DgN5tlp.png)

- **SLM:** [7]First use VIPA to spectralize according to the wavelength, then use SLM to adjust the reflection angle.
- ![|400](https://i.imgur.com/AYqzs1o.png)
## The solution to this article
Using LCOS as a Wavelength Selection Switch
![|400](https://i.imgur.com/MnnRqXD.png)

# Methods
## What is LCoS?


**Vertically, the light diverges so that the signal overlaps a large number of pixels (typically about 400).**
Light is fed from the array fiber, polarization separation is performed to maximize the diffraction efficiency [8], using reflection gratings, different light arrives at different positions of the LCOS, dispersion on the arc-vector plane, light recombination on the meridian plane, and the phase delay is controlled by switching the LCOS.
$$\begin{cases}
\tau=\frac{d\phi}{d\omega }=\frac{d\phi}{d\lambda }\frac{d\lambda}{d\omega } \\
\lambda=c \frac{2\pi}{\omega }
\end{cases}\implies \tau=-\frac{\lambda^2}{2\pi c}\frac{d\phi}{dx} \frac{dx}{d\lambda}$$
$D=\frac{d\lambda}{dx}$ is the dispersion on the x-axis of the LCOS. It can be seen that the delay depends on the wavelength and the position of $x$.
# Results
![|355](https://i.imgur.com/1Z7a0mF.png)
![|340](https://i.imgur.com/1P69KgG.png)

Obviously, compared with the previous solution using VIPA, it can be more finely controlled.
# Discussion
This article is relatively old, most of the solutions have been replaced by digital micromirror devices (DMD), and we can find some reasons for using DMDs instead of LCOS in the related literature [9-11]. Moreover, the application point of this article is only in optical networks, and in fact similar techniques can be applied in more directions such as [11-12].
# Reference
[1]B. Mukherjee, I. Tomkos, M. Tornatore, P. Winzer, and Y. Zhao, “Springer Handbook of Optical Networks,” 15-Oct-2020. 
[2]R. Ramaswami, K. N. Sivarajan, G. H. Sasaki, R. Ramaswami, K. N. Sivarajan, and G. H. Sasaki, “chapter 1 - Introduction to Optical Networks,” 01-Jan-2010. 
[3]N. Networks, “What Is Fibre Optics & How Does It Work?,” 01-Jan-2023. 
[4]D. J. Richardson, J. M. Fini, and L. E. Nelson, “Space-division multiplexing in optical fibres,” 01-May-2013. 
[5]M. C. Wu, O. Solgaard, and J. E. Ford, “Optical MEMS for Lightwave Communication,” 01-Dec-2006. 
[6]M. Shirasaki, “Compensation of chromatic dispersion and dispersion slope using a virtually imaged phased array,” 01-Mar-2001. 
[7]G.-H. Lee, S. Xiao, and A. M. Weiner, “Optical Dispersion Compensator With≫4000-ps/nm Tuning Range Using a Virtually Imaged Phased Array (VIPA) and Spatial Light Modulator (SLM),” 01-Sep-2006.
[8]“衍射效率·不同偏振光下的衍射效率 | 岛津中国.” https://www.shimadzu.com.cn/optical/guide/diffraction/08.html. 
[9]Gao, Y., Chen, X., Chen, G., Tan, Z., Chen, Q., Dai, D., Zhang, Q., & Yu, C. (2019). Programmable Spectral Filter in C-Band Based on Digital Micromirror Device. Micromachines, 10(3), 163.
[10]A. R. Faustov, M. R. Webb, and D. R. Walt, “Note: Toward multiple addressable optical trapping,” 26-Feb-2010.
[11]A. R. Faustov, M. R. Webb, and D. R. Walt, “Note: Toward multiple addressable optical trapping,” 26-Feb-2010. 
[12]Xue Dong, Xingchen Xiao, Yining Pan, Guangyao Wang, and Yiting Yu, "DMD-based hyperspectral imaging system with tunable spatial and spectral resolution," Opt. Express **27**, 16995-17006 (2019)
[13]Y. Zhang, Y. Fu, Q. Liu, L. Wang, S. Yang, S. Liang, J. Zhang, J. Zhong, B. Zhao, and Y. Meng, “Large dynamic range stellar radiation simulation optical system,” 19-Jan-2024. 



