# 3D Velocity Obstacle (VO) Airspace Detect and Avoid Engine

![C++17](https://img.shields.io/badge/Language-C%2B%2B17-blue)
![UTM](https://img.shields.io/badge/Domain-Avionics%20%26%20UTM-orange)
![Developer](https://img.shields.io/badge/Developer-Ayoub%20Lahmar-brightgreen)

A deterministic \(3\text{D}\) airspace conflict detection and resolution system based on **Velocity Obstacles (VO)**. Evaluates geometric collision cones within time-horizon boundaries \(\tau\) and projects optimal non-conflicting velocity vectors \(\vec{v}_{safe}\).

Implemented by **Ayoub Lahmar** ([@Redayoub-lang](https://github.com/Redayoub-lang)).

## 📐 Mathematical Formulation

The Velocity Obstacle region \(VO_{A \oplus B}\) for intruder \(B\) relative to ownship \(A\) is defined in velocity space as:
$$VO_{A \oplus B} = \left\{ \vec{v}_A \mid \exists t \in [0, \tau], \quad (\vec{v}_A - \vec{v}_B)t \in \mathcal{B}(P_B - P_A, R_A + R_B) \right\}$$Where $\mathcal{B}(x, r)$ denotes a spherical volume centered at offset $P_B - P_A$ with safety radius $R_A + R_B$.💻 Build & Compile
g++ -std=c++17 -O3 main.cpp -o VODAAEngine
./VODAAEngine