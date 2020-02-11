# Reversible Gates

Tags: Part I, SubUnit I

# Circuits and Entropy

- Classic gates destroy randomness → Consume energy!
- By Landauer's principle:

$$kT \ln 2 \text{ energy needed per bit!}$$

- Need reversible gates to preform low energy computing.

# Reversible Gates

1. **CNOT**: Controlled NOT

    ![Reversible%20Gates/Untitled.png](Reversible%20Gates/Untitled.png)

    Controlled Not, if X is true, output is NOT Y . Otherwise, all stay the same.

2. **Toffoli gate** or CCNOT: Controlled Controlled NOT.

    This gate is universal by itself, because it can simulate both AND and NOT gates.

    ![Reversible%20Gates/Untitled%201.png](Reversible%20Gates/Untitled%201.png)

    If both X and Y are true, output is NOT Z. Otherwise, all stay the same.

3. **Fredkin gate** or CSWAP: Controlled Swap.

    This gate is universal by itself, because it can simulate both AND and NOT gates.

    If we set Y =1 and Z = 0, it simulates the NOT gate! 

    Fredkin gate cannot change the Hamming weight (number of one's) of its inputs.

    ![Reversible%20Gates/Untitled%202.png](Reversible%20Gates/Untitled%202.png)

    If X is true, Y and Z get swapped,.Otherwise, all stay the same.

    **Theorem**: The number of garbage outputs in these gates to simulate a circuit is O(width of circuits).

    **Theorem**: Any Boolean circuit of size n can be simulated by a reversible circuit of order of polynomial
    in n reversible gates. (approx. O(n^2)) 

    **Def**. : “in-place reversible" : No garbage bits are allowed, and no extra ancilla bits are provided (constant zero or one).