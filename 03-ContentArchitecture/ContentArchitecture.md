# Content Architecture
*How it’s Structured is equally important as to what it is*

Workshops need to have a structured path.  Attendees might have knowledge of the subject, but to achieve the learning objectives, they need to be shown a path, lest they wander aimlessly.  Remember, many people are attending a workshop because they are looking for a path to apply their knowledge.

If you are using previously produced content (e.g. from the AWS Workshop catalog on Builder Center), the primary architecture is already worked out.  You should still test it out to ensure it's still current, as well as to confirm you understand how the workshop will integrate with your environment.  (More on environments in the next section.)

For those creating a bespoke workshop, there are many things to consider including the order, the grouping, the timing, different skill/speed levels and more. The content needs to also tie back to the learning objectives.  Once you have a basic outline for what you want to achieve, AI will be a useful aid for fleshing out the workshop guide. Regardless of who creates the content - people, AI or a combination - the workshop needs to be tested to both confirm the content, but also the timing and the environment.

## How-To Guide
Most workshop guides consist of a step-by-step guide for participants to execute at their direction. This is table stakes for the workshop. Some will add screenshots to this guide to make it more friendly to new users. On the flip side, avoiding this will allow the guide to survive UI changes and reduce the amount of scrolling needed. Additionally, adding screenshots is a lot of work, which would likely yield a higher return if spent in other areas. If the UI can be confusing to inexperienced users, or if the needed instructions don't lend themselves to text-based descriptions, then by all means, include images. Remember, this guide should inform your decisions, not dictate them. 

You could think of the necessary steps as one big, long, ordered list of instructions; however the instructions should be grouped into sections. Each section should be related to a deliverable or milestone in the process.  For each section (in addition to doing this for the overall workshop), give a brief description of the objective related to the section, as well as a description of the technical steps that will be taken.

Within each section, number the steps so it's easy to track progress. Each numbered item should be a distinct action. Don't use a single item for multiple steps.  If there are multiple, complex actions that are related and are essentially part of a single step, then use sub-items.  For example, an item might be to create a new S3 Bucket. The numbered item (top level) would be to create the bucket, then the next level down would be for each section, and the third level for each element in the section.  This organization will allow for specific references if there are questions, plus for someone familiar with creating a bucket (or whatever the step is) will not risk missing unrelated information buried within the step.

For an even better workshop, include alternate methods within the guide.  Assuming the environment allows you to provide a single set of instructions (i.e. one shell/operating system, one programming language), adding alternates will allow participants to use the approach of their choice.  The base set of instructions is typically using the UI (e.g. AWS console).  Alternates could be using the CLI or an AI assistant (e.g. Kiro).  If provided, that would be the first level below each numbered item, as it should be clear that only one of the approaches needs to be performed.  Organizationally, you could group all of a single approach's steps together rather than spreading them out.  This could be preferable depending on how different the steps are. If you're unsure, try it out both ways. AI should make it relatively easy to pivot between the layouts.

### Abbreviated Example
1. Create an S3 Bucket in the Account Regional namespace with a name of your choice.
    1. Set the **General Configuration** values:
        1. **Bucket type**: `General Purpose`
        1. **Bucket namespace**: `Account Regional`
        1. **Bucket name**: pick a name memorable to you, using lowercase letters and numbers
        1. Leave the remaining values as their default.
    1. Set the **Object Ownership** to **ACLs disabled**.
    1. ...
    1. Click **Create Bucket**

### Style Notes

In the previous example, **BOLD** was used for text which are labels or values to be located in the UI.  Backticks (`) were used for text which needs to be entered by the participant.

## Catch-Up Solution
Most people plan to arrive on-time; however life happens, so some people will show up late. Others might be unable to make good progress in the workshop because they are impeded by their laptop, or maybe they get an important phone call.  Or maybe, things just go so wrong - like some sort of disaster.  All of these situations will benefit from a 'catch-up' solution that helps someone catch up after falling behind, like disaster recovery.

These catch-ups are usually a script or perhaps a CloudFormation template. They provide a way for someone to skip a given section and be ready for the next, just by using the catch-up solution.  Another potential use of the catch-up solutions is to allow participants to check their work by comparing their work to the solution.  This won't work in every case since the ability to check the results is limited by the catch-up solution format.  Probably easy using a CloudFormation template. Not so much with a script unless the script is run.

## Next Steps
When wrapping up the workshop (and in the guide), be sure to include "next steps".  This should be reinforced as part of your session closing.  The questions you should address include:
* How do the participants keep their work
* How (if?) they can continue the workshop after the session
* Where can they find follow-on learning, reinforce their learning
* Where they can dive deeper

More broadly, you should encourage the participants to join the User Group / Community if they haven't already. This also includes taking an opportunity during the closing session to market your next User Group meeting.

## Bonus Content
If you have the bandwidth when preparing for the workshop, consider adding bonus or optional content. (Bonus, optional - both mean the same thing here.). This bonus content would allow advanced participants, fast workers, or folks highly interested in the target to have additional ways to fill extra time during the workshop.

---

[◀ Previous: Learning Objectives](../02-LearningObjectives/LearningObjectives.md) | [Home](../README.md) | [Next: Environment ▶](../04-Environment/Environment.md)
