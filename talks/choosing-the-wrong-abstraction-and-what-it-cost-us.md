# Choosing the Wrong Abstraction (And What It Cost Us) 

## Darius Cepulis
### Mux, Oak Park, IL USA 
- [Speaker's Notes (Placeholder)]()
- [Post-conference YouTube Recording (Placeholder)]()
## Abstract: 

We chose the wrong abstractions and had to throw out our most important component. Oops. This talk unpacks how a well-meaning API collapsed under real-world use, and why composable APIs scale better than configuration-heavy ones, across UI and deeper systems.
## Community talk notes: 

### Scribe: Mike Wasserman
- Mux player: simple video player control where feature requests made it harder
- Throwing away control now, what went wrong
- Material UI - can get unweildy when design diverges from the daefaults
- Base UI - revise attributes to control props; styling via CSS classes
- "What Makes Software Good?" Mike Bosdock(?)
- Chart.JS (vending machine, hope they've got it) vs D3 (stove, make your own pasta)
- What is the right abstraction?
  - Confgurable APIs: express what you want from a bunch of options (toy truck)
  - Composable APIs: independent parts, stack/assemble as needed (Lego Technic)
    - Great examples of composable APIs
    - Output type matches input type
    - Let users build something themselves without waiting on you
- Composition is all you need Fernando Rojo
- Composable APIs aren't free; higher upfront cost but plateaus over time; configuration costs contiually rise over time
- How to lower the cost: good docs, examples, platform idioms, good defaults, discoverability, consistency, errors that teach, types
- Provide an abstraction ladder (layers of abstraction): Visual editor, declarative marks, data binding primitives, JS/Canvas/SVG, WebGL Shaders
  - Example: D3 -> Observable Plot (users can step down to D3 parts encapsulated within)
  - Offer escape hatches to access underyling primitives for more power
  - shadcn -> BaseUI -> HTML CSS
- We can vibe code this... NYT "Coding after coders"
- Differences in AI productivity increases:
  - Brownfield (10% boost to established codebases)
  - Greenfield (20x boost)
- Example decepulis/ax-bench
- Good DX is usually good AX
  - start from there, agents build on human understanding
- Now building Video JS 10 to replace Mux Player (way more composable, escape hatches, smaller bundle size)
- Exchange config for flexibilty - get out of the way and let users build without waiting for you
