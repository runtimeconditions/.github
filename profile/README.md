# Runtime Conditions

Start here: https://runtimeconditions.io/

## What Runtime Conditions Is

Runtime Conditions Profiles are portable, machine-readable declarations of the
external runtime integrations required by one workload. A profile describes
demand: APIs, caches, datastores, configuration inputs, specific hardware,
and extension-defined runtime requirements. Platforms and adapters decide
how to fulfill that demand.

## Navigation

New readers should start with the public guide, then move to the demos and spec:

1. Start here: https://runtimeconditions.github.io/
2. Install the [CLI](https://github.com/runtimeconditions/rc-cli) found in `runtimeconditions/rc-cli`.
3. Review the [available extensions](https://github.com/runtimeconditions/extensions/tree/main/catalog) and [extension tooling](https://github.com/runtimeconditions/extensions/tree/main/tooling/extension-bindings) in `runtimeconditions/extensions`.
4. Try the [runnable workflows](https://github.com/runtimeconditions/rc-demos) in `runtimeconditions/rc-demos`.
5. Read the [latest spec draft](https://github.com/runtimeconditions/spec/blob/main/docs/sixth-draft.md) in `runtimeconditions/spec`.

## Repository Map

### Getting started:

- `runtimeconditions.io` - public reader guide and entry point.
- `spec` - core specification drafts, whitepaper, guides, and draft examples.
- `extensions` - first-party Runtime Conditions extension definitions and
  declaration packages.
- `rc-demos` - runnable demo apps, catalog fixtures, and platform adapter demos.

### For developers:

- `rc-cli` - command line tool for working generating profiles from code bindings
- `go-rc-profiler` - Go Runtime Conditions profile generator and extension
  validation tooling.
- `java-rc-profiler` - Java Runtime Conditions profiler/generator.
- `python-rc-profiler` - Python Runtime Conditions profiler/generator.
- `ts-rc-profiler` - TypeScript Runtime Conditions profiler/generator.
- `rust-rc-profiler` - Rust Runtime Conditions profiler/generator.

### For platform engineers:

- `runtime-conditions-crd` - the Kubernetes Custom Resource Definition for deploying profiles as a custom resource
- `rc-admission-webhook` - extension validator for the profile CRD
- `rc-extension-resolver` - extension resolution library used by the admission webhook
- `backstage-plugin` - helper tooling for Backstage to aid in working with profiles and condition fulfillments
- `headlamp-plugin` - Headlamp support for Runtime Condtions resources in Kubernetes
- `api-conditions-adapter` - example platform adapter for interacting with the RC CRD and Backstage 

### Ongoing efforts and research:

- `extension-registry` - navigable UI for browsing extensions and their docs in the browser
- `white-paper-artifacts` - inputs used to compose the CNCF white paper regarding the Runtime Conditions Spec
- `service-operations-inventories` and `sdk-authorship-discovery` - part of the ongoing research into supporting SDKs as sources of condition generation
- `ebpf-rc-profiler` - legacy/experimental runtime observation profiler.

### Support and tooling repos:

- `homebrew-tools` - defines the cask used in Homebrew installations for the CLI
- `packages` - defines the installation instructions for apt/yum installations for the CLI
- `.github` - organizational documents and settings
- `runtimeconditions.github.io` - GitHub Pages site repo
- 