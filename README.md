# setup-lean

This action provides functionality for provisioning the [Lean theorem prover](https://lean-lang.org/) within GitHub actions.

More specifically, it can handle:

  * Installing [elan](https://github.com/leanprover/elan), the preferred / community supported tool for managing and installing Lean versions, and thereby any version needed by a specific project
  * Installing a specific version (toolchain) of Lean and adding it to the PATH
  * TODO: Installing / caching downloaded caches
  * TODO: Registering problem matchers for error output

## Basic usage

See [action.yml](action.yml)

```yaml
steps:
- uses: actions/checkout@v4
- uses: actions/setup-lean@v1
- run: lake build
```
