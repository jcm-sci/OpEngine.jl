# OpEngine.jl

[![jcm-sci](https://img.shields.io/badge/jcm--sci-jcmacdonald.dev-blue)](https://jcmacdonald.dev/software/)

Operator-partitioned solver for composing heterogeneous subsystem solvers into a single time-stepping pipeline.

## Overview

`OpEngine.jl` is a Julia port of
[ACCIDDA/op_engine](https://github.com/ACCIDDA/op_engine) (Python). It composes
heterogeneous subsystem solvers into a unified pipeline, supporting:

- ODE integration
- IMEX (implicit-explicit) splitting
- PDE operator splitting
- Stochastic and hybrid schemes

## Status

**Pre-alpha.** Port in progress.

## Related Packages

| Package | Description |
|---------|-------------|
| [op_engine](https://github.com/ACCIDDA/op_engine) | Original Python implementation |
| [OpSystem.jl](https://github.com/jcm-sci/OpSystem.jl) | System specification compiler (input to OpEngine) |
| [ModelCriticism.jl](https://github.com/jcm-sci/ModelCriticism.jl) | Model evaluation framework (downstream consumer) |

## Installation

```julia
using Pkg
Pkg.add("OpEngine")
```

## Development

```bash
julia --project=. -e 'using Pkg; Pkg.instantiate()'
just test
```

## License

MIT
