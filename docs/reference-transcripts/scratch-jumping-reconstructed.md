# How to Make a Jumping Game in Scratch

Source URL: https://youtu.be/1jHvXakt1qw
Channel: Scratch Team
Official status: official Scratch Team tutorial
Audio/subtitle file: local/candidate_subtitles/scratch-jumping.en.vtt
Transcript source: user-provided reconstructed script based on source content

## Important Note

This is not treated as a verified verbatim transcript.
Use for structure analysis.
For exact quote work, use `local/candidate_subtitles/scratch-jumping.en.vtt`.

## Reconstructed Script

| Time | Section | Speaker | Text |
|---:|---|---|---|
| 0:00 | Introduction | Zoe | Hi everyone, it's Zoe from the Scratch team, also known as Zindia. Today I wanted to show you how to make a jumping game in Scratch. By the end of this tutorial, you'll be able to make a game where you can have a character jumping over moving obstacles. We'll do this in five steps: make your character jump, make a moving obstacle, stop the game, add more obstacles, and keep score. Let's get started. |
| 0:30 | Step 1: Make Your Character Jump | Zoe | First, let's pick a character and make it jump. I will pick the chick, and let's also choose a backdrop—I'll use the blue sky. To make the character jump upwards, we can use the "change Y by 10" block, and if we make it repeat 10 times, it'll go up really high. To make it come back down, we change Y by -10 and put that in a repeat loop too. Let's add the "when space key pressed" block on top so it jumps with the space key, and add a "start sound chirp" block to enhance the jump. |
| 1:15 | Step 2: Create a Moving Obstacle | Zoe | Next, let's make a moving obstacle. I'll pick the egg, and set its size to 80 so it's a bit smaller than your character. We want the egg to start at one side of the screen and glide over to the other side. We can use the "go to X and Y" block to tell the egg exactly where to start, and then use the "glide to XY" block to make it smoothly cross the screen. We can put this in a forever loop that starts when we click the green flag, and make the egg take 3 seconds to glide so it's not too fast. |
| 2:30 | Step 3: Game Over & Bug Fix | Zoe | Next, let's make the game stop if we run into the egg. We can use the "stop all" block and have the egg wait until it's touching the chick to stop the game. Oh, and let's fix a problem where the chick sometimes gets stuck in the air when its code is stopped. We can fix this by making the chick go to a starting position when the game starts by dragging out a "go to" block under the green flag. |
| 3:15 | Step 4: Adding More Obstacles | Zoe | To make our game even more fun, let's add more obstacles. Just right-click on the egg and click duplicate. Because they have the exact same code, let's make the second egg wait 1 second before it starts gliding so they are spaced out. We'll also make it hide when the project starts and show once it's done waiting. |
| 4:00 | Step 5: Keeping Score & Outro | Zoe | Lastly, let's add a score. In Scratch, you can use a variable to keep track of a certain number, so I'll make a variable called "score". Every time the player manages to complete a jump, we can increase their score by one, and when the project restarts, we can set their score back to zero. There we go, that's a jumping game! You could try adding multiple kinds of obstacles or changing the backdrop when the player reaches a certain score so it's like level two. I can't wait to see all the things you make. I'll see you next time, and scratch on! |

## Structure Extraction

| Time | Structure |
|---:|---|
| 0:00 | Opens with the game type and promises what the learner can make by the end. |
| 0:00 | Breaks the game into five concrete behaviors: jump, moving obstacle, stop game, more obstacles, score. |
| 0:30 | Starts by choosing a character and backdrop, giving the learner ownership. |
| 0:30 | First interaction is visible: press space to jump. |
| 1:15 | Adds one moving obstacle with controlled speed. |
| 2:30 | Adds game-over logic, then immediately fixes a bug. |
| 3:15 | Adds more obstacles by duplicating existing work, not starting over. |
| 4:00 | Adds score and suggests extensions such as more obstacle types or level-like backdrop changes. |

## 001 Relevance

Useful for 001:

- Start with what the learner will make.
- Break the game into visible actions, not abstract concepts.
- Character/background choice creates ownership.
- A bug appears and is fixed as part of normal making.
- After the base game works, extensions are suggested.

Not useful for 001:

- Exact Scratch block instructions.
- Full five-minute step-by-step tutorial.
- Scratch-specific UI or block names.

001 should borrow the structure:

```text
You will make this.
It moves.
It avoids/shoots/catches.
It has one rule.
It can be extended after it works.
```
