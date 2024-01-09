## Basic Math For ML (Review and New)

#### Vectors

- In CS we can think of these as just a list of attributes on an object. In space they are magnitudes with direction (in a classic 2D sense). _Or better put in the physics/algebra since they are objects that move you around physical space._
- Consider the following example of a single house:

```
floor_space = 120m^2
bedrooms = 2
bathrooms = 1
price = 150,000

```

$\begin{bmatrix} 120 \\
2 \\
1 \\
150 \end{bmatrix}$

- Addition and subtraction on vectors can be done on each component, pretty straightforward. Just add straight across the vectors.
- Multiplication of a scalar on a vector produces expected results, a negative coefficient will flip the vector's direction.
- Use Pythagorean theorum to calculate a vectors size.

- _The length of a vector is also known as its *size*_
- While easily applied to spatial directions (Like x (or a for right triangle axis), y (or b) 2D coordinate space), this rule that for the **vector-size** $r$ : $\begin {bmatrix}r\end{bmatrix} = \begin{bmatrix} a \cr b\end{bmatrix}$ _or_ $\begin{bmatrix}r\end{bmatrix} = \sqrt{a^2 + b^2}$
