# Function Lab

A static scientific calculator and interactive calculus graphing workbench. It runs in the browser and can be published directly with GitHub Pages.

## Features

- Scientific expression evaluation with trigonometric, logarithmic, exponential, and other common functions.
- Symbolic first derivatives, Simpson-rule definite integrals, numerical limits, and sign-changing root search.
- Interactive 2D function plots with adjustable x-range, zoom, pan, and an optional derivative overlay.
- Recent evaluation history saved in the browser.

Expressions use Math.js syntax. Use `x` as the variable, `^` for powers, and functions such as `sin(x)`, `sqrt(x)`, and `log(x)`. Trigonometric functions use radians.

## Publish with GitHub Pages

1. Create a GitHub repository and push these files to its `main` branch.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then save.
4. Open the Pages URL shown in the settings after deployment completes.

The site is static; no build step or server is required. Math.js, Plotly.js, and the fonts load from CDNs, so visitors need an internet connection.

## Numerical notes

Definite integrals use composite Simpson’s rule with 2,048 intervals. Limits are estimated from nearby samples. Root search detects sign changes, so roots that only touch the x-axis may be missed. These numerical tools are estimates, not computer-algebra proofs.