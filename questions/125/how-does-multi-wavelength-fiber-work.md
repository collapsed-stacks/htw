## How does multi-wavelength fiber work?

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-19
- tagged: `electronics`, `computers`, `technology`, `fiber`
- score: 5

I know several wavelengths are used in fiber communications, but how does the system differentiate the different wavelengths? Is it similar to radio waves where there are several frequencies?


## Answer 167

- posted by: [txwikinger](https://stackexchange.com/users/-1/40-txwikinger) on 2011-04-19
- score: 3

You can have single wavelength fibers and multi-wavelength fibers. The main difference is the transmission characteristic of the material. A single wavelength fiber has a very narrow frequency spectrum which allows optimal transmission (i.e. with low loss of signal strength and low dispersion - dispersion is actually the more important factor). In difference multi wavelength fibers will provide a far broader spectrum with such characteristics and hence allow multiple wave length travel through it with the same quality on the other end. However, usually multi wave length fibers are more expensive to manufacture and more have slightly more loss.


## Answer 212

- posted by: [mgb](https://stackexchange.com/users/-1/15-mgb) on 2011-04-19
- score: 1

<p>Just to complicate matters - modern multiple wavelength fibre systems using <a href="http://en.wikipedia.org/wiki/Wavelength-division_multiplexing#DWDM_systems" rel="nofollow">DWDM</a> do use almost single wavelength fibre. </p>

<p>The channels are only spaced around 0.5nm apart and all fit into the nominal wavelength band of the fibre around 1550nm.</p>



## Answer 130

- posted by: [zefciu](https://stackexchange.com/users/-1/98-zefciu) on 2011-04-19
- score: 0

Yes, it is quite similar, because you can send more data if you use several wavelengths. The fiber doesn't differentiate them itself (rather the diode/laser and sensor do), however there are some negative optical effects (like dispersion and absorption) which are wavelength-dependent. This is why only small portions of the spectrum are used in optical fibers.



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
