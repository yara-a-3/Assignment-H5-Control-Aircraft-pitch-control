# Assignment-H5-Control-Aircraft-pitch-control

You need to design a control system for the pitch of an aircraft. The system is illustrated in Figure 1.
The manipulated input is the elevator deflection angle, δ; changing the deflection rate affects the pitch
of the aircraft. In Figure 1, α denotes the angle of attack, which is the angle between the longitudinal
axis of the aircraft and its velocity vector. The pitch angle of the aircraft is denoted by θ. The pitch
rate is denoted by r.

![image](https://github.com/user-attachments/assets/8d175db8-09d2-4563-a051-fd28ca65e91c)

Figure 1: Illustration of an aircraft with its pitch angle, θ, the angle of attack, α, and the deflection
angle of the elevators, δ. The angle γ = θ − α is known as the slope.

The system dynamics is described by the following system of differential equations 

$$
\dot{\alpha} = -0.31\alpha + 57.4r + 0.232\delta,
$$

$$
\dot{r} = -0.016\alpha - 0.425r + 0.0203\delta,
$$

$$
\dot{\theta} = 56.7r.
$$

where all quantities are in SI units1. In addition, the deflection angle of the elevators is controlled by
an actuator whose dynamics has been found to be of the first order with unit static gain and a time
constant of 14.5 ms. The sensor has the transfer function

$$Gm(s) = \frac{exp(−0.0063s)}{0.0021s + 1}$$

(In Equation (1), α, θ and, δ are measured in radians — not degrees — and q is measured in radians per second.)
