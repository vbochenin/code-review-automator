# code-review-automator

Main purpose of this project,, it's trying to automatize code review process.

Problem #1: In our process we have rule: PR could be merged to main code base just after 2 :+1 .
First one :+1 should be received from PR creator's team.
Second one from another team in same organization.
It's hard to track this PR and chase guys from teams to take a look on it.

To solve this problem, we can use GitHub's webhooks and automate it.

Algorithm:
Apllication listen a GitHub notifications in scope of PR.

When PR created in GitHub

Then application sends a message to contributor's team. "Guys, please review it"

When reviewer set :+1
Then application sens a message to different team.
(TBD: Team choosing algorithm )

When reviewer set :+1
Then application sens a message to contributor. "Congrats, dude! You PR will reviewed."





