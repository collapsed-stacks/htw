## How does a Flash Drive work?

- posted by: [bcsanches](https://stackexchange.com/users/-1/17-bcsanches) on 2011-04-18
- tagged: `computers`, `data-storage`, `memory`
- score: 6

I'm curious: how does a flash drive store data? What allows it to be read and written, and also to keep this data when disconnected from a computer?




## Answer 26

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-18
- score: 6

A flash drive is basically a small Solid state drive also know as non volatile memory because loss of electricity doesn't affect data on it like RAM for example. It works by have several billion transistors that are either off(0) or on(1). So because computers store info in binary, this works well, for example if I need to store a 1 in binary to a flash drive I simply turn a transistor on vs moving the magnetic field around on a traditional Hard disk.


## Answer 172

- posted by: [starblue](https://stackexchange.com/users/-1/107-starblue) on 2011-04-19
- score: 2

A single unit of data storage in flash or EEPROM memory is a field effect transistor (FET) with an electric charge trapped in its gate. Trapped means that it stays there even if power is removed. To erase or write the charge a higher voltage is applied, to force the electrons in or out. This slightly damages the memory cell, which thus wears out over thousands of write cycles.

Whether the transistor conducts depends on the charge, this can be used for reading the value stored in the cell.

The unit of storage is a single bit for most types of devices. Multiple bits corresponding to multiple levels of charge are used in the latest high density flash devices, mostly for use in SSDs.




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
