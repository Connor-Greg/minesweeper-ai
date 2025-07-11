# Minesweeper AI Agent

This is a logic-based AI agent that plays Minesweeper using propositional logic and inference.

Originally developed as part of Harvard's CS50AI course. All implementation and logic for the AI agent were written by me. Starter code structure was provided by the course and is used here under fair use for educational portfolio purposes.

## Files

- `minesweeper.py`: The starter code provided the game logic (`Minesweeper` class), but I implemented the full AI system from scratch, including:

  - `Sentence` class:  
    Represents a logical statement like "these 3 cells contain 2 mines". Handles known safe/mine deduction and updates based on new information.

  - `MinesweeperAI` class:  
    Stores known safe/mine cells, updates a knowledge base, and makes inferences to select moves. Implements:
    - Knowledge updating logic
    - Inference through subset relationships
    - Decision-making for safe/random moves

- `runner.py`: Used to run a visual version of the game (provided by CS50AI, minimally modified).
- `requirements.txt`: Python dependencies.

## What It Does

- Represents the game as a knowledge base of logical sentences.
- Infers new safe moves or mines using logical inference rules.
- Plays the game without guessing, when possible.
