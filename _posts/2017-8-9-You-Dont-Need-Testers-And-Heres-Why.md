---
layout: post
title: You don’t need testers and here’s why
---

Look, we all know the usual software building workflow:

> Design -> build -> test -> ship (the product)

Usually you have at least four people involved in this chain from four different teams. My argument is that this can be greatly simplified to two teams with three people for maximum efficiency.

So what’s wrong with the current solution? I think, there is a huge problem with the handoff from building something to testing something and then shipping it. Usually the problem manifests in a ping-pong routine between the tester and developer. However I see an even more pressing issue: the tester needs facilitation to be able to test. The range of things to check of can be:
- making sure technical documentation is existing and up to date
- making sure product documentation is existing and up to date
- making sure the environments work as expected
- pre-checking the implementation before handing it off
- ensuring the tester can test the implementation in existing pre-prod environments

That’s a lot of things to do just to hand something off to the next person and try not to think about this anymore. And we all know, even if all of this is set, the tester will come back to the developer and ask additional questions when  the developer is already working on the next item. This costs time.

There are many reasons why the time lags occur, the things mentioned above are things that we should do in any case, but having someone with less technical experience testing the implementation means that if an issue is found, the developer needs to take time and evaluate the severity of the issue along with the tester. Some argue this is a good thing. I don’t think so. It wastes everyones time.

So how do you fix this? How do you get from testers to no testers? Do you just ship without testing at all? That’s no good.

I think the way to go is to have the developer test all of the implementation. This means code reviews, white box testing, black box testing, building automation and so forth. It’s essential that the person who writes the code does not do black box testing. However, this does not mean that another developer could not do that.

Let’s take another look at the flow we had above with expansion and roles attached based on this idea.

1. Design (by product team, PO, visionary or who ever builds the product)
2. Implementation (developer A [also does unit tests here])
3. White box testing (developer A on prod-like environment after merging with other code)
4. Black box testing (developer B on prod-like environment)
5. Ship it

## Why is this better?

First: as developers learn how to test, they also learn how to write testable code and how to expect common issues that they see while testing. They will implement a solution to a possible bug down the line even before the testing phase based on experience.

Second: the developer testing the code as a black box has development experience and knows the internals, so can see possible issues while testing and expect the cause of bugs when rejecting tasks. A top-level performer will find the cause in the code and make the life of the first developer much simpler because of this. Maybe even suggest a better solution in this step? Why not.

Third: while testing the developers can see and feel the product. They get the user experience that real-life users have. When only looking at the code and never considering the users after doing hand-off developers can have a very narrow focus. This forces developers to take a step back and look at the bigger picture. Are we improving the product or not?

Fourth: regression testing automation is much simpler when it’s already fascilitated by developers looking ahead and knowing how it needs to be done. Having first hand experience with implementations that are very tricky to test automatically will give valuable insight and will improve future implementations in this aspect.

Fifth: shipping needs to be done by developers. There should be a team to maintain the pipeline, but shipping needs to be fast, so developer B should be able to click on the button that says: ship to prod.

There you have it, developers can test just as well as testers, quality assurance or quality engineers. There is no magic in testing. When we skip a dedicated tester we improve our workflow greatly.

---
Footnotes:
1. I’m a Quality Engineer. Most of my days are filled with testing and automating testing. Looking at what I do, I grow more and more sure every day that my job should not exist.
2. I'm not advocating against compliance testing which is required in many fields.
3. Exploratory testing is awesome and has a clear role in any company. Just do it outside your dev cycle. 
