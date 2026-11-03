# MathLanguage

The scripting language of [MathCraft](https://github.com/ACSquaredS/MathCraft), an open-source, MATLAB-inspired numerical computing environment.

> **Status:** Proposed. The repository is not created yet and implementation has not started.

## Role in MathCraft

MathLanguage is the layer users write code in. It turns MathCraft scripts into calls to the numerical, symbolic, statistical and visualization modules.

## Architecture

- **Python surface.** The user-facing API, the package users import, and integration with the Python ecosystem. Python is the first language to be supported.
- **Rust core.** Parser, evaluator and the performance-critical execution paths. Compiled to a native extension and exposed to Python.
- **Binding.** [PyO3](https://pyo3.rs) for the Python-Rust interface, built and packaged with [maturin](https://www.maturin.rs).

Recommended versions to start: Python 3.10 or newer, stable Rust.

## Depends on

- [MathCore](https://github.com/ACSquaredS/MathCore) for shared types
- [MathNumerical](https://github.com/ACSquaredS/MathNumerical), [MathSymbolic](https://github.com/ACSquaredS/MathSymbolic), [MathStatistics](https://github.com/ACSquaredS/MathStatistics) and [MathVisualization](https://github.com/ACSquaredS/MathVisualization) as backends for calls made from scripts

## Planned scope

- Grammar and parser for the MathCraft script syntax
- Evaluator with variables, functions and matrix operations
- Python package with a stable public API
- Error messages that point to the line and column in the script

## Getting started

Not available yet. This section will be filled in with the first release.

## Contributing

Contribution guidelines will be published in the [MathCraft](https://github.com/ACSquaredS/MathCraft) umbrella repository. Until then, open an issue to discuss a change before sending a pull request.

## License

Released under the [MIT License](LICENSE).
