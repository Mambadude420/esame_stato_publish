---
lastSync: Tue May 27 2025 22:12:29 GMT+0200 (Ora legale dell’Europa centrale)
aliases:
  - motore a corrente continua a magneti permanenti
---
A direct current permanent magnet motor supplied by a voltage $V$ reaches a no-load velocity
$$
\omega_{0} = \frac{V}{K_{E}}
$$
At start-up it develops a torque[^1]
$$
C_{s} = K_{T} \cdot I_{s} = K_{T} \cdot \frac{V}{R}
$$
where $K_{E}$ is the voltage constant, that is equal to the torque constant $K_{T}$.

The $C - \omega$ characteristic moves parallel to itself with the varying supply voltage.

The efficiency of a motor is given by the ratio:
$$
\eta = \frac{P_{u}}{P_{i}} = \frac{C \cdot \omega} {V \cdot I}
$$
Expressing it as a function of the absorbed current, we get
$$
\eta = \left( 1 - \frac{I}{I_{S}} \right) \cdot \left( 1 - \frac{I_{0}}{I} \right)
$$
Maximum efficiency is obtained when the current $I_{\eta M}$ yields $P_{j} = P_{0}$.
$$
I_{\eta M} = \sqrt{ I_{0} \cdot I_{S} }
$$
Maximum efficiency is given by
$$
\eta_{M} = \left( 1- \sqrt{ \frac{I_{0}}{I_{S}} } \right)^2
$$

[^1]: una coppia
