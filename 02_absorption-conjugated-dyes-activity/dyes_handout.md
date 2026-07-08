# ABSORPTION SPECTRA OF CONJUGATED DYES

> [!NOTE]
> Particle-in-a-box
> 
> HOMO/LUMO of conjugated dyes
> 
> Computational Chemistry (TDDFT)
> 
> Data Analysis and Visualization
> 
> Molecular Orbital Analysis
> 
> Finite Well

## Quantum Theory Background

### Particle in a Box

<a id="Fig6-1-PIB"></a>

<p align="center">
<img src="media/Fig6-1.png" width="650">
</p>

**6.1.** V(x), Ψ(x) and Ψ2(x) for the particle in the box solutions.

The quantum mechanical problem of describing the motion of a particle confined in a one-dimensional box is the first problem encountered as we begin to wade into modern atomic and molecular theory in the first semester of Physical Chemistry. Mathematically, the particle-in-a-box (PIB) model illustrates key features of quantum theory with respect to translational motion, e.g., eigenfunctions and eigenvalues, operators, and the non-classical concepts of zero-point energy, charge localization, and quantization of energy. In the PIB model, a particle is confined to moving in the x-dimension of a box of length $L$. Inside the box, the potential, $V(x)$, is zero while outside the box, $V(x)$ is infinite (Figure [6.1](#Fig6-1-PIB)).[^1]

Schrödinger's time-independent equation for a particle confined to move in one dimension (along the $x$-axis) is:

$$
-\dfrac{\hbar^2}{2m_e} \dfrac{d^2}{dx^2} \Psi(x) + V(x)\Psi(x) = E\Psi(x)
$$

For an infinite potential well extending from $x = 0$ to $x = L$, the potential energy function is defined as:

$$
V(x) =
\begin{cases}
0, & 0 < x < L \\
\infty, & x \leq 0 \text{ or } x \geq L
\end{cases}
$$

In this case, the wavefunction $\Psi(x)$ must be zero outside the well due to the infinite potential barrier, meaning the particle has zero probability of being found outside the box. Inside the well, where $V(x) = 0$, Schrödinger's equation reduces to:

$$
-\dfrac{\hbar^2}{2m} \dfrac{d^2}{dx^2} \Psi_n(x) = E_n \Psi_n(x)
$$

Solving this second-order ordinary differential equation with boundary conditions $\Psi(0) = \Psi(L) = 0$ gives the normalized eigenfunctions and quantized energy levels ($n = 1, 2, 3, \ldots$):

$$
\begin{align}
\Psi_n(x) &= \sqrt{\dfrac{2}{L}} \sin\left( \dfrac{n\pi x}{L} \right)  \\
E_n &= \dfrac{n^2 h^2}{8mL^2} \end{align}
$$

Far from being only a pedagogical and mathematical exercise, confining a particle to moving in a 1D box has applications in predicting properties of dye molecules that can be measured. The energy levels predicted by solutions to the 1D PIB problem may be used to predict the maximum absorption wavelength, $\lambda_\text{max}$, for some chemical compounds that absorb light in the visible spectrum. Such compounds generally have delocalized electrons from either the $\pi$ electrons in a conjugated organic molecule or the odd electron in a free radical species. In this experiment, $\lambda_\text{max}$ will be determined for several conjugated dye molecules (having the general form shown in Figure [6.2](#Fig6-2-Dyes)) that absorb in the visible part of the spectrum. The measurements will be compared to predictions of $\lambda_\text{max}$ by Equation [6.4](#Eq6-4-Energy) as manipulated below. This approach is referred to in the literature as the "free-electron model."[^2]

<a id="Fig6-2-Dyes"></a>

<p align="center">
<img src="media/Fig6-2.png" width="650">
</p>

**6.2.** A conjugated dye compound with five carbons in the forming the π-electron backbone

<a id="Fig6-3-Pisystem"></a>

<p align="center">
<img src="media/Fig6-3.png" width="650">
</p>

**6.3.** The atomic orbitals forming the π-electron backbone in a conjugated dye compound with five (5) carbons.

The $\lambda_\text{max}$ of the visible spectrum may be approximated as transitions of the $\pi$ electrons between the *HOMO* (**H**ighest **O**ccupied **M**olecular **O**rbital) and the *LUMO* (**L**owest **U**noccupied **M**olecular **O**rbital) as defined in Equation [6.4](#Eq6-4-Energy). Referring to Figure [6.3](#Fig6-3-Pisystem), each carbon atom in the $\pi$-electron backbone contributes one (1) electron, the nitrogen at the left boundary contributes two electrons (sp$^3$), and the nitrogen on the right boundary (ionized) contributes one more. Thus, the total number of electrons ($M$) populating the $\pi$-molecular orbitals is given by Equation [6.5](#Eq6-5-TotalElectrons) where $p$ is the number of carbon atoms in the $\pi$-electron backbone. 

$$
M=p+3
$$

For a molecule with $M$ electrons in the conjugated system, using the standard building-up (Aufbau) principle, the $M/2$ lowest energy levels will be filled in the ground state (see Figure 6.4). The absorption of light is associated with the transition from the HOMO ($n_1 = M/2$) to the LUMO ($n_2 = M/2 + 1$) is $\Delta E$ defined in Equations [6.6](#Eq6-6-DeltaE)-[6.8](#Eq6-8-DeltaE). 

$$
\begin{align}
E_2-V-(E_1-V)=\Delta E&=\dfrac{h^2}{8m_e L^2}\times(n_2^2-n_1^2) \\
(n_2^2-n_1^2)=\bigg(\dfrac{M}{2}+1\bigg)^2-\bigg(\dfrac{M}{2}\bigg)^2&=\dfrac{M^2}{4}+M+1-\dfrac{M^2}{4}=M+1 \\
\Delta E&=\dfrac{h^2}{8m_e L^2 }\times(M+1) \end{align}
$$

<a id="Fig6-4-Pisystem"></a>

<p align="center">
<img src="media/Fig6-4.png" width="650">
</p>

**6.4.** The "building up" of the molecular energy levels for a conjugated dye compound with five (5) carbons and therefore M=8 electrons.

It is assumed that the potential energy, $V(x)$, is constant along the $\pi$-electron backbone, and that it rises sharply to the infinity at the ends. To determine the length, $L$ of the approximated one-dimensional "box," refer again to Figure [6.3](#Fig6-3-Pisystem). As a simplifying assumption, the average C-C and C-N bond distance is designated $l$. For a conjugated dye compound with $p$ carbon atoms, there are $p-1$ C-C bonds, two C-N bonds, and an additional length of one bond length on either side of the nitrogen atoms.[^3] 

$$
L = (p-1+2+2)l = (p+3)l
$$

 Substituting Equations [6.9](#Eq6-9-L) and [6.5](#Eq6-5-TotalElectrons) into Equation [6.8](#Eq6-8-DeltaE), we have the working equations for $\Delta E$ and $\lambda_\text{max}$ in terms of known constants and $p$, the number of carbons in the $\pi$-electron conjugated backbone. The literature value of the average bond distance, $l$, is 1.39 $\angstrom$.[^4] 

$$
\begin{align}
\Delta E&=\dfrac{h^2 (p+4)}{8m_e l^2 (p+3)^2} \\
\lambda_\text{max}&=\dfrac{8m_e cl^2 (p+3)^2}{h(p+4)}  
\end{align}
$$

### Computational Chemistry

r\[0pt\]0.6 ![image](Fig6-10.png){width="60%"}

Computational chemistry has advanced with the digital age, offering critical insight into chemical processes and properties that are difficult to measure experimentally. The seminal work of chemists, mathematicians, and physicists such as Erwin Schrödinger and Douglas R. Hartree, as well as Chemistry Nobel Laureates John Pople and Walter Kohn, throughout the 20th century constructed the foundation of computational chemistry long before the digital age began. In the context of the PIB experiment, calculating absorption spectra previously have utilized faster, semiempirical methods using the configuration interaction singles (CIS) method to calculate absorption spectra. However, excited state methods like time-dependent density functional theory (TDDFT) are more common to compute absorption spectra with greater accuracy.[6.10](#Fig6-10-PIBexample) shows how the 1D PIB framework maps onto (3E, 5E, 7E)-1,3,5,7,9-decapentaene. Computed molecular orbitals (MOs) visually encode the same nodal behavior and energy spacing consistent with the PIB model, illustrating how computational tools can bridge fundamental quantum models with observable molecular behavior. For a more detailed overview of computational chemistry, see Lab [11](#Lab11-CompChem).

l\[0pt\]0.6 ![image](Fig6-7.png){width="60%"}

Density functional theory (DFT) originates from the Hohenberg-Kohn theorems in 1964, an existence proof that proved that the charge density ($\rho [r]$) completely determines the electronic properties of the ground state including energy. The implementation of DFT is the development of numerous functionals that approximate the relationship between electron exchange and correlation and comes in numerous flavors, which makes picking a functional to use like darts on a dartboard---hoping to hit a bulls-eye for accuracy to experiment.

While TDDFT effectively models absorption spectra qualitatively, quantitative accuracy decreases at higher energy core-valence excitations, with errors ranging from 30-100 eV compared to typical UV-vis errors of 0.2 to 0.5 eV, largely depending on the chosen functional. To correct this underestimation, linear shifts (shifting absorption energies by the mean absolute error) and linear transformations (shifting the absorption energies via the best fit line between computed and experimental absorption energies) are techniques employed to show how TDDFT correctly predicted the lineshape of the spectra (Figure [6.7](#Fig6-7-Example)).[^6] Range-separated hybrid functionals like CAM-B3LYP and $\omega$B97X-D3 are particularly suited for absorption spectroscopy. This tier of functionals treats long-range electron interactions with a variable rate of exact exchange by correcting errors associated with vertical transition methods for absorption.

r\[0pt\]0.4 ![image](Fig6-8.png){width="40%"}

A use case for computed UV-Vis spectra is the prediction of the structure, spectroscopy, and formation mechanisms of aerosols. Coordination spheres consisting of solvent or other atmospheric gas phase particles present in the atmosphere at night can be used to simulate more realistic conditions. This example consisted of and radicals coordinated to monoterpenes. The figure on the right was contributed by Bianca Aridjis-Olivos (B.S. Chemistry '23).

### Particle in a Finite Well

The finite well model (Figure [6.9](#Fig6-9-PIBFinite)) extends the 1D infinite potential well (Figure [6.1](#Fig6-1-PIB)) by introducing finite barriers, allowing for quantum tunneling and wavefunctions that decay into the barrier regions. This results in lower, more closely spaced energy levels and offers a more realistic approximation of electron behavior in molecules. Computational chemistry techniques reinforce this connection by visualizing MOs of the 3D geometry (Figure [6.10](#Fig6-10-PIBexample)), which leads to an estimation of the effective box length and well depth. Rendering MOs in the context of a finite well also helps illustrate how the well depth limits the number of bound states, highlighting where the particle-in-a-box approximation breaks down and higher energy orbitals begin to resemble unbound or delocalized states. By combining these computational insights with the finite well model, we will use the finite well approximation as a predictive tool for absorption spectra. Figure [6.9](#Fig6-9-PIBFinite) shows the general solutions to the wavefunctions within each region (I, II, and III).

<a id="Fig6-9-PIBFinite"></a>

<p align="center">
<img src="media/Fig6-9.png" width="650">
</p>

**6.9.** Schematic and Wavefunction for the particle in a finite well model.

Consider a particle in a finite well model where 

$$
\begin{align}
k_0 &= \sqrt{\dfrac{2m_e}{\hbar}(V_0-E)}\\
k_1 &= \sqrt{\dfrac{2m_eE}{\hbar^2}}
\end{align}
$$

To determine the energy eigenvalues from the wavefunction, we begin the derivation where $\Psi_\text{I}(x)$ and $\Psi_\text{II}(x)$ must follow the boundary conditions at x=0, i.e., $\Psi_\text{I}(0)=\Psi_\text{II}(0)$ and $\Psi'_\text{I}(0)=\Psi'_\text{II}(0)$. 

$$
\begin{align}
Ae^{k_0(0)} &= Bsin(k_1*0)+Ccos(k_1*0)\\
Ak_0e^{k_0(0)} &= Bk_1cos(k_1*0)-Ck_1sin(k_1*0)\end{align}
$$

By solving the system of Equations [6.15](#Eq6-15-Psi1-0) and [6.16](#Eq6-16-Psi2-0), 

$$
\begin{align}
C&=A\\
B&=A\frac{k_0}{k_1}\end{align}
$$

At x=L, the system of equations containing $\Psi(L)$ and $\Psi'(L)$ is 

$$
\begin{align}
De^{-k_0L} &= Bsin(k_1L)+Ccos(k_1L) \\
De^{-k_0L} &= Bk_1cos(k_1L)-Ck_1sin(k_1L)\end{align}
$$

 By multiplying Equation [6.19](#Eq6-19-Psi2-L) by $k_0$ and using Equations [6.17](#Eq6-17-C) and [6.18](#Eq6-18-B), 

$$
\begin{align}
Dk_0e^{-k_0L} &= A\dfrac{k_0^2}{k_1}sin(k_1L)+Ak_0cos(k_1L) \\
Dk_0e^{-k_0L} &= -A\dfrac{k_0}{k_1}k_1cos(k_1L)+Ak_1sin(k_1L))\end{align}
$$

 By equality, Equations [6.21](#Eq6-21-Psi2-L) and [6.22](#Eq6-22-Psi3-L) may be solved for the quantity $Dk_0e^{-k_0L}$ 

$$
\begin{align*}
\dfrac{k_0^2}{k_1}sin(k_1L)+k_0cos(k_1L) &= -k_0cos(k_1L)+k_1sin(k_1L)\\
k_0^2sin(k_1L)+k_1k_0cos(k_1L) &= -k_1k_0cos(k_1L)+k_1^2sin(k_1L)\\
2k_1k_0cos(k_1L) &= (k_1^2-k_0^2)sin(k_1L)
\end{align*}
$$

 

$$
2k_1k_0 = (k_1^2-k_0^2)tan(k_1L)
$$

 By substituting $k_0$ and $k_1$ into Equation [6.23](#Eq6-23-FE), 

$$
2\bigg(\dfrac{2m_eE}{\hbar^2}\bigg)\sqrt{E(V_0-E)} = \bigg(\dfrac{2m_eE}{\hbar^2}-\dfrac{2m_e(V_0-E)}{\hbar^2}\bigg)tan\bigg(\sqrt{\dfrac{2m_eEL^2}{\hbar^2}}\bigg)
$$

 

$$
\dfrac{2\sqrt{E(V_0-E)}}{2E-V_0} = tan\bigg(\sqrt{\dfrac{2m_eEL^2}{\hbar^2}}\bigg) 
$$

 The values of $E$ where the two quantities in Equation [6.24](#Eq6-24-FE) are equal correspond to the energy levels of the finite well. These functions can be plotted in Python to determine the allowed values of $E$ for a given potential depth $V_0$ and box length $L$ by solving the roots. The fsolve function in Python is useful for this purpose, but any equivalent numerical root solver in Excel would suffice. For this experiment, $V_0$ is determined by finding the range of orbital energies containing the $\pi$ orbitals of the conjugated region inside the box. More details on doing this analysis will be provided in the next section. From there, the wavelength of the $\pi$-$\pi^*$ transition can be calculated.

### Discussion Questions

1.  Based on your experimental results, make a general statement about the accuracy of the free-electron model. Include a table containing the theoretical $\lambda_\text{max}$ from the free-electron model, the theoretical $\lambda_{MAX}$ from the finite well, the computed $\lambda_\text{max}$ from TDDFT, and the experimental $\lambda_\text{max}$. Include the $\Delta_{95}\lambda$ and %-error calculated by Equation [6.12](#Eq6-12-PercentError).

    

$$
\text{ error}=\left|\frac{\text{theoretical}\ \lambda_\text{max}-\text{experimental}\ \lambda_\text{max}}{\text{theoretical}\ \lambda_\text{max}}\right|\times100
$$

2.  Discuss sources of systematic error that might give rise to the % error in $\lambda_\text{max}$ that you observe. Use the resources provided in Brightspace (and footnoted herein) for this discussion. Proper citation is required.

3.  As discussed in class, the finite well model is the next step in complexity from the PIB model. How does the finite well PIB model correspond to the conjugated dyes? What is the effect of well depth on the calculated absorbance wavelengths? Did using the finite well model improve your results from the theoretical $\lambda_\text{max}$ calculated from the infinite well?

    1.  How did the Python code used for the finite well model work? What did the code do? These two questions can go into the **Procedure** section if the text flows better there.

4.  Based on your spectra, account for the observed colors of the dyes.

5.  Which orbitals were responsible for the transition that corresponds to $\lambda_\text{max}$?

6.  Are there other features in your experimental spectra that the TDDFT results can identify? If so, how would you go about identifying those?

7.  What causes peak broadening in spectroscopy? Why do computed spectra return vertical lines rather than a broad spectra? *Hint: Consider Heisenberg's Uncertainty Principle and the chapters on spectroscopy (covered in CHE 3332).*


[^1]: Patel, P. In *Engaging Students in Physical Chemistry, Volume 2; ACS Symposium Series*; **2025**; 261278.

[^2]: W. Jensen, O. Schmidt, J. Platt. "The Free-Electron Model," ACS Symposium Series; American Chemical Society (2013): 117-137.

[^3]: Hans Kuhn, "A Quantum-Mechanical Theory of Light Absorption of Organic Dyes and Similar Compounds", *J. Chem. Phys.*, **1949**, *17*, 12, 1198

[^4]: David P. Shoemaker, Carl W. Garland, and Joseph W. Nibler, Experiments in Physical Chemistry, 5th ed. (New York: McGraw-Hill, 1989), 442.

[^5]: Xu, J.; Kim, Y. L.; Khurana, R.; Havenridge, S.; Patel, P.; Liu, C. In *Ann. Rep. Comput. Chem.*; Wilson, A. K., Ed.; Elsevier, 2024; Vol. 20, pp 157187. <https://doi.org/10.1016/bs.arcc.2024.10.006.>

[^6]: Patel, P. et al., *J. Phys. Chem. C.* **2022**, *126*, 11949-11962. <https://doi.org/10.1021/acs.jpcc.2c02049.>
