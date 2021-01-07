# Home
 
All Clojurians are welcome to participate in the development of a chat app to help mitigate the risk of no longer being able to use Slack: Slackpocalypse

# What is this?

 
This will become the ultimate chat platform for the clojure community, built by the clojure community. Not only do we want to provide a realtime chat platform, we want to showcase the ecosystem and the tools this language has to offer.
 

# Why?

 

- Slack is proprietary and closed
- Slack is a for-profit company controlled by the whims of its investors
- Slack-the-company has declared they do not intend to support OSS communities as a valid use-case
- Thus, it is possible/likely that Slack will change their terms of use in the future in ways which make large OSS communities on the platform untenable
- Slack's current free plan only allows access to the most recent 10k messages. Due to the size of the community, this is about a day's messages right now, and presumably this will get worse over time. Various archiving hacks exist, but they're currently a violation of the Slack ToS and put the whole community at risk of being shut down. They also can't archive private conversations.
- See Slackpocalypse for more.

 
**Goals**

- Slack-alike functionality
  - Organisation/channel based chat rooms.
  - Direct messages
  - Avatars
  - Emoji
  - Reactji
  - File uploads
  - Code highlighting
  - Easy signup workflow
  - Smart-links (should inline gifs if a gif link is pasted, smart previews of linked articles)
  - Search (ideally full-text clever search of entire archive)
  - Image support
  - Notifications
  - Integrations (git, etc)
- Able to support at least 50k users without falling over
- Must provide complete archive of activity
- Mobile-friendly layout
- Should be scriptable/botable
- Easily deployable (should be possible to have a one-click-install button like on Digital Ocean)
- ???
### **Nice-to-haves**
- Mobile clients (arguable should be in the main goals)
- Reactji Performance Art (see pkobrien for examples)
- Identicons ([https://en.wikipedia.org/wiki/Identicon](https://en.wikipedia.org/wiki/Identicon)) or similar ([https://robohash.org/](https://robohash.org/)) so people without custom avatars can still be easily distinguished
- Embeddable (in other sites)
- Clustering? (Will or can different deployments be clustered?)
- ???

 

###  **Practical Considerations**
- Performance
  - If this app brings a phone browser to a grinding halt, it's not going to work out (shouldn't be a big problem - i'm deploying a re-frame based app to phones with cordova and, apart from transitions, html/css/js is all fine - mccraigmccraig)
  - ditto for the server, ideally it should be possible to deploy on a $5 Digital Ocean VPS (I think this is unnecessarily restrictive - cfleming)

 
**The Case For Inventing Our Own Wheel**

- It's fun!
- The Clojurians are clever and passionate people.
- The world could do with a (or indeed several) truly OSS Slack clone.
- Other wheels we've evaluated would require significant work to be a truly attractive slack replacement, and we don't want to do significant work if it's not in clj(s) :D. Also, Mattermost has a strange license...
- A Clojure-based Slack clone would be:
  - An excellent showcase of the power of the language
  - A great tool for building the Clojurians community as it builds its own platform
- Gives those of us who don't have a chance to write Clojure/Clojurescript for a living a chance to showcase abilities and practice skills.

 

### The Devil's advocate against inventing our own wheel
- It's a big project and we're all very busy.
- There are reasonable OSS options we could self-host (Mattermost, Zulip), they're just not clj(s)
### **Other wheels**
- [https://www.flowdock.com/](https://www.flowdock.com/)
  - not self-hosted, and probably not scalable to our needs. but useful to look at for UI inspiration
- Zulip
- Mattermost
  - would need lots of UI polish things, and there are some consistency issues (unread count + notifications) that might be harder to fix
- Discord
  - not self-hosted, but the reactiflux community moved there and appear to be happy w/ it
- Discourse (forum, not chat, but similar problem) 
  - not chat, but very widely used for communities such as ours, solves some of the problems.
- RocketChat
  - [Here's a source](https://www.reddit.com/r/Meteor/comments/2w3i32/is_mdg_serious_about_mongo_alternatives/coo04zy) saying that each meteor process can handle 200 users, so on an 8-core machine w/ 4 processes per core, that's 6400 users. Although we don't know how well that applies to the RocketChat app specifically
- Vector.im (matrix client) (see [The case for Matrix](/xRXYSO9zpyh))
  - the general room has ~65 people online, out of 2k members 

 

# Who?

If you feel like you have a stake in this effort please add your name to this list so we know that you feel this way. This doesn't imply a commitment or seniority or anything other than that you are involved and want to be kept in the loop. If you also have time to help out, even better. But serious interest is enough.
 

- adulteratedjedi ([https://github.com/adulteratedjedi](https://github.com/adulteratedjedi))
- cfleming ([https://github.com/cfleming](https://github.com/cfleming))
- mfikes ([https://github.com/mfikes](https://github.com/mfikes))
- pkobrien ([https://github.com/pkobrien](https://github.com/pkobrien))
- seancorfield ([https://github.com/seancorfield](https://github.com/seancorfield))
- shanekilkelly ([https://github.com/ShaneKilkelly](https://github.com/ShaneKilkelly))
- chrishowejones ([https://github.com/chrishowejones](https://github.com/chrishowejones))
- donmullen ([https://github.com/donmullen](https://github.com/donmullen))
- lfn3 (Liam) ([https://github.com/lfn3](https://github.com/lfn3))
- jaredly ([https://github.com/jaredly](https://github.com/jaredly))
- arrdem ([https://github.com/arrdem](https://github.com/arrdem))
- johanatan ([https://github.com/johanatan](https://github.com/johanatan))
- kimsnj ([https://github.com/kimsnj](https://github.com/kimsnj))
- bhauman ([https://github.com/bhauman](https://github.com/bhauman))
- s-mage ([https://github.com/s-mage](https://github.com/s-mage))
- qsys ([https://github.com/qsys)](https://github.com/qsys)
- mitchelkuijpers ([https://github.com/mitchelkuijpers](https://github.com/mitchelkuijpers))
- mccraigmccraig ([https://github.com/mccraigmccraig](https://github.com/mccraigmccraig))
- rafd ([https://github.com/rafd](https://github.com/rafd))
- madstap ([https://github.com/madstap](https://github.com/madstap))
- afhammad ([https://github.com/afhammad](https://github.com/afhammad))
- plexus ([https://github.com/plexus)](https://github.com/plexus)
- jumarko ([http://github.com/jumarko](http://github.com/jumarko))
- you... ?

 

# Where?

The Internet.
 

# When?

April 15 at Clojure/west 2016 would be a nice target date for having something, even just a demo.
 

# How?

**Tech**
Clojure on the server, Clojurescript on the client. All other technologies should be chosen on their ability to meet a particular need of the project. Our tech stack should be as simple as it _can be_, while being as complex as big as it _needs to be_. We should refrain from throwing a technology/library into the stack "just because".
Whether it should use Datomic is an open question due to licensing. 
 
**Organisation**
 
Need some kind of collaboration tool to manage features and determine who is working on what.
 

