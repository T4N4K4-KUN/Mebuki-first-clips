# Build Better Apps with AI Using This One Simple Document (PRD Guide)

Source: https://youtu.be/MZjW7mlRgdw
File: `Build Better Apps with AI Using This One Simple Document (PRD Guide).mp3`
Status: user-provided script from source; use for structure analysis

## Transcript

### [0:00] Introduction: The Problem with Vibe Coding

Host:
Vibe coding is cool until it's not. If you don't have documentation to feed your AI co-pilot, you're going to have a hard time and you're definitely going to need to start over at least once. In this video, I want to show you a simple solution: creating a product requirements document, or PRD. Feed the PRD to your AI co-pilot, whether it's Bolt, Cursor, or Claude Code, and you're going to get much better results.

### [0:45] Creating the PRD with Claude

Host:
The first thing I do is open up Claude, specifically Sonnet, because I think it's just better. I ask it to help me create a PRD for an Astro blog that is SEO optimized with a dark color scheme. I tell it the tech stack will be Astro, Netlify for deployment, and PocketBase for the back end. I also list features like an admin dashboard, a newsletter form, and proper permalinks. One reason I prefer Sonnet over models like Gemini is that it just does the work while asking clarifying questions, rather than expecting me to do a bunch of stuff first.

### [2:15] Reviewing the PRD

Host:
So it finishes writing the PRD, and we have our goals, tech stack, architecture, and core features. But the most important part is the database schema. The database schema is how you can stay consistent if you switch from Bolt to Cursor; you need a single source of truth so the AI knows how the database works. Otherwise, it's a real hassle to solve later.

### [3:30] Testing Bolt vs. Claude Code

Host:
Now, just for fun, I'm going to pop this PRD into Bolt and Claude Code to see what does a better job faster. I tell Bolt to build the blog following the specs. Meanwhile, I start Claude Code in the terminal. Bolt starts building quickly and creates a modern Astro blog with a fun purple dark style. I click deploy, and it deploys straight to Netlify successfully. It even made the admin panel, getting a lot done with just a couple of prompts.

### [5:00] Debugging Claude Code Deployment

Host:
On the other hand, Claude Code faces some issues. When I try to deploy it to Netlify, it fails. First, it looks like a dependency problem, and then I realize the folder infrastructure is causing issues. But one thing I love about Claude Code is how agentic it is. It moves the files to the root directory to fix the deployment on its own. Finally, we get it published.

### [6:30] Conclusion & Outro

Host:
Overall, I would say Bolt did a better job here and got more done in less time. But I have a hunch that the database implementation might be easier with Claude Code. I'm moving farther away from Cursor these days because I can get so much done on $20 a month with Claude Code instead of spending over $200 a month on Cursor. If this was helpful, hit that subscribe button, and check out the command line bootcamp link below, especially if you want to try Claude Code. See you in the next video, peace.

## Extracted Learnings

- Without documentation, AI-assisted coding becomes unstable and may require restarts.
- A PRD can be fed to AI tools such as Bolt, Cursor, or Claude Code.
- The PRD functions as a shared specification across tools.
- Clarifying questions are useful because they reduce the amount of up-front work by the human.
- Goals, tech stack, architecture, core features, and database schema are treated as PRD components.
- The database schema is framed as a single source of truth.
- The same PRD can be tested across multiple AI coding agents.
- AI agents may still fail at deployment, but agentic tools can diagnose and modify project structure.

