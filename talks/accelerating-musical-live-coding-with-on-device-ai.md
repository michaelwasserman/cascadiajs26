# Accelerating Musical Live Coding With On-Device AI 

## Alex Hinson
### Fleetio, Chattanooga, TN USA 
- [Speaker's Notes (Placeholder)]()
- [Post-conference YouTube Recording (Placeholder)]()
## Abstract: 

Let's explore a human-centric approach to live coding music. By fusing Strudel REPL with on-device AI via WebGPU and Wasm, we create an "intelligent scaffolder" that handles boilerplate syntax locally, keeping the performer in their flow state without losing agency.
## Community talk notes: 

### Scribe: Mike Wasserman
- Fun start with live music coding
- Strudel: make music with code, small community
- AI to help translate ideas into tooling for making music (layer on top of Strudel)
  - modifying sound with natural language edits that resolve in transforms in code
- Running locally in browser, with small on-device model
  - cost: stays free
  - latency: beats round trip to frontier model
  - privacy: input never leaves the browser, runs offline
- How do you get a small model good at a niche domain?
  - Picking a kind of model on task types, (not around a domain like JS / Strudel)
    - HF Transformers.JS task types, wide variety, lots of candidates
    - Translations (english language to Strudel)
    - Text Generation made the most sense
  - Next: Designing I/O for model to fit app
    - Take off-the-shelf model and ask for code
      - code is not fitting Strudel language
    - Try having model produce structured intent (JSON) then convert that into Strudel code
      - good solution for some projects, can work for this
      - Then every Strudel command needed translation in this layer, grew and lots to maintain
      - Latency for structured output was slow, lots of tokens 
    - Try fine-tuned structured output
      - Need lots of training data
      - Removed lots of project code, because now model generates executable code
      - Smaller token output, but less enforced correctness
      - Training did what the engine used to do
  - Training data
    - Hand curated examples would be ideal, but intractible
    - Tried LLM generated samples; again plausible confident nonsense; can't train on that
    - Added validation pipeline step - ensure output code parses, etc.
    - Validate first and then scale; avoid confident hallucinations
  - Grounding
    - Add documentation of strudel to model context
    - Include related abstract reasoning content for grounding
  - Ongoing loop of retraining
    - Fix errors, gaps, overfitting, 
    - Model continually gets better at translating ideas into Strudel
  - Making it small enough
    - started with 1.5B param model, loads quick enough and capable, but need to shrink
    - quantization trades a bit of output quality for speed and shrinking
    - Transformers JS helped
- Overall Pick task, shape the io (model/code boundary), train the model, ship it small
- Applicable to other projects in other domains
- bit.ly/cascadia-ai-music
