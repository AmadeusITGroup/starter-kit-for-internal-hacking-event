# How to organize a Hacking Event event in your company?

So, you would like to organize a Hacking Event in your company?
That's a great idea!

We propose here to organize a ~2 days contest event for your colleagues, which will look like this:

**Day 1**: Kick-off and training - 2 to 3 hours. Learn about security, and how to use the hacking tools from the security experts.

**Day 2**: Event -  Full Day. Hacking time! The teams helped by a security expert Coach, will try to hack the application they know best.

**Day 3**: Judging - Full Day for the coaches, 1h per team. Decide if the findings are real issues or not. Select the best team(s).

**Day 4**: [Survey](./post-event/Survey.md) and Closing ceremony.

If possible, we encourage you to do the event **on site**, with people seating together rather than remotely. We did it on multi sites, it's not easy but it's possible !

----

## Disclaimer

This document was originally written based on the experience of Hacking Event organized at [Amadeus](https://amadeus.com/), an IT company supporting the travel industry. You might have to adapt it to your environment. This document is opinionated, based on our environement, requirements and mindset.

----

Here are the steps to organize a Hacking Event:

## Pre-event

### Gather a team

Don't organize the event alone! See [Organization team](./pre-event/OrganizationTeam.md).

### Define a scope and get management approval

A reduced scope (one or a few products, one technical stack) helps to keep the focus on the tools and techniques.

Once decided, contact your management to get their approval and support. The more support you'll have the best outcome for the event !
See [GettingManagementSupport](./pre-event/WhySuchEvent.md) to be convincing.

### Block a date

This is challenging, especially if you are doing a multi site event with different time zones.
The Kick-off and Restitution should be at the same time for all sites. The event and judging should be done in local office hours.
Beware of bank holidays, in case of doubt, contact all site organizers.

This type of organization can take some time and we are usually starting to block a date **3 months** in advance in order to have the time to prepare everything on our side.

### Prepare the contest

If you want the team to be more interested and more efficient it is cool to organize the event like a contest. In order to do this, you need to prepare
- Rewards for the winning/runner-up teams
- Prepare the [judging rules](./event/JudgingRules.md) and made them publicely available

### Communicate

A critical part! See [Communication pre-event](./pre-event/Communication.md)
The clearer your communication is, the more people will be interested.

----

## Event

You reached this point? Congratulations, the event will occur!
Now let's dig into the logistics and organization.

### Logistics

It's important to be a good host for a good events. Go to [logistics](./event/Logistics.md) to get more informations.

### Create the teams

The perfect team size is 5 people, to have everyone working and some animation :

- You can ask the participants to create teams themselves. It might help getting more people but you can't decide the skills in each team.
- Tou can create the teams yourself. A bit more work for the organizer, but allows to mix skills (for example UI, Backend, Database,...) and allow networking.

Do as you prefer, we tried both and both are working.

Once done, communicate to the participants which teams they belong to, and ask them to select a **team captain**, who will be the main point of contact for the teams.

We also listed some [common issues](./event/CommonIssues.md).

### Create the team's pages

During the event, the team will find useful information on the **team's pages**, and will write their findings and tests on these pages. This is really important because this template will guide the team to follow a way of working and, from your experience, the teams are usually a bit lost at first so the better your template is, the best the results will be !

Ask the Captain to fill the team's page before the event.
You can find the template on [team-pages-template](../material/team-pages-template.md)

Use your usual Wiki/knowledge sharing platform preferably (Confluence, Sharepoint, Google Docs, ...).
If possible, restrict the team's pages to the team members + coaches to avoid potential sensitive information such as a set-by-step exploit being publicly visible in the company.

### Prepare the kick-off presentation

The kick-off is also your training. You can invite much more people than the one doing the contest. I'll allow to train people and make them want to participate to the next event !
See [material/training-content-sample.md](material/training-content-sample.md)

Make sure the participants read the rules of engagement: [material/rules-of-engagement.md](material/rules-of-engagement.md)

----

## Post-event

### Survey

As strange as it seems, it should be prepared before the event !
I'll be critical to assess the quality of the event as well, get feedback from the participants and prove that your event was successful!
More information [here](./Survey.md) and a sample [there](../material/survey-sample.md).

### Communicate on the event and its results

After the event (and ideally the survey) you should communicate on it. Send pictures, a cool text and highlight the winning team(s). More details here [communications](./post-event/Communication.md) 

### Fix the vulnerabilities

This is something important as you could discover complex things. From our experience, we followed our usual application security ticket process but you need to be ready to manage thoses new tickets.

Having such tickets **could** be seen as a failure but it's in fact a great success. Each vulnerability you find is something that exists, maybe since a long time, and that you are now aware.

The more vulnerabilities the better!

### Communicate on the findings (yes, you read it right)

The findings maybe completely unique or similar finding by different teams. In this case, it's always good to communicate **privately** (restricted audience) them to your management and your application security office (or the equivalent for your organization). They could learn from them, update some scenario, improve some process.

Once they are fixed (it could take several weeks for the most complex) you should communicate **internally** (in your organization but with a wide audience) on the findings.

Why such craziness?

- The audience will learn **real** vulnerabilities that actually will talk to them (as they know the product). Not basic training of basic problem, but real life example they understand
- The audience may find similar vulnerabilities in different products
- Showing **transparency**, that only the ones who don't do anything aren't making mistake. That finding your mistake and fixing it is much more valuable that just hoping that you don't have any.

Every vulnerability you'll find and fix is a vulnerability that the hackers won't exploit!

----
