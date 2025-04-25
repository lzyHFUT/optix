---
{"dg-publish":true,"cssclass":"img-grid","permalink":"/Weekly reading/Journal of Lightwave Technology; Wavelength Selective Switch/","dgPassFrontmatter":true,"created":"2025-04-25T22:27:07.540+08:00","updated":"2025-04-26T00:41:12.000+08:00"}
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
		- ![Pasted image 20250426001443.png|300](/img/user/Weekly%20reading/Pasted%20image%2020250426001443.png)![Pasted image 20250426002015.png|325](/img/user/Weekly%20reading/Pasted%20image%2020250426002015.png)
		- The shape of the mirror is $c(y)=\frac{K}{8f^4}y^4+\frac{{K\Theta}}{2f^3}y^3+\frac{{K\Theta^2-(f-a)}}{2f^2}y^2$, and the slope of the graph can be represented by $-\frac{2n^4K}{c\lambda}$. The final system is designed to be regulated by adding a grating diffraction, where different wavelengths arrive at different positions after diffraction, and different positions have different shapes.
		- ![Pasted image 20250426002102.png|300](/img/user/Weekly%20reading/Pasted%20image%2020250426002102.png)![Pasted image 20250426003356.png|325](/img/user/Weekly%20reading/Pasted%20image%2020250426003356.png)
- **SLM:** [7]First use VIPA to spectralize according to the wavelength, then use SLM to adjust the reflection angle.
- ![Pasted image 20250426003804.png|425](/img/user/Weekly%20reading/Pasted%20image%2020250426003804.png)
## The solution to this article
Using LCOS as a Wavelength Selection Switch
![Pasted image 20250426004011.png|500](/img/user/Weekly%20reading/Pasted%20image%2020250426004011.png)
# Methods



# Reference
https://books.google.com.hk/books?id=EisDEAAAQBAJ&dq=directionless+roadm&pg=PA620&redir_esc=y#v=onepage&q=directionless%20roadm&f=false

https://www.sciencedirect.com/science/article/pii/B9780123740922500096

https://neosnetworks.com/resources/blog/fibre-optics-what-is-it-and-how-does-it-work/

https://www.nature.com/articles/nphoton.2013.94

https://ieeexplore.ieee.org/document/4063445

https://ieeexplore.ieee.org/document/927385

https://ieeexplore.ieee.org/document/1673476




