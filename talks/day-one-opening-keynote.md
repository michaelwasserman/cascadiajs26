# Day One Opening Keynote 

## Matt Biilmann
### Netlify, San Francisco, CA USA 
- [Speaker's Notes (Placeholder)]()
- [Post-conference YouTube Recording (Placeholder)]()
## Abstract: 
AX, Agent Experience
Building products for agents

## Community talk notes:

### Chapter I
Netlify objective - Turn imagination into reality
Discussion of how JavaScript is one of the languages that help create the magic of the web.

Progression breakdown of AI assistance and agents within driving vehicles, to having AI autonomy.

"""The whole stack changes when the driver is no longer human"""
Timelapse of autocomplete within the IDE to building with an AI agent to describe ideas and supervise the development to using AI assistance. Shifting the "build vs buy" equation.

We will see a lot of shift happening in how things are developed.
Referencing OpenClaw.ai, autonomous coding agents, and making the comparison to self-driving cars.
While autonomous cars make us rethink cities, autonomous agents make us rethink our platforms, virtual cities, products and more.

### Chapter II - Agent Experience
Today - AX is critical for infra and dev tools
Tomorrow: your products wont' succeed without it

Before UX (User Experience) was coined by Don Norman, the interaction with the UI was not seen as an experience.
DX - Developer Experience coined by Jeremiah Lee Cohick
AX - Agent Experience
Covering the experience that agents will have as they work with a product or platform.

### How to AX?
It's about understanding how agents experience your product.

*Four pillars:*
1. Access
- Can the agent access your product?
- Does your agent have the correct permissions?
For Netlify, they've added netlify.ai that provides two different experiences for humans vs bots. For bots, markdown files are provided instead of the marketing website.
Agent Auth is an emerging standards to facilitate access to different products. 
2. Context
- Does the LLM know about your product?
Provide docs as context. Shipping a Markdown variant of every page is cheaper to read, easier to parse and friendlier to LLM context windows.
Model Context Protocol (MCP) - Focusing on context to expose what your product knows in an universal format as UI for LLMs.
API vs MCP - Same product, different surfaces
3. Tools
- Are you building your product for agents?

Every product has an Agent Experience, but is it good?
A good developer experience doesn't necessarily mean a good agent experience.
For Netlify CLI, by adding a response that indicates how to use the product without interaction, AX improves by providing an alternative route.

4. Orchestration
Agents are launchable from your product
Working in AI-native environments to allow aysnc agents to work autonomously.

### The Road Ahead
"""As agents become autonomous and our whole team become builders, we need to reshape every part of our developer platforms"""
Netlify provided Axis, an open-source framework developed to rate the agent experience.

### Scribe: Mike Wasserman
- Turn imagination into reality 
- AI Assistance hels us do more
  - supervising car driving instead of manually driving
  - looking forward to autonomy
  - changes how we think about commuting, rethink surrounding infra
- Copilot in the IDE came after driving assistance - some minor help
- Then build with an AI agent - describe an idea and agent builds for you
  - Universal hands-free
- AI Assistance lets us do much more
  - can fundamentally change what companies do
  - unlocking software development resources in other departments
- From Assistance to Autonomy
  - Openclaw owns a computer and interacts with you
  - Live demo of using a selfie to update presentation
- Autonomous cars make us rethink cities
  - Autonoms agents make use rethink our work
- Expands the population of who is a builder
  - Big impact on Netlify
- AX (Agent Experience)
  - Today: is crtiical for infra nad dev tools
  - Tomorrow: your products won't exceed without it
- How to AX: Prompt -> Agent Loop -> Goal
  - Agent loop is: llms <-> context + tool calls <-> your product
  - Access, Context, Tools, Orchestration
- Access:
  - Bot Gmail account blocked for being a bot
  - netlify.ai: for humans and agents (humans get instructions, agents get markdown)
  - Netlify database - service for agents 
  - self-auth UUID for agents
- Context:
  - Docs as context; offer markdown variants of every page
  - Header requests markdown
  - MCP: UI for LLMs; universal way to expose context
  - Skills: steering the context of the agent
  - API vs MCP - same product different surfaces
- Tools:
  - Netlity has 100 Endpoints; would overwhelm agent
  - instead offer 5 tools via MCP
  - Agents use your product regardless; without AX, it's just a bad experience
  - Iterated on Netlify CLI - initially bad UX; helped with simmple mode
- Orchestration:
  - Offering agent workflows in products you use; better integrations
  - Async agents working autonomously
- As agents become autonomous and the whole team becomes builders, need to reshape every part of our developer platforms 
- Axis.run - open source project to automate agents testing your product
- Thank you slide was updated by agent, woohoo!
  
