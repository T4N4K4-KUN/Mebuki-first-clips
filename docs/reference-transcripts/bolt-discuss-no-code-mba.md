# Bolt's new feature: plan and debug projects without wasting tokens

Source URL: https://youtu.be/d8JTs12rxT0
Channel: No Code MBA
Official status: non-official tutorial
Audio file: local/audio/Bolt's new feature_ plan and debug projects without wasting tokens.mp3
Transcript source: user-provided transcript

## Alternate Source File

File name: `Bolt's new feature_ plan and debug projects without wasting tokens (1).mp3`
Transcript source: user-provided transcript

## Transcript

| Time | Section | Speaker | Spoken text |
|---:|---|---|---|
| 0:00 | Introduction | Host | In this video, you're going to see how to use the discuss feature in Bolt, how it works, how it can save you time and tokens, and search the internet to bring more context into Bolt. And in doing so, we're going to build a to-do list app like Things 3. I know it's another to-do list app, but we will add AI functionality to break down a task and give you step-by-step instructions. But the main purpose of this video is showing you this new discuss feature that Bolt has, so let's get into it. |
| 0:40 | Building the Basic App & Discuss Mode | Host | I'm just going to say, "I want to build a simple to-do list app like Things 3". Okay, so we have our basic app here. If I click "add task," type "go to the gym," and click "add tasks," there we go, it is added. Now I want to show you the discuss feature. This discuss feature allows you to plan out tasks in Bolt before actually doing it, which should save you tokens because you don't have to go back and forth as much. I think one message in discuss equals 10 messages in actual build mode. Let's say I want to add a feature to drag tasks up or down to move the order. Let's plan it out in discuss mode. Now it's coming up with a plan for this, and then I'm going to click "implement the plan". With discuss mode, it is a lot more likely to do it successfully on the first try because it creates a plan before actually building it out. |
| 2:20 | Integrating AI & Web Search | Host | The next thing I want to do is add AI into this app. Something else that discuss has, which is really great, is it can search the internet and get information. I'm going to say, "I want to integrate OpenAI into this app and add a button to press on the task which will give me a breakdown of how to successfully complete the task". I'll tell it to research the OpenAI API documentation of how to integrate it. So first it researches the documentation, and now it's coming up with a plan based on all of that. Here on the top, we can see the sources that it looked at, which happened really quickly. |
| 3:45 | Connecting Supabase and API Keys | Host | Now I'm going to get out of discuss mode and say, "execute on the above plan" because I want the agent to do it for us. It just asked me to connect to Supabase, which is going to be needed for that OpenAI connection. I'm going to say, "let's fully implement the AI feature now that Supabase is connected". It's saying to set the OpenAI key in my Supabase secret. The way you get to that is through edge functions and then to secrets, and this is where we're going to add our API key. Let me add a task like "cook a chicken dinner" and click the little light bulb, which I'm assuming is the AI, but nothing is happening. |
| 5:10 | Debugging with Discuss Mode | Host | I'm going to say, "added the API key, clicked the light bulb in the UI, but nothing happened". I'm going to do the discuss mode again to see if it's able to see what's happening. So, it's giving me a plan, and then I'll say "debug this please" out of discuss mode. Okay, so at least we made some progress, but now it says "failed to fetch". Let's discuss the problem first, come up with a plan, and attempt the fix again. Let's try the light bulb again. There we go, generating breakdown! So now it worked correctly, and we got a cool breakdown. |
| 6:30 | Outro | Host | That's the main thing I wanted to show in this video: how to use this new discuss feature in Bolt to search the internet, help you debug things, and build without using as many tokens. If you like this video, be sure to like and subscribe to our YouTube channel. Click the link in our description to go to noode MBA to learn more about building with noode and AI tools. We have dozens of in-depth tutorials, and if you have any questions, leave a comment below. Thanks for watching! |

## Fact Extraction

| Time | Fact |
|---:|---|
| 0:00 | The video demonstrates Bolt's discuss feature. |
| 0:00 | The video builds a Things 3-like to-do list app and adds AI functionality to break down a task into step-by-step instructions. |
| 0:40 | The initial prompt is "I want to build a simple to-do list app like Things 3". |
| 0:40 | A basic app is generated and a task can be added. |
| 0:40 | Discuss mode is described as planning tasks in Bolt before actually doing them. |
| 0:40 | The host uses discuss mode to plan drag-and-drop task ordering, then clicks "implement the plan". |
| 2:20 | Discuss can search the internet and get information. |
| 2:20 | The host asks it to research OpenAI API documentation before planning integration. |
| 3:45 | The host asks the agent to "execute on the above plan". |
| 3:45 | Supabase connection and OpenAI API key setup are required. |
| 5:10 | The AI feature initially fails when clicking the light bulb. |
| 5:10 | The host uses discuss mode to debug, then asks "debug this please". |
| 5:10 | After another fix attempt, the feature works and generates a breakdown. |
| 6:30 | The host summarizes the feature as searching the internet, helping debug, and building while using fewer tokens. |

## 001 Usable Structure

| Element | Evidence time | Use for 001 |
|---|---:|---|
| say what you want first | 0:40 | 001 can show a direct natural-language request before any code. |
| working basic app appears early | 0:40 | The first proof should be a simple working thing, not a roadmap. |
| plan before build | 0:40 | Keep for later clips, not the first hook. It is too procedural for 001. |
| research docs and sources | 2:20 | Useful for later "AIに聞いていい/検索していい"; not main 001. |
| debug loop | 5:10 | Useful for later error/log clips; avoid in 001 because the hook is "作れる". |

## Notes

- This is not an official Bolt.new clip.
- This video is more useful for later clips 004/006 than for 001.
- For 001, only use the high-level pattern: plain request -> basic working app appears.

## Alternate Transcript Notes

The alternate transcript confirms the same structure with slightly different segmentation:

| Time | Confirmed detail |
|---:|---|
| 0:00 | The host starts by saying they will build a to-do list app like Things 3 and add AI functionality for step-by-step instructions. |
| 0:00 | The initial request is "I want to build a simple to-do list app like Things 3". |
| 0:00 | Once ready, the basic app can add tasks such as "go to the gym" or "clean my room" with a due date. |
| 1:10 | Discuss mode plans tasks before building and then the host clicks "implement the plan". |
| 1:10 | The drag-and-drop feature works after implementation. |
| 2:30 | Discuss mode can search the internet and research OpenAI API documentation. |
| 2:30 | The host exits discuss mode and says "execute on the above plan". |
| 3:50 | Supabase is needed for the OpenAI connection; the OpenAI key is set in Supabase secrets. |
| 3:50 | The first light-bulb test does nothing. |
| 5:15 | The host reports the failure, uses discuss mode to plan, asks "debug this please", hits "failed to fetch", then discusses and fixes again. |
| 5:15 | The feature eventually generates the breakdown successfully. |
| 6:40 | The closing summary says discuss can search the internet, help debug, and build while using fewer tokens. |

## 001 Decision From Alternate Transcript

Use for 001:

- simple natural-language request first
- basic working app appears early
- user can interact with the generated app

Do not use for 001:

- discuss mode
- token saving
- OpenAI API docs research
- Supabase/API key setup
- failed-to-fetch debugging

Those belong to later clips about AI interaction, debugging, and returning from errors.
