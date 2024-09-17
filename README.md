# Flappy Bird NEAT AI

This project is a Flappy Bird clone, implemented in Python using the Pygame library and a neural network trained with NEAT (NeuroEvolution of Augmenting Topologies). The AI birds learn to play the game and improve over generations through evolutionary principles.

## Description

In this project, multiple birds are controlled by neural networks that evolve using the NEAT algorithm. Each bird attempts to navigate through pipes by learning from its previous generations. The birds' movements are based on the output of the neural network, and their fitness is evaluated based on how far they progress in the game.

Key Features:
- Pixel-perfect collision detection.
- NEAT-powered AI that learns to play Flappy Bird through neuroevolution.
- Visualization of the game window and AI performance.

## Installation

### Requirements
- Python 3.x
- Pygame
- NEAT-Python

### Steps to Install
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/flappy-bird-neat.git
    ```

2. Navigate to the project directory:
    ```bash
    cd flappy-bird-neat
    ```

3. Install the required dependencies:
    ```bash
    pip install pygame neat-python
    ```

4. Download or prepare the `imgs` folder with the game assets (background, bird, pipe, and base images).

## Usage

1. Make sure you have the `config-feedforward.txt` NEAT configuration file in the same directory as the script.

2. Run the game:
    ```bash
    python3 flappy_bird_neat.py
    ```

3. The AI will start playing the game, and the birds will evolve over generations.

### How the Game Works:
- **Score**: The score increases as the birds pass through pipes.
- **Fitness**: Birds with higher fitness survive longer and pass on their genes to the next generation.
- **Generations**: When all birds die, a new generation is spawned with improved neural networks.

## Configuring NEAT

The NEAT algorithm's behavior is controlled by the `config-feedforward.txt` file. You can modify various parameters like population size, mutation rates, and more.

For example, to adjust the population size, open `config-feedforward.txt` and modify the `pop_size` parameter:

## References 
The code is highly referenced from Tech with Tim https://github.com/techwithtim/NEAT-Flappy-Bird