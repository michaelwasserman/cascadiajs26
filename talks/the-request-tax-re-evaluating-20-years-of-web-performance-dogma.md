# The Request Tax: Re-evaluating 20+ Years of Web Performance Dogma 

## Alex Moon
### WP Engine, Bellingham, WA USA 
- [Speaker's Notes (Placeholder)]()
- [Post-conference YouTube Recording (Placeholder)]()
## Abstract: 

For 20 years, we've been told to "Minimize HTTP Requests." But is that still true? I'm investigating how HTTP/3 and QUIC change the "Request Tax" and why I'm seeing patterns where granular fetches beat monolithic queries. Let's look at the data and re-evaluate the rules.
## Community talk notes: 

### Scribe: Mike Wasserman
- React is 13yo; SPA; to bundle or not to bundle
- bundle: JS/CSS (webpack, rollup, etc), inline CSS/JS/ data URLs, lots of ways
- 13yo HTTP had lots of things that made it slow, had to bundle, network is fater, but caching is worse
- tension between HTTP and TCP want bundling, but caching doesn't
- doc caching and code splitting
- HTTP/2 (SPDY) solved some problems, but TCP still broken
- HTTP/3 over QUIC solce problems in alot of cool ways
- but did that actually fix things in practice
- HTTP/3 wins when there's latency or packet loss, more requests is better for caching
- prompts:
  - avg dev: optimize for caching, stop stressing about the network
  - framework/bundler maintainers: is the fegault app/framework/route still the answer
  - cloudflare: get us more data on 2020 article on HTTP/3 performance
  - 

  