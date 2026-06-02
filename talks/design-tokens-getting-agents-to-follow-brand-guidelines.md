# Design Tokens: Getting Agents to Follow Brand Guidelines 

## Kaelig Deloumeau-Prigent
### Design Tokens W3C CG, Seattle, WA USA 
- [Speaker's Notes (Placeholder)]()
- [Post-conference YouTube Recording (Placeholder)]()
## Abstract: 

While AI allows us to ship more UI than ever, it also makes it easier to ship experiences that don't match our design language. Let's see how Design Tokens, the lingua franca of design systems, bridge the gap between design, engineering, and AI.
## Community talk notes:

### Scribe: Mike Wasserman
- Adding buttons with AI; design intent translated into bad impls 
  - Doesn't quite fit branding or layout, missing state or dark mode support
  - Give AI design system toolbox of reusable components
  - Design system can't do everything, always use cases that you can't satisfy
  - Dropdown example
- How do we store design decisions?
  - catalog with names and descriptions
  - want all languages/impls to respect a single source of truth
- "Design Tokens" format module spec and Community Group
  - JSON schema - name, type, when to use, value
  - Global tokens, Component (menu, card) tokens, relationships between each
  - Getting AI agents to use this source of truth with skills, mcp, etc.
  - AI plan/code/verify loops
- Join the fight against UI slop
