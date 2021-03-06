# Code Review Comments

This page collects common comments made during reviews of code, so that a single detailed explanation can be referred to by everyone. This is a good starting for both new developers and experienced developers. New developers can use this while development and reviewers can use this while code reviews.

This is a laundry list of common mistakes, not a comprehensive guide. The list may not include typical issues identified by code analysis tools like linting tools, [SonarQube rules](https://rules.sonarsource.com), [fbinfer](https://fbinfer.com) or [errorprone.info](http://errorprone.info).

If your reviews are comprehensive and covered different perspectives than mentioned here, please feel free to continue the practices. You may raise an issue on this repository, if you feel those reviews checklist items are important to others as well.

Please discuss any changes for existing checklist items before editing them here, even minor ones. Many people have different opinions and this is not the place for edit wars. Raise a PR all members in the project team will be notified immediately.

## Languages

Please feel free to add new pages for languages not defined here.

* [Generic](./docs/Generic.md)
* [Java](./docs/Java.md)
* [Java Concurrency Special](https://github.com/code-review-checklists/java-concurrency)
* [Javascript](./docs/JavaScript.md)
* [React](./docs/React.md)
* [Python](https://pep8.org/)
* [Go](https://github.com/golang/go/wiki/CodeReviewComments) (Please [discuss](https://golang.org/issue/new?title=wiki%3A+CodeReviewComments+change&body=&labels=Documentation) with Google GO authors.)

## Code Design Review

We do not discuss the use of common design principle for each programing paradigm in this context. But the reviewer should be able to apply design principle knowledge while a review. Some good design principle are SOLID, GoF, Removing Side Effects, language specific designs etc...

## Unit Test Review

Some generic unit test review comments are identified [here](./docs/UnitTests.md).

## API Review

It is also important verify REST API standard while the code review when applicable. See the standard [here](https://github.com/syscolabs/api-standards).

## Security

We should use Static Code Analyzers and Dynamic Analyzers. But including an aspect of security review is mandatory as part of peer code reviews where these tools are unable to reach. Please refer Security Code Review Checklist (Page 196), Threat Modeling (Page 200) and Code Crawling (Page 205) [here](https://www.owasp.org/images/5/53/OWASP_Code_Review_Guide_v2.pdf).

## Code Reviewers Guide

* You don’t have to find fault in the code to do a code review. If you always find something to criticize your comments will loose credibility.
* Do not rush a code review. Finding security and functionality bugs is important but other developers or team members are waiting on you so you need to temper your do not rush with the proper amount urgency.
* When reviewing code you need to know what is expected. Are you reviewing for functionality, security, performance, and / or compatibility? (We have kept style away from peer reviews purposefully)
* Before beginning a code review does your team have a defined way to resolve any conflicts that may come up in the code review by the developer and code reviewer?
