# Venture Timeline

A chronological arrangement of list of things to take care of when starting a venture.

# Background

Working in the software industry, I often came across a situation where a green field project needed to be setup. This meant, figuring out what kind of tools to use, how to maintain documentation, sprint tracking, deployment, CI/CD, ops, support and the list goes on and on.

I finally decided to write this all down once for myself so instead of trying to remember all the things, I would just have a checklist of things to follow in a timely order and I wouldn't miss something cruicial. The numbering of the [list items](#list-index) does not signify any ordering, any step can be done in any order. The scope is what matters more i.e what to do at which stage of the project.


# How to read this
For terminologies, refer to [Wiki page for Gloassry](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary).


# <a name="list-index">Index</a>
* [Getting Started](#getting_started)
* [Development Tools](#dev_tools)
* [Project Management](#project_management)
* [CI/CD & Deployments](#ci_cd)
* [Environments](#envs)
* [Testing & Quality Control](#tools)
* [Tech Debt](#)
* [Documentation & Reporting](#tools)
* [Team Communication]()
* [System Security]()
* [User Studies]()
* [System Backups]()
* [Support & Disaster recovery]()
* [Methodologies & Frameworks](#tools)
* [Monitoring](#)
* [Licensing](#)
* [Version control](#)


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
| Licensing   | Early   |      S/M/L       |Lots of libraries and tools out there are not exactly freen & open source. Some require certain policies and rules to be followed. Avoid unnecessary legal battles by addressing this early|


## Project Management [&#8593;](#list-index)

### What is this ?
A way of managing and visualizing incoming work and outgoing results. Visualizations and demographics are far more interesting and tell a lot as compared to mediocre emails and chat messages.

### Timeline

| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Ticketing System   | Step-1   |      S/M/L       |A good ticket management system to manage and structure tasks. Cheap tools exist|
| Work flows  | Early   |      M/L       |What needs to be done first? Set priorities. What comes next? How does a working task move forward in e.g swimlanes of a kanban baord|
| Customer Support  | Later   |      M/L       |Find a way to manage feedback coming in from customrs and/or market to keep users happy|
| Professional Project Managers  | Early   |      M/L       |Invest in good and certified professionals to help you manage your project better.|


## CI/CD & Deployments

### What is this ?

During the course of development, a lot scripts and hacks are created on how to 'build' the code base and how to make it run. The famous [it works on my machine](https://github.com/MSaifAsif/venture_timeline/wiki/Glossary#definition-of-done) mindset is what needs to be avoided at all costs. The goal needs to come up with a strategy whereby the entire codebase can be buit and deployed without any manual intervention and something that is reporducable on any/all possible environments and hardware.

### Timeline

| What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| Code build   | Step-1   |      P/S/M/L       |A tool that builds your code without your intervention|
| Code Deployer   | Step-1   |      P/S/M/L       |A tool that deploys your code without your intervention|


## Environments

### What is this ?

Overtime, you need a cloud based env where you can showcase your product, how it works, how you can interact with it, how other teams can see how well different components work together. A kind of a tricky thing to decide from the start since this can easily turn into a money drain if not chosen wisely.


### Timeline

 What To Do | Epoch | Scope    | How To Do          |
| ------- | ------|--------------- |--------------|
| All purpose stage   | Step-1   |      P       |Money is tight, time is precious, investors are waiting to see something quick. This env can act as your development, early release, stage and demo at the same time|
| Development   | Early   |      P/S/M/L       |Nice to seperate it out at an early stage but also means you have to spend some extra money on a demo and/or a live environment. Also important to have once dev team starts to grow. [Dev is break-able](sss), so the over-all expectations from this env should be adjusted|
| Testing   | Later   |      S/M/L       |A relatively stable env compared to the development, where people can see a feature or group of features and/or bugs working together in harmony. Not a break-able env|
| Staging   | Early   |      S/M/L       |You want to get the money from the investors, this is supposed to the the most stable env before production. Code works here. All configs are perfectly set. The URL works. The env works, investors are to be impressed.|
| Demo per tenant   | Later   |      L       |Once you grow, you want to have different settings/features for different user-base over your product. Makes sense to have seperate env per each user-base of tenant|
| Production   | Early   |      S/M/L       |Stable, non-breakable, resilient and performant env. Users are using this. This is the face of your product. Money will be made by this|
| Production per tenant   | Post Live   |      L       |Similar to demo per tenant, if the need arises, a per tenant seperate production system can be made. Features, bugs or load on one tenant will not affect other tenants|
| System on System   | Early   |      M/L       |To gain most user trust, showcase your product by running on your own systems. Examples of such products can be logging infrastructures or monitoring frameworks. This env is more of a show-case, non-breakable. You will impress more audience by showcasing it and gainging the trust of more people.|


## Testing & Quality Control

### What is this ?
...
### Timeline
/...