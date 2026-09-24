# Environment
*How much of a problem it is depends on where it happens*

The Workshop environment has multiple facets, from physical to virtual to financial. Consider each and plan accordingly.

## Physical Location
Given the context of the in-person workshop, the venue is a key decision from which many other things flow. A few advantages of the in-person workshop include the ability for participants to focus (distraction-free), people walking around can observe when someone is struggling, and networking (the people kind).

As you select and prepare your venue, questions you'll need to consider include:
* Where is the venue?  Is it available?  Is it convenient to the target audience?
* What is the room layout?  Classroom style is ideal, but group tables can also work.  Theatre style is much harder to make work.
* How many people can be accommodated?  What about support personnel?  Can rooms be combined to make a larger room?  Will there be multiple rooms, potentially connected via video feed?  What is your normal drop-off rate when comparing registrants to those who show up?
* Is the venue relatively distraction-free?  Will there be other groups co-mingling?
* How do you get support from the venue as needed?  E.g. what happens if the room is too hot (or too cold)?
* Are there sufficient electrical outlets that are accessible to the various tables?
* Is there a projector/screen?  Are there whiteboards?  Will microphones be necessary/helpful?
* How is the wifi connection?  Can it support the number of expected participants doing the expected things? Will a password be required? What happens if the network goes down?
* How does the venue accommodate food? Can you bring your own? Are there tables?  Plates, napkins, cups?

## Technical Environment
Equally important to the physical environment is the virtual or technical environment. It starts with the participants' laptops (or other devices) and extends from there.

Assuming that participants will use a laptop (something you should validate for your workshop), then you'll need to consider what operating systems you will support, browsers, programming languages, etc. It's normally workshop specific, however the more standard you can make it, the easier running the workshop will be.

Consider if you have to write instructions for mac, linux, and windows. Then multiply that by Node.js, Python, Java and Rust. It can get complex very quickly. Then layer on different security setups - both account access and local access. Keep It Stupid Simple (KISS).  The best solution is to minimize local requirements and host as much as possible in the cloud where you can provide a standard environment.

If you can, the best option is the AWS Workshop Studio. It handles many of the challenges that come up with workshops.  AWS has poured a lot of heart and soul into making it a good environment. Unfortunately, there are some conditions to using that environment.  The two main ones are that someone from AWS has to be involved, and the workshop needs to be a workshop provided by AWS.  If you want to be on your own schedule or want to deliver a custom workshop, then the AWS Workshop Studio probably won't be a fit.

A closely related option that was recently released on Builder Center is individual Sandbox accounts. Great for individuals to explore workshops on their own schedule, however this can be a risky option for an organized event.  First, only one session is permitted per week, so if someone tries it out to ensure it works or explores a different workshop, then that person won't be able to participate during the workshop. Second, capacity isn't guaranteed.  Participants could attempt to launch the workshop, and can be denied because too many other workshops are running.

Another option is the Sandbox Accounts for Events solution found at https://github.com/awslabs/sandbox-accounts-for-events. Sandbox Accounts for Events provides multiple, temporary AWS accounts (preferably in an AWS Organization) to a number of authenticated users simultaneously via a browser-based GUI. It uses the concept of "leases" to create temporary access tickets and allows to define expiration periods as well as maximum budget spend per leased AWS account.  This can be a suitable option, but does require additional setup and management.

The next option to consider is the Innovation Sandbox on AWS found at https://docs.aws.amazon.com/solutions/latest/innovation-sandbox-on-aws/solution-overview.html. It's enterprise grade, great for internal teams which need long term accounts. Authentication is handled through Identity Center.  Unless the workshop is internal to a company, it's likely this is not going to be suitable.

For some workshops it will be suitable to use a shared AWS Account. If you apply some credits, it could be no cost to participants.  You can do a custom workshop, however by default there are no guardrails, no isolation, and participant management/access management is all on the organizer.  It’d be the wild west, relying on local setups heavily.  For most cases, probably not the right choice.

Bring your own account (BYOA) is the approach that provides the most flexibility. You'd need to spread around credits to avoid incurring costs. Accounts have to be setup individually which can add to the workshop load. Then there's no central visibility into issues, so it puts a lot on the attendee.  For more advanced participants, this may make the most sense, especially since it allows them to retain what they produce very easily.
		
Practice Yard is a community-built workshop platform. It uses a single AWS account, with participant isolation and a management tool. It can handle up to 99 participants, and includes pre-provisioning an EC2 instance per participant with pre-installed tools (including Kiro) accessible via browser.

### Cleanup
If you aren't using an ephemeral account that will automatically dispose of resources, consider the following methods to clean up the accounts:
* AWS Nuke - removes all resources - https://aws-nuke.ekristen.dev/
* Resource Explorer - within AWS use Resource Explorer to locate resources, then remove them.

## Financial
The final environment to consider is the financial one.  Who pays for the venue?  The food? Who covers any cloud costs?

Venue and food sponsorships would be handled like any other meetup - perhaps a local AWS Partner will cover the costs.  Worst case you could consider BYO snacks or charge an admission fee.  If you choose to charge a fee, consider how that barrier will affect participation.  Scholarships should be available, or just don't charge a fee - find a sponsor.

If you aren't using a technical environment managed by AWS, then consider requesting credits for a central account, or each participant account, depending on the chosen environment.  It may also be possible to get Kiro credits.

---

[◀ Previous: Content Architecture](../03-ContentArchitecture/ContentArchitecture.md) | [Home](../README.md) | [Next: Delegation ▶](../05-Delegation/Delegation.md)
