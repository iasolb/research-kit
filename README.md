# research-kit

The research surface: the analysis framework and the API wrappers that feed
it. One clone with `--recursive` brings the whole research toolchain onto a
new machine.

## What is here

| Submodule | What it does | Installs as |
|---|---|---|
| `ResearchFramework` | regressions, forecasting, and result output for papers | `research-framework` |
| `FRED_Loader` | readable names over the FRED API instead of raw series codes | `fred-loader` |
| `Census_Loader` | readable names over the US Census APIs instead of raw variable codes | `census-loader` |

All three are installable Python packages as of 2026-08-21, verified by
installing each into a clean virtual environment and importing every public
name.

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

Open `ResearchFramework` first: it is the analysis core the two loaders
feed. The naming convention is `<domain>-kit`; the sibling surfaces are
`dev-kit` (editor and tooling config), `cloud-kit` (syncing between
machines), `data-kit` (validation, checks and transforms), and `ai-kit`
(the AI tooling umbrella).
