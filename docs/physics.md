
This page describes the fundamental physics behind the radio telescope.

> **BEWARE!** There is lots of math in this section! If math causes you emotional and physical distress, do not read this page!

<img src="https://imgs.xkcd.com/comics/physics_safety_tip_2x.png" alt="A cartoon about physicists" width="300" />

## Electromagnetic waves

Radio waves from space are just a type of electromagnetic radiation, like infrared, UV light, etc. Electromagnetic waves can be described using Maxwell's equations:

$$
\begin{align*}
\nabla \cdot \mathbf{E} &= \rho/\varepsilon_0 \\
\nabla \cdot \mathbf{B} &= 0 \\
\nabla \times \mathbf{E} &= -\frac{\partial \mathbf{B}}{\partial t} \\
\nabla \times \mathbf{B} &= \mu_0\mathbf{J} + \mu_0 \varepsilon_0\frac{\partial \mathbf{E}}{\partial t} \\
\end{align*}
$$

Where $\mathbf{E}, \mathbf{B}$ are the electric and magnetic fields, $\mu_0 \approx \pu{1.257E-6 N*A^{-2}}$ and $\varepsilon_0 \approx \pu{8.854E-12 F*m^{−1}}$ are the vacuum permeability and permittivity, $\rho$ is the charge density, $\mathbf{J}$ is the current density, and the speed of light $c$ is given by:

$$
c = \frac{1}{\sqrt{\mu_0 \varepsilon_0}}
$$

With some vector calculus we can show that in free space (where $\rho = \mathbf{J} = 0$) the Maxwell equations reduce to two wave equations:

$$
\begin{align*}
\frac{\partial^2 \mathbf{E}}{\partial t^2} = c^2 \nabla^2 \mathbf{E} \\
\frac{\partial^2 \mathbf{B}}{\partial t^2} = c^2 \nabla^2 \mathbf{B}
\end{align*}
$$

The simplest solutions of the wave equation are **plane waves**, given by:

$$
\begin{align*}
\mathbf{E}(\mathbf{r}, t) &= \mathbf{E}_0 e^{i\phi}, \quad \phi = \mathbf{k} \cdot \mathbf{r} - \omega t, \quad \mathbf{E}_0 = E_0 \hat{\mathbf{n}} \\
\mathbf{B}(\mathbf{r}, t) &= \frac{1}{c} \mathbf{n} \times \mathbf{E}
\end{align*}
$$

Where $E_0$ is the electric field's amplitude, $\phi$ is the phase, $\hat{\mathbf{n}}$ is the polarization vector, $\mathbf{k}$ is the wavevector, and $\omega = |\mathbf{k}|c$ is the angular frequency of the waves. The angular frequency and wavevector can also be related to the frequency $\nu$ and wavelength $\lambda$ with:

$$
\omega = 2\pi \nu, \quad k = |\mathbf{k} | =\frac{2\pi}{\lambda}
$$

And the magnetic field amplitude $\mathbf{B}_0$ is related to the electric field amplitude $\mathbf{E}_0$ with:

$$
|\mathbf{E}_0| = |\mathbf{B}_0|c
$$

## Atomic transitions and spectra

Due to quantum mechanics, the electromagnetic field is **quantized** and we know that the classical electromagnetic field is a *quantum field*. The quantum field associated with electromagnetism is the **photon field**, whose excitations are fundamental particles known as photons.

Atoms cause absorb and emit photons due to their quantized (discrete) energy levels, which can be calculated approximately using the Schrodinger equation:

$$
H \psi_n = \left(-\frac{\hbar^2}{2m}\nabla^2 + V\right) \psi = E_n \psi_n
$$

Where $H$ is the quantum Hamiltonian, $\psi_n$ are the eigenstates of the system, $E_n$ are the energy levels (quantized energies) of the system, and $V$ is the potential. The Schrodinger equation can be solved approximately via perturbation theory to find the energy levels. Physically, when an atom jumps from one energy level to another, a **quantum transition** occurs. The 21 cm line is the result of the hyperfine transition in atomic hydrogen. The two lowest hyperfine energy levels in hydrogen has an energy difference $\Delta E$ of:

$$
\Delta E = \pu{5.87433E-6 eV}
$$

Converting to wavelength with $\lambda = hc/\Delta E$, where $h$ is the Planck constant this corresponds to a wavelength of $\lambda = \pu{21 cm}$.