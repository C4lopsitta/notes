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
The second law defines that the tension incoming into a mesh is equivalent to the outgoing tension 
## Mesh
A mesh is group of nodes that are crossed only once 