# Root Locus Field Guide

An interactive guide to root locus plots, built as a single static page.

**Live site:** https://seanclough.github.io/root-locus-field-guide/

## What's in it

- **Anatomy of one locus**: a labeled example with breakaway, break-in, asymptotes, departure angle and jω crossing.
- **The angle condition**: drag a test point and watch the pole and zero angles add up to 180° on the locus.
- **Rules 1–8**, each with its own plot (plus a bonus rule on the poles' center of gravity), several with tabs for more transfer functions.
- **Common shapes and edge cases**: repeated roots, breakaway points off the axis, right-half-plane poles and zeros, conditional stability, pole–zero dipoles, the 0° locus.
- **Playground**: type or paste your own transfer function (LaTeX like `\frac{K(s+2)}{s(s+4)}`, plain text like `K(s+2)/s(s+4)`, or a characteristic equation like `s^3+6s^2+8s+K=0`) and copy the current one back out as LaTeX; type an exact K next to any slider; drag poles and zeros, stack repeated roots, cancel poles with zeros, multi-select, pan (drag the background or middle-click) and zoom, rectangular or ωn/ζ grid. The panel applies every rule to whatever you build.

Every curve and number is computed from the polynomials (D(s) + K·N(s) = 0), not measured.

## Branches

- `main`: the published site.
- `design-bench`: adds a **Design bench** section (place closed-loop poles, solve for the controller and K, check the step response against %OS/Ts/Tp specs). Not published yet.

## Running locally

Open `index.html` in a browser. Fonts load from Google Fonts; everything else is in the one file.
