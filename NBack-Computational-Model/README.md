# N-Back Computational Model — Course

Five lessons building from exponential decay buffers to fMRI regressors.

## Rendering

Each lesson is a self-contained HTML file with all resources embedded.

```bash
cd course/
quarto render lesson_*.qmd
```

Each produces a standalone `.html` file you can open in any browser or upload individually.
To render a single lesson: `quarto render lesson_01_memory_buffer.qmd`

## Dependencies
```bash
pip install numpy scipy pandas plotly
```
Quarto: https://quarto.org/docs/get-started/

## Lesson map

| Lesson | Core concept | Scripts connected |
|---|---|---|
| 1 | Exponential decay buffer, δ, μ | `nback_model.py` (buffer + activation) |
| 2 | Probit decision, β, σ, trial types | `nback_model.py` (compute_trial_signals) |
| 3 | Lure interference, normalisation, α, correction | `nback_model.py` (full) |
| 4 | MLE, parameter transforms, AIC, model comparison | `03_fit_model.py` |
| 5 | fMRI regressors, z-scoring, FSL format | `04_regressors.py` |
