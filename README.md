<img width="603" alt="image" src="https://github.com/boyney123/complexity-is-the-gotcha-of-event-driven-architecture/assets/3268013/90508a06-604a-4956-ad42-b7b70b3514fe">

---

_Here you can find resources for the talk "Complexity is the gotcha of event-driven architecture"_

## Potential of EDA

### Static vs Evolutionary:
- Static architectures anchor us, may slow us down, and can appear from nowhere.
- Risk of static architectures as we face the **Project paradox**, this is where we make decisions up front without the knowledge we may need.
- We can use EDA to defer decisions to later, with abstractions and a evolutionary architecture.
- Many businesses are looking for speed and agility this year ([view the report](https://www.gartner.com/en/information-technology/technology-adoption-roadmap)), EDA can help us here.
- EDA helps us build loosely coupled, high cohesion, a platform to experiment and team dependency
- One major problem is that evolutionary architecture increases complexity.

### Links
- [The project paradox](https://beyond-agility.com/project-paradox/) - Why is it that many decisions are made up front when we start projects, but our knowledge increases over time? Maybe we should push decisions back when we have more knowledge, we can do this with event-driven architectures. Here is a blog post on learning more about the **project paradox**
- [Building Evolutionary Architectures: Principles & Practices](https://www.youtube.com/watch?v=jTX45V5JuN4) - Dive deeper with this talk from Rebecca Parsons

---

## Manage complexity with guardrails

There are three guardrails that can help you manage complexity:

- Behaviour first thinking
- Event evolution strategy
- Understanding coupling in events

### Behaviour first thinking

- As we build evolutionary architectures, without managing complexity you are at risk [creating a big ball of mud](https://eda-visuals.boyney.io/visuals/avoid-big-ball-of-mud).

<img width="566" alt="image" src="https://github.com/boyney123/complexity-is-the-gotcha-of-event-driven-architecture/assets/3268013/effaca9d-a1ee-49c7-ba5e-d6358afb87fc">

- Complexity grows over time, as we add nodes the number of channels increase. So we lean into EDA to control the channels between the nodes.
- But even with these managed channels, complexity lies within the details.
-  Highly recommend favouring behaviour over implementation details. You can use [EventStorming](https://www.eventstorming.com/) to help you identify domains, boundaries, events and more!

### Event evolution strategy

- Events will evolve as you understand more about your domain, you need to have a strategy in place on your teams to manage versioning.
- In this talk we discussed **Backwards compatibility**, **Optional new fields** and **Parallel versions**.
- Remember to understand [Postels Law](https://en.wikipedia.org/wiki/Robustness_principle), be conservative in what you do and liberal in what you accept from others.

### Complexity with consumers

- How you consume events can couple you, understand what options you have.
- Look at [bounded context mappings](https://eda-visuals.boyney.io/visuals/bounded-context-with-event-architectures), these can help you.
- Remember the level of communication required between teams increases depending on which bounded context mapping you choose.

### Links
- [Journey to event-driven architecture](https://www.youtube.com/watch?v=hvGuqHp051c) - Previous talk I did at re:Invent 2023 about how and where you should get started with EDA. This goes into many various aspects of EDA, and patterns to help you build an EDA.
- [EventStorming](https://www.eventstorming.com/) - Explore event storming to help you identify events, domains, services and much more! Start here before building your EDA, understand behavior first.

---

## Biggest gotcha of them all

Regardless of what you do, you will hit this problem. The fact we take this saying way to literraly in EDA, that producers should not know about consumers. 
This can lead to issues.

### Producers should not know about consumers

- Every article out there will suggest this, although technically correct, you need to understand the importance of governance.
- Common questions will come over time, "What events do we have?", "What’s the payload of these events?", "Who is consuming this event?", many people face this.
- Explore standards to help you overcome these issues.
- Use [CloudEvents](https://cloudevents.io/) to define standards in your events.
- Use [AsyncAPI](https://www.asyncapi.com/) to help document your EDA.
- Explore how [EventCatalog](https://www.eventcatalog.dev/) can help you take this further, visualize your events, and build a static website for your EDA.

### Links
- Join [EventCatalog community](https://discord.com/invite/3rjaZMmrAm). I'm looking to build v2 of EventCatalog and help people document their EDA, but I can't do this on my own. Join the project let's fix the issue!

# Summary

- To get the full potenital of EDA you need to manage complexity.
- Put guardrails in place to manage complexity over time.
- Complexity comes in all shapes, there is no avoiding it, but you can manage it.

---

## EDA Visuals

Want to learn more about EDA? Then you can [download my free book about EDA](https://eda-visuals.boyney.io/). Over 60 bite sized visuals to help you learn more about event-driven architecture.

![image](https://github.com/boyney123/complexity-is-the-gotcha-of-event-driven-architecture/assets/3268013/138a303f-48d9-4a3c-bbe6-f4b9c75651b9)

## Want more?

Want to learn more, I have a [few more talks on my website](https://www.boyney.io/talks) that can help you dive into EDA.

<img width="610" alt="image" src="https://github.com/boyney123/complexity-is-the-gotcha-of-event-driven-architecture/assets/3268013/91a0da5b-08c2-4379-bdc4-46a943bc2615">

## EventCatalog v2

EventCatalog helps you document your event-driven architectures. 

I am currently working on v2 with many more features, new framework, support for 1000s of events and much more. 

EventCatalog v2 also comes with enterprise features and support. If this is something you are interested in [please get in contact](https://www.linkedin.com/in/david-boyne/), I would love to understand your problems and how EventCatalog may be able to help.

![image](https://github.com/boyney123/complexity-is-the-gotcha-of-event-driven-architecture/assets/3268013/b4c747a3-0d79-4b8e-be69-b09c04c30723)



Reach out to me if you would like me to run this talk at your event.

Thanks!
