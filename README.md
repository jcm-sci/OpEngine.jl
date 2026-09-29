# OpEngine.jl

[![jcm-sci](https://img.shields.io/badge/jcm--sci-jcmacdonald.dev-blue)](https://jcmacdonald.dev/projects/)

> [!IMPORTANT]
> **Inactive design scaffold.** This repository does not currently provide a
> usable Julia package or public API. Its source module and tests are
> placeholders, and the package is not registered in Julia's General registry.

## Current implementation

The maintained implementation is the Python
[ACCIDDA/op_engine](https://github.com/ACCIDDA/op_engine) package, with
documentation at [accidda.github.io/op_engine](https://accidda.github.io/op_engine/).

## Repository purpose

This repository is retained as a possible starting point for a future Julia
port. There is no active development timeline. Do not depend on it for
research or production work.

## Development

```bash
julia --project=. -e 'using Pkg; Pkg.instantiate()'
just test
```

## License

MIT
