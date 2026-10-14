# Latent Factor Explorer

An interactive toy model for teaching exploratory factor analysis. Two latent factors generate three observed variables; the page shows the raw data as a rotating 3D scatter plot and the recovered factor solution as a 2D plot of factor scores with loading vectors.

Everything runs in the browser. There is no build step and no server-side code: open `index.html` directly, or serve the folder from any static web host.

## What you can change

- **Generating model**: the six loadings, the factor correlation φ, and the sample size (up to 3,000).
- **Factor distribution**: normal (an elliptical cloud), sparse (an X), or sparse and non-negative (two "horns"), with a prevalence slider and a choice of how severity is spread among cases where a factor is present.
- **Analysis**: principal axis factoring or principal components; no rotation, varimax, promax or oblimin (direct quartimin, the default); optional matching of estimated factors to the true ones.
- **View**: colour points by either true factor, and optionally show the common-factor plane, each point's distance to it, the factor directions in the 3D plot and the variable loadings in the 2D plot.

## Presets

- **Psychosis and mania (rare)**: schizophrenia spectrum and bipolar mania as rare, non-negative factors, measured by negative symptoms, elevated mood and delusions (which load on both). Prevalence is inflated to 4% so each horn has enough points.
- **Child behaviour problems**: internalising and externalising problems, measured by emotional symptoms, conduct problems and irritability.
- Four loading patterns with normal factors.

## Notes

With three indicators and two factors the model has −2 degrees of freedom, so the factor solution is not unique; principal axis factoring often produces Heywood cases.

The only external resource is the IBM Plex font family from Google Fonts; the page falls back to system fonts without it.
