---
aliases: 
publish: true
parent:
  - "[[512.64  Linear algebra MOC]]"
---
#anki

### Between two [[Point]]s
$$
d(p, q) = ||q - p|| = \sqrt{(q_x - p_x)^2 + (q_y - p_y)^2 + (q_z - p_z)^2}
$$

### Between a line and the origin
Line: $l : \{ p_o + t \vec{v}, t \in R \}$ and origin $O = (0, 0, 0)$
$$
\Large d(l, O) = || p_o - \frac{p_o \cdot \vec{v}}{||\vec{v}||^2}\vec{v} ||
$$
![[Pasted image 20230913142456.png|300]]

### Between a [[Plane]] and the origin
Line: $\Large P: \{\vec{n}\cdot [(x, y, z) - p_o] = 0 \}$ and origin $O = (0, 0, 0)$
$$
\Large d(P, O) = \frac{|\vec{n} \cdot p_o|}{||\vec{n}||}
$$
![[Pasted image 20230913142909.png|300]]






