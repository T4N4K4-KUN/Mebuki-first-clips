# How to Make a Catch Game in Scratch

Source URL: https://youtu.be/7NN5v2wSL4U
Channel: Scratch Team
Official status: official Scratch Team tutorial
Audio/subtitle file: local/candidate_subtitles/scratch-catch.en.vtt
Transcript source: user-provided reconstructed script based on source content

## Important Note

This is not treated as a verified verbatim transcript.
Use for structure analysis.
For exact quote work, use `local/candidate_subtitles/scratch-catch.en.vtt`.

## Reconstructed Script

| Time | Section | Speaker | Text |
|---:|---|---|---|
| 0:00 | Introduction | Zoe | Hi everyone, it's Zoe from the Scratch team, also known as Zineia. Today I wanted to show you how to make a catch game in Scratch. A game where objects are falling from the sky and you catch them to score points. We'll break this into five steps: move the catcher, make your object go to the top, fall down, catch it, and keep score. Let's get started. |
| 0:30 | Step 1: Move the Catcher | Zoe | First, let's pick the character or object that you want to be catching things, like the bowl, and let's add a backdrop, too. I'll use the boardwalk. We want the bowl to be able to move side to side with the arrow keys, so we can use the "change X by 10" block to make the bowl go this way. We can use an "if then" block to make the bowl change X by 10 if the right arrow key is pressed. To make sure it's always checking if the key is pressed, we can just put this inside a "forever" loop. To make the bowl go to the left, instead of changing X by 10, we can change X by -10 if the left arrow key is pressed, and put this in the forever loop, too. |
| 1:45 | Step 2 & 3: Go to the Top and Fall Down | Zoe | Next, let's pick the object that we want to be falling, like the apple. At the beginning of the game, we want the apple to start at a random place at the top. If we make the apple go to a random position and then set Y to 180, it goes to a random place, but then Y is always set to be at the top. To make our apple fall down, we can put in a negative number to change Y inside a forever loop, so it'll keep falling till it hits the bottom. To make it go back to the top when it hits the bottom, we can check if the Y position of the apple is less than -170. If it is, we just put a copy of that same code to make it go back up to the top. |
| 3:15 | Step 4: Catch It | Zoe | Now let's make it so that we can actually catch the apples instead of them just falling through the bowl. This is another good time for an "if then" block. We can use the block that tests if the apple is touching the bowl. If the apple is touching the bowl, we want it to go back to the top. Let's put this inside a forever loop, and let's make it play a sound when we catch it. Nice! |
| 4:20 | Step 5: Keeping Score & Outro | Zoe | Lastly, let's add a score so that you get points for every apple you catch. We can make a variable called "score" and use it to keep track of how many points we've scored. We can put the "change score by one" block here, so every time we catch the apple, the score increases by one. And when the game starts, let's set the score to zero so it resets. There we go, that's a catch game! I love catch games because they can be any type of game; you could be catching pieces of trash to keep an ocean clean or a pet could be catching treats. I'm so excited to see all the things you make. Well, I'll see you next time, and scratch on! |

## Structure Extraction

| Time | Structure |
|---:|---|
| 0:00 | Opens with the exact game type and a one-sentence rule: falling objects are caught for points. |
| 0:00 | Breaks the game into five concrete behaviors: move catcher, object top, fall down, catch, score. |
| 0:30 | Learner chooses catcher and backdrop, creating ownership. |
| 1:45 | Learner chooses falling object and uses random top position, making repeatable play. |
| 3:15 | The core interaction is introduced: catch instead of falling through. |
| 4:20 | Score creates a visible reward loop. |
| 4:20 | The same game pattern can become many themes, such as cleaning ocean trash or pet catching treats. |

## 001 Relevance

Useful for 001:

- Explain the game in one sentence.
- Break the game into five visible behaviors.
- Let the learner choose objects/background to own the result.
- One base mechanic can become many themes.
- Score/reward loop makes the result feel like a game.

Not useful for 001:

- Exact Scratch block instructions.
- Full step-by-step tutorial.
- Scratch-specific UI or block names.

001 should borrow the structure:

```text
This is the game.
Here is the one rule.
It has a few visible behaviors.
You can choose the look.
Once it works, you can change the theme.
```
