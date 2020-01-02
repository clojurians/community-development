## Rules and guidelines for the `#announcements` channel

`#announcements` is one Clojurians' most popular channels, and a particularly benefitial one for having a healthy, cohesive community of makers.

Because of that, it's important to have some rules about what can be posted, and how often: that way the channel can sustainably keep people engaged.

#### Focus

The focus of the channel is sharing Clojure libraries and projects.

That excludes content that would fit better in `#news-and-articles`, `#events`, etc.

Specifically, the focus of the channel is _not_ 'hit as many eyeballs as possible'. People generally come to the channel with a certain expectation of its contents. People willing to be offered random content will be browsing `#off-topic` or specific channels.

#### Frequency

* Announcing new libraries is generally always ok.
  * Perhaps, try to not announce projects too early (unless user feedback is specifically sought): it's reasonable to say makers want to be informed of _libs that can be used_.
  * Announcing libs too early leads to having to post updates later, depleting overall attention.
* Posting updates of libraries in `#announcements` is ok, provided that:
  * the update frequency is occasional: think 4 to 6 times per year max.
    * as a rule of thumb, we should try not bother too much people who are aware of the existence of your library, and don't happen to be using it at the moment
  * the update is important
    * major features, critical bugfixes, etc
  * the update is properly presented
    * posting a link plus the new version number is not informative enough

#### Automation

Although adding a personal touch can add something, generally we should be aware that a large chunk of the current `#announcements` activity could be as well automated.

Did you know both GitHub and Slack offer a RSS integration?

Given that people can hit `/feed https://github.com/user/repo/releases.atom` themselves, perhaps we can encourage that kind of workflow.

In the end it's more selective (people decide what news to receive), and might result in _more_ engagement - not less.

Accordingly:

* Consider updating your project's README instructing how to keep up
  * e.g. here's my twitter, our company's engineering blog, use this RSS feed
* Consider posting fewer updates to `#announcements`, accordingly
* Consider integrating security bugfixes with the NVD database
  * [lein-nvd](https://github.com/rm-hull/lein-nvd) is a thing
