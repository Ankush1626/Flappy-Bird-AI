# Flappy-Bird-AI

<div align="center">
<img src="https://github.com/Ankush1626/Flappy-Bird-AI/blob/main/Flappy%20Bird%20AI.gif" align="center" style="width: 100%" />
</div>  

Note - Required python modules are pygame and neat-python.

This code is for a Flappy Bird game where an AI learns to play the game using the NEAT algorithm. Here's a detailed explanation:

1. **Game Overview**:
   - This code creates a Flappy Bird game where an AI, using the NEAT algorithm, learns to control the bird to avoid pipes and achieve the highest score possible.

2. **Bird Mechanics**:
   - The bird can jump and fall, with its movement controlled by physics-based calculations. The bird’s image rotates as it moves, simulating the look of flying or diving.

3. **Pipes and Obstacles**:
   - Pipes appear at random heights and move horizontally across the screen. The bird must fly through the gaps between the pipes to stay alive.

4. **Scrolling Background**:
   - The ground scrolls continuously to give the illusion of forward movement. The game has a repeating background and base image.

5. **AI Control with NEAT**:
   - The NEAT algorithm evolves neural networks that control the bird's movement. Each bird’s neural network decides when to jump based on its environment.
   - The AI learns by trial and error, with successful birds (those that navigate the pipes well) having a higher chance of passing on their traits to the next generation.

6. **Fitness and Scoring**:
   - Birds earn points by passing through pipes, and their fitness score increases the longer they survive.
   - The fitness score is used to determine which birds' neural networks will be used to create the next generation.

7. **Game Loop**:
   - The game runs in continuous loops, where the AI-controlled birds try to survive as long as possible. If a bird crashes into a pipe or the ground, it’s removed from the game.

8. **Evolution Process**:
   - The game uses a configuration file to set up the NEAT algorithm. The AI birds improve over multiple generations by evolving better neural networks that can navigate the pipes more effectively.
