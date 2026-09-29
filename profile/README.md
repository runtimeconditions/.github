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

## Navigation

New readers should start with the public guide, then move to the spec and demos:

1. Start here: https://runtimeconditions.github.io/
2. Try the [runnable workflows](https://github.com/runtimeconditions/rc-demos) in `runtimeconditions/rc-demos`.
3. Deploy the [Backstage plugin](https://github.com/runtimeconditions/backstage-plugin) found in `runtimeconditions/backstage-plugin`.
4. Read the [latest spec draft](https://github.com/runtimeconditions/spec/blob/main/docs/sixth-draft.md) in `runtimeconditions/spec`.
5. Review the [available extensions](https://github.com/runtimeconditions/extensions/tree/main/catalog) and [extension tooling](https://github.com/runtimeconditions/extensions/tree/main/tooling/extension-bindings) in `runtimeconditions/extensions`.

## Repository Map

### Getting started:

- `runtimeconditions.github.io` - public reader guide and entry point.
- `rc-demos` - runnable demo apps, catalog fixtures, and platform adapter demos.
- `spec` - core specification drafts, whitepaper, guides, and draft examples.
- `extensions` - first-party Runtime Conditions extension definitions and
  declaration packages.

### For developers:

- `go-rc-profiler` - Go Runtime Conditions profile generator and extension
  validation tooling.
- `java-rc-profiler` - Java Runtime Conditions profiler/generator.
- `python-rc-profiler` - Python Runtime Conditions profiler/generator.

### For platform engineers:

- `runtime-conditions-crd` - the Kubernetes Custom Resource Defition for deploying profiles as a custom resource
- `rc-admission-webhook` - extension validator for the profile CRD
- `rc-extension-resolver` - extension resolution library used by the admission webhook
- `api-conditions-adapter` - example platform adapter for interacting with the RC CRD and Backstage 

### Ongoing efforts and research:

- `white-paper-artifacts` - inputs used to compose the CNCF white paper regarding the Runtime Conditions Spec
- `service-operations-inventories` and `sdk-authorship-discovery` - part of the ongoing research into supporting SDKs as sources of condition generation
- `ebpf-rc-profiler` - legacy/experimental runtime observation profiler.
