# Runtime Conditions

> [!IMPORTANT]
> Runtime Conditions is currently seeking adoption by an established parent
> project. The repositories in this organization are split for hands-on
> usability, review, demos, and implementation feedback. They are not intended
> to present Runtime Conditions as a standalone foundation or competing project.

Start here: https://runtimeconditions.github.io/

## What Runtime Conditions Is

Runtime Conditions Profiles are portable, machine-readable declarations of the
external runtime integrations required by one workload. A profile describes
demand: APIs, caches, datastores, configuration inputs, SDK-discovered
dependencies, and extension-defined runtime requirements. Platforms and
adapters decide how to fulfill that demand.

The current goal is to make the model concrete enough for feedback from
ecosystems such as Score, Backstage, Dapr, CNCF platform tooling, service
catalogs, policy systems, and platform engineering teams.

## Repository Map

- `runtimeconditions.github.io` - public reader guide and entry point.
- `spec` - core specification drafts, whitepaper, guides, and draft examples.
- `extensions` - first-party Runtime Conditions extension definitions and
  declaration packages.
- `go-rc-profiler` - Go Runtime Conditions profile generator and extension
  validation tooling.
- `java-rc-profiler` - Java Runtime Conditions profiler/generator.
- `python-rc-profiler` - Python Runtime Conditions profiler/generator.
- `rc-demos` - runnable demo apps, catalog fixtures, and platform adapter demos.
- `ebpf-rc-profiler` - legacy/experimental runtime observation profiler.

## Navigation

New readers should start with the public guide, then move to the spec and demos:

1. Start here: https://runtimeconditions.github.io/
2. Read the core spec draft in `runtimeconditions/spec`.
3. Review the first-party extensions in `runtimeconditions/extensions`.
4. Try the runnable workflows in `runtimeconditions/rc-demos`.
