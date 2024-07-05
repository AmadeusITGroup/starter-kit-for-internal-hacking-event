# Training

This page contains sample ideas for the training to be provided the day before the hacking event.

We recommend to have, at least, the 4 following items:

* Real life vulnerability: previous (fixed) vulnerability on your product to show that it exists
* Tooling: show what tool to use and how it is working 
* Method : show the methodology that the teams will have to follow during the event
* Fake example: display what the team will need to do on D-day with an interactive session
At the end of the training, explain how the event will work, the [judging criteria](doc-for-organizers/JudgingRules.md) and the rewards for the teams .

## Show real life (old) vulnerability

The problem with security vulnerabilities is that they can be of many different kinds. The goal of this event is to focus on **functional security** only, so you need to find a _common_ vulnerability that happened in the past. Ideally it should be on a product that is well known and in a use case which is very standard. The more the teams can related to it, the more that can imagine interesting tests.

**Warning** : When you disclose a vulnerability, there are some ground rules to follow

* Do not disclose something that is not fully fixed in all environments
* Do not explain in detail the impact, cost, and if it has been exploited
* Do not point finger at the product or team that "produced" the vulnerability
* Focus on how it may apply on other similar product or use case

## Learn about the tool

Depending on your technology you may have different tools to do security testing. For example, if you are doing web applications, a tool like [Burp](https://portswigger.net/burp) is very interesting as it is user friendly, free for most features and allow to tamper the HTTP request from a browser to a server.

Doing a demo of BURP, changing some values and seeing that the server may behave differently is really interesting as it is simple but sufficient to find a lot of vulnerabilities.

The team will learn and practice a new activity, so the simpler the tool, the easier it is for them to focus on the security testing scenario rather than learning how the tool is working.

Finally, the team will be able to reuse this tool and possibly integrate it in its own process of quality assurance.

## Learn about the method

The methodology of functional security testing is to twist the team's usual way of working.

Normally, you are creating a feature that can (or cannot) be used to provide something. Here your user becomes an **abuser** and your use cases becomes **abuses cases**.

The recommended process is something like this:

* Find your **assets**, the data that the hacker wants or the service that are important to you
* Find the use cases where those assets are managed and try to abuse them
* Abusing a case is usually about playing with the parameters
* Try to change escalate privilege
* Try to escape isolation
* Try to do an action unauthorized
* ....

## Example of team working

The next demo should be showing what the event will look like the next day. A good approach could be to _play_ a team, do a security test live, fill the documentation page and even the judging session.

This way the team will have a good idea about what will happen during the hacking day.

## Logistics

Finally you need to finish with a word about the logistics, at which time people should come, in which room, and a quick agenda about the day.