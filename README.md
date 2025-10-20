**Overview**

This project implements a numerical approach for approximating eigenfunctions and eigenvalues of quantum mechanical systems governed by the time-independent Schrödinger equation. By combining the Runge–Kutta method for solving differential equations with a root-finding algorithm, the code determines energy levels for a range of standard potentials drawn from theoretical and research literature.

The work was completed as part of the PHAS0029 Computational Physics module.



**Methodology**

The algorithm proceeds as follows:

Runge–Kutta Integration (4th Order):
Used to numerically propagate the wavefunction across a spatial domain for a trial energy 
𝐸.

Boundary Condition Enforcement:
The wavefunction is required to vanish at spatial boundaries to ensure physical validity.

Root-Finding Routine:
A root-finding algorithm (e.g. bisection or Newton–Raphson) iteratively adjusts 
𝐸 to satisfy the boundary conditions.

Eigenfunction Normalization:
Once an eigenvalue is found, the corresponding eigenfunction is normalized and plotted.


**Potentials Studied**

The solver was tested on several canonical potentials:
<br>
Infinite Square Well
<br>
Harmonic Oscillator
<br>
Finite Square Well
<br>
Double Potential

Comparisons were made between numerical and analytical eigenvalues where available.


**Results**

Numerical eigenvalues closely match analytical results for benchmark systems (errors typically < 1%).

The Runge–Kutta method ensures high accuracy and stability even for steep potentials.

Wavefunctions exhibit the expected symmetry and node structure consistent with quantum theory.


**Dependencies**

Python ≥ 3.9
<br>
NumPy
<br>
SciPy
<br>
Matplotlib
