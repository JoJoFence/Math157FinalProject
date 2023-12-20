# How to Beat Wordle: An Optimization Approach Using Shannon Entropy, Minimax, and Frequency Analysis

## Summary
This project explores three different approaches to optimally winning Wordle: a Shannon entropy algorithm, a minimax algorithm, 
and a frequency analysis approach. The three algorithms are written in Python, as well as the helper functions to extract and analyze 
relevant data. After running each algorithm across all the possible solution words accepted by Wordle, the lowest average number of 
guesses it took to find the solution word was 4.012 for Shannon entropy, 3.610 for minimax, and 4.378 for frequency analysis, with 
starting words ”salet”, ”crane”, and ”bares”, respectively, and runtimes of 1981.27 minutes, 3.66 minutes, and 12.77 minutes, respectively. 

## Project Structure
This repo contains three Jupyter Notebooks, one each for the Shannon entropy, minimax, and frequency analysis approaches. These notebooks use
the ```data``` folder, containing ```.txt``` files of lists of five letter words (all possible words and only words accepted by Wordle). The 
```results``` folder contains ```.txt``` files of the number of guesses it took to solve Wordle for each Wordle word, and the ```figures``` folder 
contains plots generated from these results.

## Usage
To run the notebooks, first clone the repo:

```
git clone https://github.com/JoJoFence/WordleOptimizer.git
```

Next within the repo directory, open a notebook and simply run the cells to begin the Wordle solving process. You can also play Wordle yourself
within each notebook (by running ```player_run_wordle()```). **Note:** running the Shannon entropy notebook for all of the words will take a *long* 
time. I would recommend only running it for a few words if you want to test it out, or running it on a powerful machine if you want to run it
through the whole sequence of possible five letter words.

## Research Paper
If you want to learn more about the process behind this project (including the math involved for each approach), I wrote an accompanying research 
paper, located [here](https://github.com/JoJoFence/WordleOptimizer/blob/095820c5ec72d6666637e758662342591985b059/paper/JonasHansen_HowToBeatWordle_15May2022.pdf)!
