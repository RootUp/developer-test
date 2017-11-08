# Smarterly Developer Test

This test can be conducted in any language, but PHP would be preferred. Once complete add @waxim as a collaborator on your private repository here on GitHub. The repo must be private to avoid other applicants from seeing your code.

Email: tech@smarterly.co.uk of you require more information.

## Test
You must write a game with the following rules.

### Game Rules
 - This game is played spin by spin.
 - Each spin of the game will select a bee at random.
 - Each spin will attempt to hit a bee with a success rate that averages at 0.9
 - When a bee is hit it will cascade the rules relevant to the bee type.
 - When a bee is missed, you are stung and lose 3 health points.
 - You start the game with 100 health points, when reach 0 health points you are dead.
 - If you die before all the bees, the bees win.
 - If the bees die before you, you win.
 - The game is over when there is a winner.

### Bees Rules
 - There are three bee types, each with the following rules.
   - Queen Been
     - The Queen Bee has a lifespan of 100 health points
     - When the Queen Bee is hit she loses 8 health points
     - When the Queens health points reach 0 she is dead, and so are ALL other bees of ALL other types.
     - There is only one Queen Bee
   - Worker Bee
     - The Worker Bee has a lifespan of 75 health points
     - When the Worker Bee is health it loses 10 health points
     - When the worker bee's health points reach 0 it is dead.
     - There are 5 worker bees
   - Drone Bee
    - The Drone Bee has a lifespan of 50 it points.
    - When the drone bee is health it loses 12 hit points.
    - When the Drone Bee's health points reach 0 it is dead.
    - There are 8 Drone Bees.

### Gameplay Rules
This game must be playable in the command line with the following API and responses. The file should be called `beesinthetrap`

`new` - starts a new game.

`restart` - restarts a game at any points.

`status` - lists information about the current game, our health, bees living and dead and their health.

`hit` - in game play it performs a spin of the game and returns a result.

`autoplay` - This will run a whole game, outputting step by step results to the console until there is a winner.

This is just a sample output but the game should play like so, feel free to be creative though.

```
$ beesinthetrap new

New game started. There are 14 Bees. Use hit to try and kill them.
> hit

Missed! You lose 3HP you have 97HP remaining.
> hit

Hit! You hit the Queen Bee, she has 92HP remaining.
> hit

# More moves here.

Hit! You killed the queen. You have won. Cogratulations.

$
```
