# Validations

A repository for storing and running validation scripts for the RCFTR framework, targeting **CASP16** and other benchmarks/datasets.

## Structure

```
validations/
  casp16/       # Validation scripts and results for CASP16
  others/       # Validation scripts and results for other benchmarks
scripts/        # Shared utility scripts used across validations
```

## Usage

1. Place validation scripts in the appropriate subdirectory under `validations/`.
2. Run scripts from the `scripts/` directory for shared utilities.
3. Results and outputs should be saved alongside their respective validation scripts.

## Benchmarks

| Benchmark | Directory              | Description                         |
|-----------|------------------------|-------------------------------------|
| CASP16    | `validations/casp16/`  | Critical Assessment of Protein Structure Predictions, round 16 |
| Others    | `validations/others/`  | Additional benchmark datasets       |
