# Trust, But Verify: Human-in-the-Loop for Agents That Actually Matter 

## Michael Liendo
### Auth0, Davenport, IA USA 
- [Speaker's Notes (Placeholder)]()
- [Post-conference YouTube Recording (Placeholder)]()
## Abstract: 

We've built an ecosystem of capable agent. Now let's learn how to make them stop. In this talk we'll walk through various human-in-the-loop patterns. From simple inline confirmations, to out-of-band permission gates, to handing your agent a wallet with real money in it and more.
## Community talk notes: 

### Scribe: Mike Wasserman
- agents are doing more than answering questions: need human-in-the-loop to trust but verify 
- patterns
  - interrupt (back and forth check with human)
  - token vault (short-lived auth tokens)
- example travel apps that books flights
  - made flight reservation; wants to add google calendar event
  - how to give agent permission: connect google account in app settings
  - use Oath login; grant short lived permission to post
  - short lived scoped token (calendar only, with expiration date), not a long-lived API key
- What's ahead?
- CIBA: Client initiated backchannel authentication
  - push notification instead
  - stripe temporary credit card to let agent make purchase on your behalf
- High stakes external triggers: want human in the loop when things leave the app