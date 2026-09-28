# @inzumer/tsconfig

Shared TypeScript configurations for Inzumer projects. Part of the Inzumer shared packages (one repository per package:
`inzumer-<name>` published as `@inzumer/<name>`).

## Install

```sh
pnpm add -D @inzumer/tsconfig
```

## Usage

```jsonc
// tsconfig.json
{ "extends": "@inzumer/tsconfig/react-library" }
```

| Entry                             | For                                                                                     |
| --------------------------------- | --------------------------------------------------------------------------------------- |
| `@inzumer/tsconfig/base`          | Strict ES2022 base: `strict`, `noUncheckedIndexedAccess`, `exactOptionalPropertyTypes`… |
| `@inzumer/tsconfig/react-library` | React libraries and apps (DOM libs, `react-jsx`)                                        |
| `@inzumer/tsconfig/node`          | Node scripts and tooling (`types: ["node"]`)                                            |

## Releases

[Changesets](https://github.com/changesets/changesets): add a changeset (`pnpm changeset`) with each
change. On `main`, `.github/workflows/release.yml` opens a "Version Packages" PR and, when it is
merged, publishes to npm (needs the `NPM_TOKEN` repository secret).

Previously @inzumer/tsconfig (private, in ui-library).
