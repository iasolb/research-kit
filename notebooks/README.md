# Notebooks

Two tracks. Start at the top of the one that describes you.

## Start here

For someone who has seen pandas once, or not at all, and wants to get from
nothing to a real answer about real data. Nothing is assumed except that you can
run a notebook.

| | |
|---|---|
| [`01-get-set-up.ipynb`](01-get-set-up.ipynb) | Install the three libraries, get two free API keys, and pull your first series. Ends with a chart of something true. |
| [`02-your-first-question.ipynb`](02-your-first-question.ipynb) | Turn a vague thought into a question data can answer, run one regression, and read the output line by line. |

## Going further

For someone partway through a degree, comfortable with pandas, taking or about
to take econometrics. These use all three libraries together, because that is
the point of them.

| | |
|---|---|
| [`03-two-sources-one-question.ipynb`](03-two-sources-one-question.ipynb) | FRED and Census answer different halves of one question. Joining them is where most of the real work lives. |
| [`04-is-the-difference-real.ipynb`](04-is-the-difference-real.ipynb) | How big a sample you need before you start, whether a difference is real, and how much of your answer is noise. |

## Why this exists

Most library documentation shows you the library. These show you a piece of
work, and the library happens to be how it gets done. If you finish one and
remember the question rather than the function names, that is the right outcome.

The examples these replaced were four scripts that each demonstrated one
module. They were accurate and nobody learned anything from them.

## Running them

```bash
pip install otter fred-loader census-loader jupyterlab
jupyter lab
```

Both loaders need a free API key, which the first notebook walks through. No
paid service is involved anywhere in these.
