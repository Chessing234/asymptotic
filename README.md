# asymptotic

Lean 4 library for asymptotic analysis utilities used in the [teorth](https://github.com/teorth) ecosystem.

## Build

Requires [Lean 4](https://leanprover.github.io/lean4/doc/setup.html) matching `lean-toolchain` (currently Lean 4.5.0-rc1).

```bash
lake update
lake build
```

Mathlib is fetched automatically via `lake-manifest.json` on first build.

## Layout

- `Asymptotic/` — library modules (`discretize`, `majorize`, `sum_approx_integral`, …)
- `Asymptotic.lean` — root module imported by `lake build`
- `Temp/` — experimental scratch files (not part of the default build target)
