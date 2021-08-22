# Venture Timeline

A chronological arrangement of list of things to take care of when starting your next big venture making sure all necessary things are addressed correctly at the right time.

# Background

Working for the software industry, I often came across a situation where a green field project needed to be setup. This meant, figuring out what kind of tools to use, how to maintain documentation, sprint tracking, deployment, CI/CD, ops, support and the list goes on and on.

I finally decided to write this all down once for myself so instead of trying to remember all the things, I would just have a checklist of things to follow in a timely order and I wouldn't miss something cruicial. 

# Who is this for ?

Take a look at the following scenarios

1. I am a Product Owner of a fresh startup, things are very crazy, no processes exist and no-one has a clear idea what is going on. Chaos everywhere.
2. I am an Engineer of a company in its initial stages, nobody has much experience, including myself, on how to build a tech project and what steps one should take care of.
3. I am a (somewhat) Senior engineer and this new startup is relying on me to setup their processes. The weight of the success of the entire product is on my shoulders; YES pressure.
4. I am starting my own software venture and I want to make sure that I don't overthink a lof ot things or ignore some cruicial things that may bite me in the future

If any of the above things apply to you, then this document can guide you. Obviously this is not a silver bullet, it reflects most of my personal choices and recommendations that have catered to my needs in the past. Based on experiences, I have come across a [commmon pattern](pattern); and if this pattern was common among 6 of the startups that I was acquinted with in the past plus my friends who are also currently struggling and working in startups, chances are you might also have come across this infamous pattern. So the aim of this document is to address this.


# How to read this
For terminologies, refer to [Wiki page for Glossary](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary).

## Quick Legend

### [Epoch](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#epoch)

- Step 1
- Early
- Later
- Post Live

### [Scope](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#scope)

- (__P__)rototype
- (__S__)mall
- (__M__)edium
- (__L__)arge


# <a name="list-index">Index</a>

## Aspects

### Preparatory homework

Lets get this party started

