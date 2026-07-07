# Paraxial Ray Bending — interactive

A single-page, interactive explainer of how **paraxial ray bending** works, built around the Paraxial Ray Trace Equations:

- **bending:** `n′·u′ = n·u − y·φ`
- **transfer:** `y′ = y + u′·t`
- **power:** `φ = (n′ − n)·C`,  `C = 1/R`

Three interactive demos:
1. **Bending at one surface** — drag the ray or type values; watch a ray refract and see the equation update live, in reduced-slope (n·u) language. Presets for the vertex ray, the flat plane, negative power, and glass→air; plus a "make the ray leave parallel" challenge.
2. **Bend → transfer → bend** — step through a two-surface trace by hand: bend, fly the gap, bend, fly to the axis. The gap has an adjustable index n, so with n > 1 it is a real **thick lens**: BFD ≠ EFL, the principal plane H′ appears on the plot, and the result is checked against Eq 4.18 (1/EFL = φ₁ + φ₂ − (t/n)·φ₁φ₂). Presets: thin lens (t = 0: powers add), thick lens (n = 1.5), afocal telescope.
3. **Why all rays meet at one image** — a fan of rays from an on-axis object through a thin lens. Pick "your ray" height Y and watch the PRTE crossing −Y/u′ stay put for every Y; the Gaussian formula is then *derived* by cancelling Y, not decreed.

Accessible: keyboard-operable ARIA tabs, labelled sliders, live-region readouts, WCAG-AA colors, touch-friendly drag handles that don't trap page scrolling, print stylesheet.

Grounded in Joseph M. Geary, *Introduction to Lens Design* (with practical ZEMAX examples), Chapter 4 — "Paraxial World" (Figs. 3.1, 4.4, 4.8; Eqs. 4.1, 4.2, 4.4, 4.18).

## Use it

Live demo: **https://maksimbulatov.github.io/paraxial-ray-bending/**

Or just open `index.html` in any browser — it is one self-contained static file with **no dependencies** and **no build step**.

## License

MIT — free for anyone to use, share, and adapt.
