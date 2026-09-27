## 📐 Mathematical Formulation

The Velocity Obstacle region \(VO_{A \oplus B}\) for intruder \(B\) relative to ownship \(A\) is defined in velocity space as:

$$
VO_{A \oplus B} = \left\{ \vec{v}_A \mid \exists t \in [0, \tau], \quad (\vec{v}_A - \vec{v}_B)t \in \mathcal{B}(P_B - P_A, R_A + R_B) \right\}
$$

Where \(\mathcal{B}(x, r)\) denotes a spherical volume centered at offset \(P_B - P_A\) with safety radius \(R_A + R_B\).
