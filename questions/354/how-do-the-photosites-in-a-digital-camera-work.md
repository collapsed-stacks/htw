## How do the photosites in a digital camera work?

- posted by: [mattdm](https://stackexchange.com/users/-1/172-mattdm) on 2011-04-24
- tagged: `electronics`, `sensors`, `cameras`
- score: 2

A digital camera sensor is CCD or CMOS chip which records the image. This chip has millions of tiny "photosites" that do the actual recording. Typically, these are covered in a pattern of red, green, and blue filters — the "Bayer color filter array" — to sort out wavelengths of light.

But how do the individual photoreceptors work?


## Answer 355

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-24
- score: 2

A CCD photo receptor (And CMOS, for that matter),works somewhat as follows. An incoming photon knocks an electron out of place. One key point is that the electron must transition the bandgap of the main material. For silicon, the minimum energy is around 1.1 um, but there are other materials with different band gaps. This electron will be stored as a charge, which is later measured. The charge is cleared out when the sensor is read, thus starting all over again. There are a few more subtle details, but this covers the basics. 

I should note that CCD and CMOS differ significantly in the rest of what follows, but they are otherwise the same.

In CCD arrays, the charge is actually passed from one neighboring cell to another. Once it gets to the end of the row, the signal is passed through an amplifier, then an analog to digital converter. 

This can actually create some artifacts. This is put into great use in orbiting sensors around planets. They can actually bin images in such a way that the charge is passed from one row to the next in the same amount of time it takes to move over the pixel's resolution at the orbiting planet. Thus a single pixel can be integrated twice, without loosing as much signal. In effect, it drastically improves the signal to noise ratio.

CMOS cameras typically have each pixel read in it's own information, thus reducing the amount of artifacts, but also reducing the amount of light a given pixel can receive.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
