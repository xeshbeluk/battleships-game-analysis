# Battleship Simulation & Strategy Comparison

This project simulates the classic game of Battleship in R, using three different ship placement strategies:
- **Random**: Ships are placed randomly on a 10x10 board.
- **Wolf**: Ships are placed using a pre-defined pattern favoring clusters.
- **Edge**: Ships are placed mostly along the board's edges.

A smart shooting algorithm is used in all three cases. It switches from random shots to focused targeting when a ship is hit.

## Features
- Enforces legal ship placement (no overlap, spacing around ships).
- Monte Carlo simulation of 1000 games per strategy.
- Statistical analysis using ANOVA to compare efficiency (shots to win).
- Visualization with histograms and boxplots.

## Files
- `play_game()` – random board placement and play
- `play_game_wolf()` – fixed board layout (wolf strategy)
- `play_game_edge()` – fixed board layout (edge strategy)
- `shoot_at_ship()` – smart shooting logic
- `is_ship_destroyed()` – checks ship destruction status
- Final analysis compares:
  - Total number of shots per strategy
  - Turn of last ship destroyed per ship length
  - ANOVA p-values and confidence intervals

## How to Run
1. Load the R Markdown file.
2. Run all chunks from top to bottom.
3. Plots and statistical summaries will be generated at the bottom.
