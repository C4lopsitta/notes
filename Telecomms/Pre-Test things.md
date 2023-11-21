# Resistances
## In series
Calculating the equivalent resistance of $n$ resistances in series:
$$
R_{eq} = R_1 + R_2 + R_{\dots} + R_n
$$
## Parallel
To calculate the equivalent resistance of $n$ parallel resistances with different values:
$$
R_{eq} = \frac{1}{G_{eq}} = \frac{1}{\frac{1}{R_1} + \dots + \frac{1}{R_n}}
$$
so by converting the $\frac{1}{R_{n}}$ into a conductance unit it becomes:
$$
\begin{cases}
R_{eq} = \frac{1}{G_1 + \cdots + G_{n}} \\
\text{where } G_n = \frac{1}{R_n}
\end{cases}
$$
Or with only two resistances:
$$
R_{eq} = \frac{R_1 \cdot R_2}{R_1 + R_2}
$$
If two resistances in parallel have the same resistance value in $\Omega$ the equivalent resistance will be equal to it's half. Example:
$$
\begin{cases}
R_1 = 10\Omega \\
R_2 = 10\Omega \\
R_1 \parallel R_2 \\
R_{eq} = 5\Omega
\end{cases}
$$
Resistances in parallel with the same value can be easily calculated with the following formula:
$$
R_{eq} = \frac{R^2}{n-1}\cdot\frac{n-1}{n \cdot R}
$$
Applied to an example case with three resistances, it simply becomes:
$$
R_{eq} = \frac{R^2}{n-1}\cdot\frac{n-1}{n \cdot R} = \frac{R}{n}
$$
# Kirchhoff's laws
## First Law
The first law declares that all incoming currents summed are equivalent to the sum of the outgoing currents.
By standard, incoming currents are positive and outgoing currents are  negative.
$$
i_{incoming_1}+i_{\dots}=i_{outgoing_1}+i_{\dots}
$$
## Second Law
The second law defines that the tension incoming into a mesh is equivalent to the outgoing tension.
$$
V_1+V_2+V_n = V_3+V_4+V_n
$$
A graph of this has been drawn on the 31 of October at 11:50 on Tab S6 Lite Off Screen Notes.
# Meshes
Meshes are groups of nodes that are crossed once
## Star meshes
From triangle
$$
\begin{cases}
r_a = \frac{R_{AB}\cdot R_{AC}}{R_{AC}+R_{AB}+R_{BC}} \\
r_b = \frac{R_{AB}\cdot R_{BC}}{R_{AC}+R_{AB}+R_{BC}} \\
r_c = \frac{R_{AC}\cdot R_{BC}}{R_{AC}+R_{AB}+R_{BC}}
\end{cases}
$$
## Triangular meshes
From star
$$
\begin{cases}
R_{AB} = \frac{r_Ar_B+r_Br_C+r_Cr_A}{r_C} \\
R_{BC} = \frac{r_Ar_B+r_Br_C+r_Cr_A}{r_A} \\
R_{AC} = \frac{r_Ar_B+r_Br_C+r_Cr_A}{r_B}
\end{cases}
$$
## Star <=> Triangular
If all resistances are equivalent:
$$
3\cdot r_{star} = r_{triangle}
$$
Where $r_{triangle}$ represents the resistance between any two vertices.

# Tension Generators
## Ideal Generator
Represented by a circle and a line. It generates as much current as it's written it generates. It has an arrow to show the direction.