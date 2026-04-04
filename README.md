# OpEngine.jl

Operator-partitioned numerical solver — ODE + IMEX/PDE operator splitting.

## Overview

`OpEngine.jl` is a Julia port of
[ACCIDDA/op_engine](https://github.com/ACCIDDA/op_engine) (Python). It provides
a numerical solver that decomposes dynamical systems into operator-partitioned
components, supporting:

- Standard ODE integration
- IMEX (implicit-explicit) splitting
- PDE operator splitting

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
