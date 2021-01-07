# IRC
Before Slack there was IRC. There still is IRC, but Slack is more popular. What can we do to create a better integration of the two in the new app? Or do we not need to do that? Please discuss.
 

- [http://whatthefuck.computer/blog/2015/11/01/on-the-balkinization-of-my-chat-communities/](http://whatthefuck.computer/blog/2015/11/01/on-the-balkinization-of-my-chat-communities/)

 

# Comments on IRC

@seancorfield 

  "A couple of Slacks I'm on have tried full-on IRC bridges and they're an ugly experience (for both sides) since they have to fake the to/from accounts in bridged messages and they don't will any of the rich formatting or multimedia on the Slack side."

 
@seancorfield

   "[#clojure](/ep/search/?q=%23clojure) on freenode is much smaller then this Slack community and there's a huge overlap in the actual participants ... I'd say there's probably only a small number of folks who are IRC-only (compared to 4,400 here, rather than 700? on IRC)."

 
@seancorfield 

  "it must have the low barrier of entry that Slack provides (which is why IRC has never grown to the level that Slack has).

 

  IRC is great as a plain text communications tool for communities but it’s a pretty sucky UI/UX, even with the nicest clients. And even with those clients, you’re still confronted with servers and ports and a bunch of IRC mumbo-jumbo that is irrelevant to "having and growing a community".

 

  If you want to bolt file uploading, code snippets, formatting, pasting images inline, sharing links that auto-expand and a whole bunch of features on top of IRC, you’ve got to also consider how all that affects the users of the underlying IRC rooms. You also need to consider community administration: Slack allows an administration team to manage user accounts, permissions, integrations and so on.

 

  Even on a closely controlled IRC server, maintaining decorum in a community is nigh-on impossible: have you seen the drive-by trolling and abuse that happens on Mozilla’s IRC servers in the Rust community, for example?

 

  I gave up on the Rust IRC community because they seemed unable to prevent spamming to a level that was making rooms unusable. *On their own servers*

 

  "I would be interested in seeing why people have latched onto Slack vs. IRC." — mostly because of the issues with IRC I listed above, which Slack does not suffer."

 
@shaun-manhood

  "Yeah, that's my main reason as well - I kept thinking of going on the IRC channel but never wanted to put in the effort."

 
@jaen

  Re: multiline messaging [not being supported by the IRC protocol] - that seems to be true according to the RFC:
    IRC messages are always lines of characters terminated with a CR-LF (Carriage Return - Line Feed) pair, and these messages SHALL NOT exceed 512 characters in length, counting all characters including the trailing CR-LF. Thus, there are 510 characters maximum allowed for the command and its parameters.  There is no provision for  continuation of message lines.
  ...
  True, but the server/proxy could just collapse messages according to some criteria for non-IRC users.
  And Matrix quite possibly solves those problems as well.
# IRC Bridge

Just because one implementation of a bridge does not handle multimedia integration very well does not mean that all possible bridge implementations would suffer the same.
 
And this is precisely why I suggested folks setup a test Slack and ***actually try out the various IRC bridge projects*** rather than continuing to discuss them in the abstract!
 
Also, "fake handles" might not be an issue: why not just clone whichever handle the person is using on whichever side to the other side (unless there is a collision and then just append _N)?
 
And, regarding the potential for abuse/trolls from the IRC side polluting the "nice UX" side-- I would expect that the IRC channels themselves are already moderated/supervised so this wouldn't be an issue any more so than it already is for the IRC folks.
 
Based on Rust's experience -- on Mozilla's _own_ IRC servers -- it is virtually impossible to stop abuse and trolling on popular channels: 

  I gave up on the Rust IRC community because they seemed unable to prevent spamming to a level that was making rooms unusable. *On their own servers*

 

# IRC vs something else

Discussion from HN here: [https://news.ycombinator.com/item?id=10494224](https://news.ycombinator.com/item?id=10494224)
 
See also: [https://twitter.com/patio11/status/660931499680657409](https://twitter.com/patio11/status/660931499680657409)
 
IRC protocol extensions
 
Lots of info is [here](https://github.com/grawity/irc-docs/blob/master/extensions.md) . I have no idea what 90% of that page means. In fact I have no idea what 90% of the IRC terminology means in general. I stumbled through getting myself set up on IRC but it was painful and I've forgotten whatever small amount I learned in the process.
 
 

