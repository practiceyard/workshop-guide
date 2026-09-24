# Learning Objectives
*Clearly communicated clarity aligns expectations*

Having clearly defined learning objectives for your workshop will make a big impact.  Not only will it help guide the decisions you need to make, it will align both participant expectations and the work your team does.  If you're reusing content, you'll want to first identify the objectives embedded in the content, then review and revise based on what you're looking to accomplish.  If you're creating your own, you'll start with some, and be ready to revise as things progress.  Either way, you'll want to write them down. The level of detail can vary, as this is about clarity in decision making, not creating an auditable document. 

## What Will Be Done

The first component of the objectives is the most intuitive - what will be done.  This could be building a "product" that is usable.  Realistically, an output from a workshop will not be a full-fledged product.  There'll almost certainly be other things that will need to be done before shipping.  However, what is produced ideally will be usable.

A second option is to learn a "business" process, or how to perform a task (with task here meaning something meaningful or useful - not just using a feature for the sake of using it).  This process/task should be something they would look to do again in their own environments.

A third thing for participants to do is to "explore".  For some situations, that's all you can do, but it results in less experience.  However, exploring can be a secondary objective. For instance, creating a DynamoDB table might be key to building a product, but exploring the backup settings may be a secondary objective.

Once you have a primary objective/goal, you might also identify secondary objectives.  These can be additional aspects added to the product/process (the primary objective), or specific learning objectives, including "exploring" a feature. Knowing what is on the critical path and what is optional is important if tradeoffs need to be made both before the workshop and during it.

## What Won't Be Done

One might think that anything that isn't in the "What Will Be Done" classification will comprise the "What Won't Be Done" category.  If everything is defined precisely, that might be true; however most of the time there will be things that only *might* need to be done, or are implied instead of explicitly being noted.  Either of these situations is fine, and as previously noted, defining the learning objectives is meant to guide, not be an exhaustive audit.  To make things more manageable, noting the things that are not expected to be done provides better guidance than trying to define everything that *must* be done.

Additionally, it is good to differentiate between what participants won't be doing that the organizer will (on their behalf), vs. things that are just plain out of scope.  For instance, if an AWS account won't be set up, does that mean that the participants won't do that, the organizer will do it for them, or the participant needs to have one already?  Being clear will avoid confusion.

Ignoring irrelevant items, the strongest candidates for this category are things that might seem related (thus putting them out of scope), or things that can run longer than the workshop itself.  For instance, if an automated security review of code is required, perhaps that needs to be set up in advance so the participants can look at the outcome instead of just a "waiting to complete" message.  We'll come back to waiting time when we cover the content architecture.

## What Comes Before

Everyone's background will be different, so it's going to be best if you articulate what people should bring or have, plus what they're expected to know ahead of time. If it's too much of a stretch, participants can self-select out. Ideally lecturing or non-active content during the workshop should be kept to a minimum. This doesn't mean there should be zero. Setting up the context and recapping the objectives should be done at the outset, and a recap with next steps is ideal for the end.  Based on your content, you'll have to find the right overall balance, but lean towards more time spent on hands-on activity.  Most workshops are 200-300 level to achieve this balance.

If you have a prerequisite that is knowledge based, help your attendees by pointing them to resources to help them come up to speed.  Maybe it's documentation, maybe it's a video. If there's software that they should have set up in advance, share the install link/command or a getting started page.  Remember some people might not have administrator access, so advance notice can help them work around that.  It's unlikely that if someone doesn't have a laptop that you'll be able to bridge that gap, but knowing in advance will help lessen any surprises.

> Be prepared for the unprepared.

Despite good communication, it's bound to happen that someone will come unprepared. Someone will not bring the required laptop, won't be able to access an account, or won't have done any assigned pre-reading.  Have a plan for how to handle (if not outright prevent) people from being unprepared.  Consider backup devices, virtual desktops accessed via browsers, extra accounts, in-line context/reading or whatever is relevant to your workshop.  If you want a top-notch workshop, treat it like resiliency planning - explore what could go wrong, what the potential impact would be, and decide if mitigating or accepting the risk is the best path forward.

## Example Learning Objectives

Here's a basic example to help jump start your objective development:

### Will
* GOAL: Build a working Flappy Kiro game on their laptops using Kiro.
* Learn how to get started using Kiro
* Explore vibe coding
* Explore spec-driven development
* Understand when to use which approach
### Won't
* They won't set up (or use) an AWS account.
### Pre-requisites
* Generally aware of what AI is.

---

[◀ Previous: Introduction](../01-Intro/Introduction.md) | [Home](../README.md) | [Next: Content Architecture ▶](../03-ContentArchitecture/ContentArchitecture.md)
