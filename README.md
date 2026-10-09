# ⚽ World Cup Prediction — Ensemble Model

> 🚧 **Work in progress.** Built step by step; each step is a notebook in [https://github.com/chilukuru-saikrishna/world-cup-prediction/tree/main/notebooks](notebooks/).

An ensemble model that forecasts international football matches and simulates the FIFA World Cup. It combines three different approaches, each with its own strengths, and runs the full tournament thousands of times with Monte Carlo simulation to estimate each team's chances.

## Approach

| Component | What it captures |
| --- | --- |
| **Elo ratings** | Overall team strength, updated after every match |
| **Dixon-Coles model** | Each team's attacking and defensive strength, with goals modelled as Poisson and a correction for low-scoring results |
| **Neural network (PyTorch)** | Non-linear patterns across features such as form, rating gaps and venue |
| **Ensemble + Monte Carlo** | Combines the three, then simulates the tournament many times |

## Progress

| Step | Notebook | Status |
| --- | --- | --- |
| 1 | [Data exploration & cleaning](notebooks/01_data_exploration.ipynb) | ✅ Done |
| 2 | Elo ratings from scratch | ⏳ Next |
| 3 | Dixon-Coles Poisson model | ⬜ Planned |
| 4 | Neural network (PyTorch) | ⬜ Planned |
| 5 | Ensemble & evaluation against baselines | ⬜ Planned |
| 6 | Monte Carlo tournament simulation | ⬜ Planned |

## Data

Historical men's international results from the open [martj42/international_results](https://github.com/martj42/international_results) dataset. The notebooks download it automatically; no data is stored in this repo.

## How to run

Open any notebook in [Google Colab](https://colab.research.google.com) (**File → Open notebook → GitHub**, then paste this repo's URL) and run the cells in order.

## Tech stack

Python · pandas · NumPy · SciPy · Matplotlib · PyTorch

## Author

**Saikrishna Chilukuru** — Physics M.Sc., moving into data science. [GitHub profile](https://github.com/chilukuru-saikrishna)
