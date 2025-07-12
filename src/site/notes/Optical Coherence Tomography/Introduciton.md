---
{"dg-publish":true,"cssclasses":["img-grid"],"permalink":"/Optical Coherence Tomography/Introduciton/","dgPassFrontmatter":true,"created":"2025-07-12T09:37:31.244+08:00","updated":"2025-07-12T15:57:29.895+08:00"}
---

# What is Optical Coherence Tomography?
## Basic Understanding
Optical Coherence Tomography (OCT) is a non-contact optical measurement that can precisely measure the distance, and is mainly used for imaging the laminated structure of objects. Currently, it can be divided into two types: time-domain (TD-OCT) and Fourier-domain (FD-OCT), with a resolution of 1-15 um and an imaging depth of about 2 mm, and FD-OCT can usually achieve higher resolution and signal-to-noise ratio[1-3].
## How it Work?
Now let's consider how an OCT system can make measurements, the simplest idea is to shine light on a sample and measure the intensity of the reflected light and the time difference between the two beams. This is essentially the same method as ultrasound measurements, but it is not applicable to optical measurements because the speed of light is far too fast to be measured by a machine with accurate time intervals. Of course, we can use femtosecond time-domain measurements to take advantage of this approach, but at a wavelength of $625nm$ the resolution of this approach is only $15\mu m$ [4], and the signal-to-noise ratio is far lower than that required for biological tissues.
![250|275](https://i.imgur.com/FnGytI4.png)![375|400](https://i.imgur.com/UCvL5nD.png)
Although the discussion just now did not lead to a general principle of measurement, we note that both ultrasound imaging and femtosecond measurements are based on measuring the intensity of reflected light as well as the time difference obtained. Since the speed of light is essentially constant, the time difference is equivalent to the optical range difference. And with the combination of light-range difference and intensity, we think of interference-which can be thought of as a phenomenon of amplitude modulation by light-range difference.
Further, we know that interference is the interaction between fields, which can be measured by interferometers, Michelson interferometers, Mach Zender interferometers, ..., there are already too many classical interferometer structures to choose from. It is worth noting that interferometers are used to measure the interaction between the electric fields of two beams of light, a process that is not actually visible and requires the use of components such as CCDs to convert the electric field into light intensity.
Next let's consider some details on how to utilize interferometry? We have chosen to use a Michelson interferometer and based on the figure below we have the following derivation:![](https://i.imgur.com/ypI0lD7.png)
![|700](https://i.imgur.com/OghuGrD.png)

$$
I=4I_{0}\cos \frac{k\delta}{2}
$$
The CCD at the back end converts the electric field amplitude into light intensity, and the light intensity is modulated by the distance between the two arms. The simplest way to solve for $k\delta$ is by inverse trigonometry, but this obviously leads to multiple solutions. Therefore we utilize the coherence length $l_{c}=\frac{\lambda_{0}^2}{\Delta \lambda}$ and select a broadband light source to make $l_{c}$ as small as possible so that when interference occurs, we have
$$
0\to l_{c}\geq |l_{r}-l_{s}|\implies l_{r}\to l_{s}
$$
**A suitable broadband light source is selected and the reference arm is configured with a motor for scanning, so that when interference occurs, the two arms are approximately equidistant from each other.**
## Disadvantage and Improve

## Performance Indicators and Corresponding Determinants
| index                 | factor             | magnitude        | expression                                                        |
| --------------------- | ------------------ | ---------------- | ----------------------------------------------------------------- |
| axial resolution      | bandwidth          | $1-15\mu m$      | $\Delta z=\frac{2\ln2}{\pi}  \frac{\lambda^2}{\Delta \lambda}$    |
| imaging depth         | center wavelength  | $2mm$            | $\pm z_{max}=\pm   \frac{n_{0}\lambda_{0}^2}{4\delta_{s}\lambda}$ |
| transverse resolution | numerical aperture | $5\mu m-20\mu m$ | $\delta x=\frac{4\lambda}{\pi}  \frac{f}{d}$                      |
# Reference
[1]Choma, M. A., Sarunic, M. V., Yang, C., & Izatt, J. A. (2003). Sensitivity advantage of swept source and Fourier domain optical coherence tomography. _Optics express_, _11_(18), 2183-2189.
[2]Wojtkowski, M., Srinivasan, V. J., Ko, T. H., Fujimoto, J. G., Kowalczyk, A., & Duker, J. S. (2004). Ultrahigh-resolution, high-speed, Fourier domain optical coherence tomography and methods for dispersion compensation. _Optics express_, _12_(11), 2404-2422.
[3]Leitgeb, R., Hitzenberger, C. K., & Fercher, A. F. (2003). Performance of fourier domain vs. time domain optical coherence tomography. _Optics express_, _11_(8), 889-894.
[4]Fujimoto, J. G., De Silvestri, S., Ippen, E. P., Puliafito, C. A., Margolis, R., & Oseroff, A. (1986). Femtosecond optical ranging in biological systems. _Optics letters_, _11_(3), 150-152.