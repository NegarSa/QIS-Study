# Single Qubit!

Tags: Part I, SubUnit II

### Date: Yesterday

# Topic:  Single Qubit!

### Recall

Quantum States

Bloch Sphere 

Rotations of the sphere

Single qubit gates

Relations?

Unitary Transitions

Copenhagen interpretation

Rotation of Theta around Axes?  

Degrees of Freedom for Rotation?

(2x2 unitary)

### Notes

- Are vectors
- ***Global*** phases don't change states!
- Any pure state of a two-level quantum system can be written as a superposition of the basis vectors |0⟩ and |1⟩, where the coefficient or amount of each basis vector is a complex number.
- Any state:

    $${\displaystyle |\psi \rangle =\cos \left(\theta /2\right)|0\rangle \,+\,e^{i\phi }\sin \left(\theta /2\right)|1\rangle }$$

- Main points:

    ![Single%20Qubit/Untitled.png](Single%20Qubit/Untitled.png)

- Also note:

    [Understanding the Bloch sphere](https://physics.stackexchange.com/a/205209)

    [Introduction to quantum computing: Bloch sphere.](http://akyrillidis.github.io/notes/quant_post_7)

- Each rotate around the axis!

    ![Single%20Qubit/Untitled%201.png](Single%20Qubit/Untitled%201.png)

- Gates!

    ![Single%20Qubit/Untitled%202.png](Single%20Qubit/Untitled%202.png)

The Hadamard gate acts on a single qubit. It maps the basis state |0⟩  to |0⟩ + |1⟩ / 2  and |1⟩  to |0⟩ − |1⟩ / 2, which means that a measurement will have equal probabilities to become 1 or 0 (i.e. creates a superposition)

$$S^2 = \sigma_z, \ T^2 = S$$

$$\sigma_x\sigma_y = i\sigma_z = -\sigma_y\sigma_x$$

$$\sigma_y\sigma_z = i\sigma_x = -\sigma_z\sigma_y$$

$$\sigma_z\sigma_x = i\sigma_y = -\sigma_x\sigma_z$$

- **Result**: The three Pauli vectors are anti-commute pairs.

$$U\ |i\rangle = |C_i\rangle$$

Ci is of unit length. Also, Ci is the ith column of U.

$$U = \sum_{i=1}^{d-1} |C_i\rangle \langle i|$$

Where d is the dimension of the state space. Now:

 

$$U|j\rangle = \sum_{i=1}^{d-1} |C_i\rangle \langle i|j\rangle = \sum_{i=1}^{d-1} |C_i\rangle \delta_{ij} = C_j$$

**Def** 1: Takes a complex unit vector to another.

**Def** 2: All columns are unitary vectors and orthogonal. (takes a basis to another)

**Def** 3: All rows are unitary vectors and orthogonal.

**Def** 4: 

$$U^{-1} = U^{\dagger}$$

Two Kinds of Processes:

- Unitary
- Measurement

$$e^{i\theta \sigma_z/2}, ...$$

$$U = e^{i\alpha}\begin{pmatrix}     \cos \theta       & e^{i\phi_2}\sin \theta  \\     e^{i\phi_1}\sin \theta       & -e^{i(\phi_2 - \phi_1)}\cos\theta  \end{pmatrix}$$

3 Degrees of freedom! 

Note: Above formula is diff in lecture, why am I wrong?

Every Transformation can be done by a transformation around x, z, and x. (So 3 deg. of freedom again!)

> *On the Bloch sphere, the axis of rotation of a single-qubit gate U is the line going from the center of the Bloch sphere, and a point p⃗ =(px,py,pz) on the Bloch sphere, corresponding to an eigenstate of U.*

**SUMMARY: Bloch Sphere, Unitary Matrices and Rotations! ⇒ Quantum Gates.**

---