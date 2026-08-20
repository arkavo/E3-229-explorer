# E3-229 Quantum Mechanics Explorer

An interactive companion for building physical intuition about wave mechanics,
bound states, tunnelling, electronic bands, and lattice vibrations. The
controls connect mathematical parameters directly to wavefunctions, probability
densities, spectra, dispersion relations, and animated normal modes.

**Interactive playground:** <https://arkavo.github.io/E3-229-explorer/>

## Physics modules

### Free particle

Explore a Gaussian wave packet and free-particle dispersion,

\[
E(k)=\frac{\hbar^2k^2}{2m}.
\]

The animation illustrates phase evolution and wave-packet spreading.

### Quantum wells

Compare infinite, finite, triangular, and coupled wells:

- quantized energies and stationary-state wavefunctions;
- probability densities shown independently from wavefunction amplitude;
- degeneracy and cumulative state counting in one, two, and three dimensions;
- continuum density-of-states estimates;
- finite-barrier leakage and field-induced confinement;
- splitting of atomic levels into bands as wells are coupled.

For an infinite one-dimensional well,

\[
E_n=\frac{n^2\pi^2\hbar^2}{2mL^2},\qquad
\psi_n(x)=\sqrt{\frac{2}{L}}\sin\left(\frac{n\pi x}{L}\right).
\]

### Quantum tunnelling

Vary barrier height, width, and incident energy while comparing transmission
and reflection. For a rectangular barrier with \(E<V_0\), the evanescent scale
is controlled by

\[
\kappa=\frac{\sqrt{2m(V_0-E)}}{\hbar},
\]

which makes the exponential sensitivity to barrier width visible.

### Periodic potentials and band structure

The Kronig–Penney and coupled-well views connect discrete bound states to
allowed energy bands, forbidden gaps, and crystal-momentum dispersion. The
large-system coupled-well spectrum uses a disclosed interpolation approximation
for interior levels while retaining explicitly calculated band edges.

### Quantum harmonic oscillator

Inspect Hermite-Gaussian eigenstates and equally spaced energy levels,

\[
E_n=\hbar\omega\left(n+\frac{1}{2}\right).
\]

Wavefunction amplitude and probability density are plotted against their
corresponding energy baselines.

### Phonons

Animate normal modes of a one-dimensional alternating-spring chain, then move
to a material-specific graphene visualizer using the six-branch MC2D-71 phonon
dataset. Click a point on the \(\Gamma\rightarrow M\rightarrow K\rightarrow
\Gamma\) dispersion to animate its complex eigenvector in a repeated,
rotatable honeycomb lattice.

For a monoatomic nearest-neighbor chain,

\[
\omega(k)=2\sqrt{\frac{K}{m}}\left|\sin\left(\frac{ka}{2}\right)\right|.
\]

## Conventions and scope

- Unless otherwise labelled, plots use dimensionless model units with
  \(\hbar=1\).
- Energies, lengths, masses, and spring constants should be interpreted
  consistently within each module, not as SI values.
- Continuum state counts and densities of states are Weyl-law approximations.
- The graphene frequencies and eigenvectors are sourced from the
  [Materials Cloud MC2D-71 dataset](https://mc2d.materialscloud.org/details/mc2d-71);
  animation amplitudes are visually exaggerated.
- Numerical visualizations are intended to support physical intuition and
  tutorial discussion, not replace a converged research calculation.

## Suggested tutorial path

1. Begin with free-particle dispersion and wave-packet spreading.
2. Introduce confinement through the infinite and finite wells.
3. Connect barrier penetration to tunnelling probabilities.
4. Increase the number of coupled wells to observe band formation.
5. Compare electronic bands with phonon dispersion and normal modes.
