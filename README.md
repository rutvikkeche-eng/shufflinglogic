# Weighted vs Random Ordering Visualizer

This project explores different ways of shuffling brands in sponsored carousels. 
The core idea behind the weighted model is that not every item needs to have the same likelihood of appearing first. Instead, items can be assigned different weights, which expand or shrink their probability ranges during sampling. A random number is then generated and mapped against these ranges to determine which item wins Position 1. Once the first position is selected, the remaining positions are reconstructed using the original weight hierarchy so the ordering remains stable and intentional rather than continuously re-randomized at every step.

The visualizer exposes the complete sampling process, including configured probabilities, generated random numbers, active sampling ranges, and long-run convergence against expected probabilities through repeated simulations.

The project also includes a toggle for a pure random shuffle mode, where every item has equal probability for every position and every permutation is equally likely.

Demo - https://rutvikkeche-eng.github.io/shufflinglogic/