* [Getting Started](#getting_started)
* [Methodologies & Frameworks](#tools)

### Tooling

> A man is only good as his tools

* [Development Tools](#dev_tools)
* [Project Management](#project_management)
* [CI/CD & Deployments](#ci_cd)
* [Team Communication]()
* [Version control](#)
* [Monitoring](#)

### Quality

> Anything worth doing is worth doing right the first time

* [Environments](#envs)
* [Testing & Quality Control](#tools)
* [Tech Debt](#)
* [Documentation & Reporting](#tools)


### Cherry-on-top

> Ice cream tastes better with a cherry on top

* [System Security]()
* [Refactoring]()
* [User Studies]()
* [System Backups]()
* [Support & Disaster recovery]()
* [Licensing](#)
* [Community](#)

## Getting started [&#8593;](#list-index)

### What is this :

Somethings you need to ask yourself before you jump into the venture. You need to be absolutely sure about answering the ultimate question; *What is the problem you are trying to solve here*. Think outside the box, come up with anykind of way on how you want to come up with an answer to this, ask more poeple or search online. Basically do extensive research here. This is the part where you commit yourself to your idea. And you need to be 100% vested into it.

### Timeline

| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Requirements   | Step-1   |      P/S/M/L       |Sit down with yourself and answer the question: What are you trying to solve ? How do you plan to do it, and what is the [Definition Of Done](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#definition-of-done) ?|
| Market research   | Step-1  |     P/S/M/L         |Research about existing solutions out there. How does your solution differentiate? What is the Competition out there looking like.|
| Cost Analysis   | Early      |     M/L     |What is the status of your pocket looking like vs what you plan to achieve.|
| Interview people   | Post Live  |   M/L            |Ask relavant people out in the market what they think about your solution. Would anyone invest time and money in your idea?|

## Development Tools [&#8593;](#list-index)

### What is this ?

The tools are an extension of your creative mind. Your project will materialize from these tools and your idea will manifest into something physical using these tools. Choose wisely.

### Timeline

| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| IDEs   | Step-1   |      P/S/M/L       |Whether a single person or a team of engineers, find a tool that you are familiar with. Favor community based free and open source ones.
| Licensing   | Later   |      S/M/L       |Lots of libraries and tools out there are not exactly freen & open source. Some require certain policies and rules to be followed. Avoid unnecessary legal battles by addressing this early|


## Project Management [&#8593;](#list-index)

### What is this ?
A way of managing and visualizing incoming work and outgoing results. Visualizations and demographics are far more interesting and tell a lot as compared to mediocre emails and chat messages.

### Timeline

| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Ticketing System   | Step-1   |      P/S/M/L       |A good ticket management system to manage and structure tasks. Cheap tools exist|
| Product Owner   | Step-1   |      S/M/L       |Someone with the business knowledge. What are we making and how to manage time-lines of making this product.|
| Work flows  | Early   |      M/L       |What needs to be done first? Set priorities. What comes next? How does a working task move forward in e.g swimlanes of a kanban baord|
| Customer Support  | Later   |      M/L       |Find a way to manage feedback coming in from customrs and/or market to keep users happy|
| Professional Project Managers  | Early   |      M/L       |Invest in good and certified professionals to help you manage your project better.|


## CI/CD & Deployments

### What is this ?

During the course of development, a lot scripts and hacks are created on how to 'build' the code base and how to make it run. The famous [it works on my machine](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#definition-of-done) mindset is what needs to be avoided at all costs. The goal needs to come up with a strategy whereby the entire codebase can be buit and deployed without any manual intervention and something that is reporducable on any/all possible environments and hardware.

### Timeline

|What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Manual scripts   | Step-1   |      P/S/M/L       |Write unix compatible scipts of all things you do to build your code. All OS out there now support `/bin/sh` so you don't have to worry about support|
| Code builder   | Step-1   |      S/M/L       |A [tool](recommendation) to build your code without your intervention|
| Code Deployer   | Step-1   |      P/S/M/L       |A [tool](recommendation) that deploys your code without your intervention|


## Environments

### What is this ?

Overtime, you need a cloud based env where you can showcase your product, how it works, how you can interact with it, how other teams can see how well different components work together. A kind of a tricky thing to decide from the start since this can easily turn into a money drain if not chosen wisely.


### Timeline

|What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| All purpose stage   | Step-1   |      P       |Money is tight, time is precious, investors are waiting to see something quick. This env can act as your development, early release, stage and demo at the same time|
| Development   | Early   |      P/S/M/L       |Nice to seperate it out at an early stage but also means you have to spend some extra money on a demo and/or a live environment. Also important to have once dev team starts to grow. Dev is break-able, so the over-all expectations from this env should be adjusted|
| Testing   | Later   |      S/M/L       |A relatively stable env compared to the development, where people can see a feature or group of features and/or bugs working together in harmony. Not a break-able env|
| Staging   | Early   |      S/M/L       |You want to get the money from the investors, this is supposed to the the most stable env before production. Code works here. All configs are perfectly set. The URL works. The env works, investors are to be impressed.|
| Demo per tenant   | Later   |      L       |Once you grow, you want to have different settings/features for different user-base over your product. Makes sense to have seperate env per each user-base of tenant|
| Production   | Early   |      S/M/L       |Stable, non-breakable, resilient and performant env. Users are using this. This is the face of your product. Money will be made by this|
| Production per tenant   | Post Live   |      L       |Similar to demo per tenant, if the need arises, a per tenant seperate production system can be made. Features, bugs or load on one tenant will not affect other tenants|
| System on System   | Early   |      M/L       |To gain most user trust, showcase your product by running on your own systems. Examples of such products can be logging infrastructures or monitoring frameworks. This env is more of a show-case, non-breakable. You will impress more audience by showcasing it and gainging the trust of more people.|


## Testing & Quality Control

### What is this ?

The famous [Testing Pyramid](https://martinfowler.com/bliki/TestPyramid.html) can be a good starting point to find a good balance between speed, precision and scope of various test suites. 

### Timeline

| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Code Quality   | Early   |      S/M/L       |Delivered product is only as good as the codebase that makes it up. A good quality code base maybe defined by something that is low on [technical debt](https://martinfowler.com/bliki/TechnicalDebt.html), high on [code coverage](https://martinfowler.com/bliki/TestCoverage.html), follows [best pratices]() and is free from [CVEs](https://cve.mitre.org/)  |
| [Smoke testing](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#smoke-testing)   | Step-1   |      P/S/M/L       |Extremely basic testing to make sure system is working at the core.  |
| Developer testing   | Early   |      P/S/M/L       |Most commonly referred to as Unit-testing and Integration testing. 100% automated and dev team is responsible for writing and maintaining them |
| Modular/Functional testing   | Later   |     S/M/L       |Group of tests, normally a team other than developers, execute to make sure more cases are covered and the delivered product is meeting all expectations from the customers and adhering to the [quality gates](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#smoke-testing) |
| Load & [Stress]() testing   | Post Live   |      M/L       | How much amount of load i.e users, traffic or any quantifiable entity can the system sustain without affecting [SLAs](). The maximum threshold, after which the perfomance of the system is compromised is recorded as the stress point of system under load|
| End to End testing   | Later   |      M/L       |A set of automated tests that cover [business use case]() of a complex system. Usually very high level tests that simulate actually user interaction from UI. May require more time to execute|


## Methodologies & Frameworks

### What is this ?

A methodology can be best define as what processes you would like to follow while e.g doing daily business, completing tasks or deploying to production. A good methodology can be defined as one that suits your team, is flexible enough to adapt changes and is dynamic when it comes to tweaks. 

### Timeline

| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Working methodology   | Step-1   |      P/S/M/L       |Opt for something that is [flexible](). As a member of a team, you should be able to answer the following questions at any point in time; what is being worked on? What is planned next? What are our challenges?|
| DevOps methodology   | Early   |      S/M/L       |Deploy fast. Not only your codebase and product, but also the  infrastructure hosting your codebase. |
| Testing methodology   | Early   |     S/M/L       |Various layers can be adopted in parallel, best practices suggest adopting [fail fast]() strategies.|


## Team Communication

### What is this ?

A good team can become an awesome one when transparent communication lines exist in all dimensions, horizontally across teams on the same level and vertically across management hierarchy.

### Timeline
| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Riding the elevator   | Early   |      M/L       |A good example of such communication can be defined by the [Architect Elevator](https://martinfowler.com/articles/architect-elevator.html) concept which can be customized to fit entire team instead of just one person.|
| Product Owners   | Early   |      S/M/L       |the goal should be to empower everyone to think more in the direction of owning the product rather than working on a project. The aim should be to enable everyone to become a product owner.|


## Version control
### What is this ?

A way to collabrate with other team members while maintaining versions of your codebase

### Timeline
| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Raw code base   | Step-1   |      P/S/M/L       |Keep codebase in version control system. Follow best practices when it comes to [branching strategies](). No matter team size, no matter project size.|
| Infrastructure as a Code   | Step-1   |      P/S/M/L       | Follow best practices to version control your [IaaS]() alongside your |
| Environment setup & configs   | Step-1   |      P/S/M/L       | Follow best practices to version control your [IaaS]() alongside your |
| Test suites   | Step-1   |      P/S/M/L       | Follow best practices to version control your [IaaS]() alongside your |

## Monitoring
### What is this ?

> Applications running in the cloud (and on prem) tend to misbehave the minute you stop looking at them. 
-- Cloud for dummies

On the other hand, you can't always maintain an ssh connection to each and every deployement of your product. What you need is a really good monitoring infrastructure in place, something that will allow you to navigate to any point in time and enable you to drill down to any time of you your system. The mindset needs to be of Murphy's law; anything that can happen, will happen 


### Timeline
| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Infrastructure   | Step-1   |      S/M/L       |The monitoring infrastrcuture needs to be kept seperate and as far from the product infra as possible. If the product infra is affected, you still want your monitoring infra to be available. You don't want to end up being blind when something wrong is happening. Opt for [free tools]()|
| System monitoring   | Step-1   |      P/S/M/L       |In larger teams, track must be kept on who is doing what to which system and when. A solid audit monitoring system will help in this regard|
| Audit monitoring   | Later   |      M/L       |In larger teams, track must be kept on who is doing what to which system and when. A solid audit monitoring system will help in this regard and save you a lot of time and struggle|



## Tech Debt
### What is this ?

Best described as [days to fix problems](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#tech-debt) in a project. Something that is un-avoidable and will accumalate over time. The idea is to have a good balance between not letting it explode and not compromising feature development.

### Timeline
| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Measure   | Step-1   |      P/S/M/L       |No need to invent your own measure, there are tools out there that measure this for you. I personally [recommend](), since it does all of this automagically over the background.|
| Resolving strategy   | Later   |      S/M/L       | In theory, tech debt should be addressed at the earliest possible time. In practical, there is not definition of 'earliest possible'. Scrum teams usually keep a percentage threshold that if tech debt crosses X%, then the next sprint will be [house keeping sprint]()|

## Documentation & Reporting
### What is this ?

> If you have to explain it to a 5yr old, you are not clear enough

It's a bit of a strech to apply the same quote on something technical, surely the chances of a 5yr old understanding what is Memoization are a bit low, but the concept of proper documentation does NOT only apply to code bases. Your processes, scrum, testing strategies, building block views, architecture, more-tech-jargen etc all need to be documented. There are numerous documenting strategies that people use out there. Most of them are even template based, don't aim to write everything on day one. And best strategy could be summed as below

* A new team member can read through it and get a good gist of what is going on
* A non-tech person can see diagrams and have an understanding of work flows
* Outside organization people can grasp what you are doing below the surface
* Your grandma can be proud that you use the computer for something more than gaming !

### Timeline
| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Strategy   | Step-1   |      P/S/M/L       |My [personal favourite is this](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#arc42) one. It promotes evolutionary documentation and is very concise and complete|
| Building block views   | Step-1   |      P/S/M/L       |Blobs of text might fill more area on a (virtual) paper but diagrams will always explain more. A picture is worth a thousand words, draw it out ! What is connected to what, where and how. I recommend using [this template](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#c4)|
| Architecture & Design Decisions   | Early   |      P/S/M/L       | Often certain decisions have to be taken, that will affect future decisions. Whether code-base, architectural or design, document them seperately so they are easy to find|
