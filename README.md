# Assignment-H5-Control-Aircraft-pitch-control

You need to design a control system for the pitch of an aircraft. The system is illustrated in Figure 1.
The manipulated input is the elevator deflection angle, δ; changing the deflection rate affects the pitch
of the aircraft. In Figure 1, α denotes the angle of attack, which is the angle between the longitudinal
axis of the aircraft and its velocity vector. The pitch angle of the aircraft is denoted by θ. The pitch
rate is denoted by r.
Figure 1: Illustration of an aircraft with its pitch angle, θ, the angle of attack, α, and the deflection
angle of the elevators, δ. The angle γ = θ − α is known as the slope.
The system dynamics is described by the following system of differential equations
 ̇α = − 0.31α + 57.4r + 0.232δ, (1a)
 ̇r = − 0.016α − 0.425r + 0.0203δ, (1b)
 ̇θ = 56.7r, (1c)
where all quantities are in SI units1. In addition, the deflection angle of the elevators is controlled by
an actuator whose dynamics has been found to be of the first order with unit static gain and a time
constant of 14.5 ms. The sensor has the transfer function
Gm(s) = exp(−0.0063s)
0.0021s + 1 . (2)
1In Equation (1), α, θ and, δ are measured in radians — not degrees — and q is measured in radians per second.
1
