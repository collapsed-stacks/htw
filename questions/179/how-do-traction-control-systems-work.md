## How do Traction Control Systems work?

- posted by: [Noctrine](https://stackexchange.com/users/-1/50-noctrine) on 2011-04-19
- tagged: `vehicles`, `automobile`
- score: 3

How do Traction Control Systems work, or specifically what causes them to 'kick-in' so to speak?


## Answer 187

- posted by: [Christopher](https://stackexchange.com/users/-1/129-christopher) on 2011-04-19
- score: 2

IANAM (I Am Not A Mechanic!) but this is my (researched) understanding of TCS:

Traction Control Systems work primarily by sensing the amount of rotation through the drive wheels relative to the power being applied (that is, the wheels connected to the driveshaft and receiving power from the engine through the differential) along with calculated factors such as slip angle. Rotation and torque amounts through the differential play a crucial part in these measurements, along with engine revs and engine torque; cylinder spark and valve timing (or firing), independent application of brakes and adjustment of the fuel supply to the engine (for fly-by-wire vehicles) are typically electronically adjusted in realtime in modern vehicles.

More sophisticated TC systems employ active differentials which sense the yaw of a vehicle during turns and can redistribute power to the drive wheels depending on road conditions, with the added benefit of allowing the EMS to calculate optimal slip angle for the outside tyres along with relative rotational speeds and control the redistribution of power. (Innermost wheels rotate more slowly than outer wheels when a car goes through a corner; simpler differentials on two-wheel drive vehicles only redistribute power across the drive wheels based on a purely mechanical operation.)



The level of traction is measured tens or hundreds of times per second to allow the powertrain's management system (aka the EMS) to constantly adjust the level of power sent through the wheels irrespective of how leaden-footed the driver may be. TCS' operation is also similar to the operation of All Wheel / Four Wheel Drive where power is redistributed from the wheels experiencing low traction to ensure continued velocity and traction. (Audi's "quattro" system was the first successful widescale commercial implementation of an AWD system after its wildly successful debut in the eponymously named rallygoing "Audi Quattro".) AWD vehicles also employ more complex differential and transaxle systems; this however falls outside the scope of this response.


Rear wheel drive vehicles and high-powered motorcycles benefit more from TCS than front wheel drive vehicles - by controlling excessive wheelspin and subsequent loss of drive (and resultant oversteer) in low-grip conditions it becomes useful as a safety feature and avoids the requirement to constantly modulate throttle input. The predecessor to TCS was the limited-slip differential, still common in many competitive vehicles as seen in British Touring Cars / German DTM and other hi-octane motorsports.

TCS engagement can be more obviously heard on high-powered motorsports vehicles like MotoGP motorbikes and pre-2009 Formula 1 cars (audible as brief spurts of white noise or distortion in the otherwise-regular engine tone) as the regular operation of the driveshaft, clutch and throttle are computer-compensated for the wheelspin. Usage in this scenario maximises drivetrain efficiency, wheel slip (for optimal traction) and application of power through corners.



There are numerous other factors additionally measured in more sophisticated combined systems, such as velocity, direction of travel, degrees of travel on the steering and amount of pressure applied to pedals. There is some crossover here with "Electronic Stability Programme" features on some cars such as BMWs; it is advisable to disable ESP (or enable 'Snow Mode' or a limited operation mode) on rear wheel drive vehicles as the TCS & ESP will by its nature cause a gradual loss of power to the drive wheels as it cannot understand the low-traction situation, instead interpreting it as an uncontrolled wheelspin or slide. ABS should always be disabled in snowy conditions as the system will continue to reduce braking power to the point where the vehicle is not being slowed down at all!



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
