# research-kit

The research surface: the analysis framework and the API wrappers that feed
it. One clone with `--recursive` brings the whole research toolchain onto a
new machine.

## What is here

| Submodule | What it does | Installs as |
|---|---|---|
| `otter` | econometrics: regressions, diagnostics, forecasting, and paper-ready result tables | `otter`, [on PyPI](https://pypi.org/project/otter/) |
| `fred-loader` | readable names over the FRED API instead of raw series codes | `fred-loader` |
| `census-loader` | readable names over the US Census APIs instead of raw variable codes | `census-loader` |

All three are installable Python packages. The loaders fetch and name public
data; `otter` does the econometrics on it.

## Clone

```
git clone --recursive https://github.com/iasolb/research-kit.git
```

An existing clone picks up the submodules with
`git submodule update --init --recursive`.

## Where this is going

The long-term aim is that this stops being three separate libraries with a
folder around them and becomes one coherent toolkit: good enough at the
things it covers to be the preferable option for that work, rather than a
wrapper you reach past. That is a direction, not a plan with a date.

## Start here

Open `otter` first: it is the econometrics core the two loaders feed. The naming
convention is `<domain>-kit`; the sibling surfaces are
`dev-kit` (editor and tooling config), `cloud-kit` (syncing between
machines), `data-kit` (validation, checks and transforms), and `ai-kit`
(the AI tooling umbrella).
