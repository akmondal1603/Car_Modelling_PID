# Car_Modelling_PID
PID Block of SIMULINK
Tune the gains and configuration until satisfactory performance of the model is not achieved.

# Forces in Action
•  Traction force: energy conversion from electric to mechanical through motor and wheels.
•  Aerodynamic drag: air displacement when moving or due to wind gusts.
•  Rolling resistance: tyre deformation on the ground due to the weight of the car.
•  Car Inertia: inherent property of masses to resist changes in motion.

# Rolling Resistance
𝐹𝑟=𝐶𝑟∗𝑚𝑇∗𝑔
With 𝐶𝑟 is the rolling resistance coefficient, 𝑚𝑇 the total mass of the car and _g_ the gravitational constant.

# Aerodynamic Drag
𝐷=1/2(𝜌𝑉^2)(𝑆𝐶_𝐷)
With 𝜌 the air density, V the velocity of the car, S its frontal area and 𝐶_𝐷 its coefficient of Drag

# Torque to Traction Force
𝐹𝑓=𝑇𝐿∗𝐺𝑟
Where 𝐹𝑓: Resultant force, 𝐺𝑟: Gear ratio, L: Distance from center of rotation

# Mathematical mnodel
Torque as a function of Voltage Input and rotational velocity:
𝑇(𝑠)=𝐾_𝑇∗[{𝑉(𝑠)−𝐾_𝐸∗𝜔(𝑠)}/{𝑠𝐿+𝑅}]
where 𝑅=5.3∗10−3𝑂ℎ𝑚
      𝐿=493∗10−9𝐻𝑒𝑛𝑟𝑦𝑠
      𝐾_𝐸=0.12𝑉𝑠/𝑟𝑎𝑑
      𝐾_𝑇=0.25𝑁𝑚/𝐴𝑚𝑝
