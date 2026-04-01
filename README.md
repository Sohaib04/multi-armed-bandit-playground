# Multi-Armed Bandit Playground

**A Product Experimentation Simulator**

A production-quality, research-grade simulation environment for comparing multi-armed bandit algorithms in realistic product experimentation scenarios — such as testing homepage designs, pricing strategies, or feature rollouts.

## What This Project Does

This notebook simulates and compares five bandit algorithms across diverse experimental conditions:

| Algorithm | Strategy | Best For |
|---|---|---|
| **Epsilon-Greedy** | Random exploration at rate ε | Simple, controlled exploration |
| **Optimistic Initial Values** | Start optimistic, converge naturally | Cold-start scenarios |
| **UCB1** | Explore uncertain arms | Deterministic, no randomness needed |
| **Thompson Sampling** | Bayesian posterior sampling | Production rollouts, best overall |
| **Sliding-Window TS** | Windowed posterior for drift | Non-stationary environments |

## Key Questions Answered

- Which algorithm maximizes cumulative reward?
- Which converges fastest?
- Which minimizes regret?
- Which is safest for real product rollout?
- How do different traffic volumes impact performance?
- What happens under non-stationary reward distributions?

## Quick Start

```bash
# Clone the repository
git clone https://github.com/<your-username>/multi-armed-bandit-playground.git
cd multi-armed-bandit-playground

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook notebook.ipynb
```

## Project Structure

```
multi-armed-bandit-playground/
├── notebook.ipynb        # Main notebook — all code, analysis, and visualizations
├── requirements.txt      # Python dependencies
├── README.md             # This file
├── .gitignore            # Git ignore rules
└── outputs/              # Auto-generated plots and CSV exports (gitignored)
```

## Tech Stack

- **NumPy** — numerical computation
- **Matplotlib** — visualization
- **SciPy** — statistical analysis
- **ipywidgets** — interactive exploration

No external bandit libraries — everything is implemented from scratch.

## License

MIT License — feel free to use, modify, and share.
