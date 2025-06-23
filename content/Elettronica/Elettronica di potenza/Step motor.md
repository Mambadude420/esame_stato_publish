---
lastSync: Wed May 28 2025 11:22:30 GMT+0200 (Ora legale dell’Europa centrale)
aliases:
  - stepper motor
---
Step, or stepper motors, turn a constant angle $\gamma$, known as a step, with every command.

There are three types of step motors:
- Permanent Magnet (PM);
- Variable Reluctance (VR);
- Hybrid (HY)

The permanent magnet (PM) motor has cylindrical permanent magnet rotor with magnetic poles on the rotor's surface. $D$ indicates the number of pole pairs. The angle $\alpha$ taken up by one pole pair is:
$$
\alpha = \frac{360^\circ}{D}
$$
The PM motor is robust and inexpensive

The full step configurations can be obtained by energizing one phase at a time, or by energizing two phases simultaneously; in the second case better performances and a more regular operation are obtained; in the second case better performances and a more regular operation are obtained.

The full step command uses all configurations of the same type. The half-step command alternates a single phase configuration with a two-phase configuration.

The step motor drive circuits receive logical commands that define the sequence of the configurations and supply the motor windings with the same configurations at suitable power.

Step frequency $f_{p}$ is defined as the number of steps carried out in one second and step time $T_{p}$ as the duration of one step
$$
T_{p} = \frac{1}{f_{p}}
$$
During $T_{p}$ the rotor describes an angle $\gamma$.

The angular velocity of the step motor is equal to:
$$
\omega = \frac{{2 \pi}}{T_{p} \cdot S} \text{[rad/s]} \quad\text{oppure} \quad n = \frac{60}{T_{p} \cdot S} \text{[giri/min]}
$$
Where $S = \frac{{360^\circ}}{\gamma}$ (number of steps).

A number of drive schemes are possible, but the most common is the bipolar drive scheme.

The bipolar motor has only one winding per phase. Each winding is driven in both directions by means of a bridge circuit.

Four transistors per phase are required for bipolar driving, sized appropriately to conduct the phase current and to withstand the input voltage.