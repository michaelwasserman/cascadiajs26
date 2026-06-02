# Unlocking AI's Hidden Connections With Graphs 

## Nyah Macklin
### Neo4j, San Francisco, CA USA 
- [Speaker's Notes (Placeholder)]()
- [Post-conference YouTube Recording (Placeholder)]()
## Abstract: 

When AI agents have to execute complex, multi-hop reasoning across interconnected knowledge domains, traditional Retrieval-Augmented Generation (RAG) systems fail. Although vector-based retrieval is very good at finding content that is semantically similar, it cannot find meaningful connections between data, which leads to hallucinations. In this talk, we'll dive into how engineers can ground agents and large language models (LLMs) to uncover connections in data that are often missed by conventional RAG techniques
## Community talk notes: 

### Scribe: Mike Wasserman
- Trouble connecting I/O from different agents; production breakages
- Agents are making real decisions
- Agents miss implicit connections (e.g. approve credit increase for person with a sanctions watchlist employer)
- Building RAG piplines that miss connections; want transparency into AI black box
- example of apple, vector view, and knowledge graph view
- knowledge graph is fusion of info understandable for machine and people
- vector views: proximity in vector space
- knowledge graphs, visible connections with more than one hop of connections
- add to your vector retrieval pipeline to get better results
- knowledge graph - organized representation of entities and their relationships
- SQL vs Cypher syntax for lookup of the credit request info
- Text similarity finds docs with similar meaning
- Structureal similarity finds entities with similar connections
- tracability with AI agents
- The missing "Why?": No memory, no audit trail, no shared learning
- context graph: captures why and causal chain
- http://context-graph-demo.vercel.app demo
  - Lots of algorithms to analyze topoligical similarity
- Build solutions that cut hallucinations; force agents to show their work
- Learn more at Neo 4j Graph academy: https://graphacademy.neo4j.com/
  - blog post: https://neo4j.com/blog/agentic-ai/hands-on-with-context-graphs-and-neo4j/
- 
