# 001 Why Installing Copilot Still Doesn’t Make a Company AI-Native

English | [中文](../zh-CN/stories/001-why-copilot-is-not-ai-native.md)

**By Jacky Hsu**

Copilot is not obsolete.

What is obsolete is treating Copilot as the destination.

When [GitHub first released Copilot](https://github.blog/news-insights/product-news/introducing-github-copilot-ai-pair-programmer/) in 2021, it called the product an “AI pair programmer.” It read the code a developer was writing and suggested the next line—or even an entire function—as the developer typed. “Copilot” soon became the name for a whole category of generative AI products: the person sits in the driver’s seat, chooses the direction, controls the speed, and remains accountable for the result; AI sits beside them, offering suggestions and helping with the work.

At the time, this was both an advanced and necessary design.

Early large language models could produce astonishing answers and make confident mistakes. They could complete local tasks but struggled to retain context over time. They could offer advice but were not yet suited to holding system permissions or independently executing a sequence of actions. Keeping the human at the wheel and the AI beside them matched both the models’ capabilities and people’s expectations of responsibility and safety.

Copilot answered the most important question of that era: how can AI help a person do the same work faster?

But it also quietly preserved an assumption that few people questioned: the work itself would remain unchanged.

The company would still be the same company. Departments, roles, applications, approval processes, and reporting lines would all remain in place. Salespeople would work in the same CRM. Product managers would write requirements in the same documents. Engineers would code in the same development environment. Managers would continue waiting for information to be summarized layer by layer. We had simply put a copilot beside every person.

It was like giving every car a more powerful engine in a city that was gridlocked every day.

Each car could go faster. The city might not.

## What does the copilot model conceal?

When the human is the driver and AI is the copilot, the basic syntax of work remains:

> A person discovers a task → gathers the context → asks AI for help → copies the result → hands it to the next person

AI can make the “help” stage extremely fast. It does not automatically remove the wait before a task is noticed, the movement of context between systems, the handoffs between departments, or the review and execution that follow the result.

It optimizes one node, not necessarily the whole chain.

That is why a company can buy AI tools for every employee—and employees can genuinely write, summarize, and make presentations faster—while management feels no increase in the speed of the company as a whole. Sometimes the opposite happens. AI produces a flood of drafts, proposals, and code, and the queue in front of reviewers grows longer. The bottleneck moves from production to judgment.

One sentence captures the contradiction:

> Local efficiency is not organizational efficiency.

```mermaid
flowchart LR
    A[A person discovers a task] --> B[A person gathers context]
    B --> C[AI provides assistance]
    C --> D[A person copies and reviews]
    D --> E[A person hands it off]
```

A product manager generating ten requirement drafts in a day does not mean the engineering team can deliver ten more features. A salesperson quickly writing one hundred outreach messages does not mean the company suddenly has the capacity to handle one hundred leads. Engineers producing more code does not mean that code has been properly reviewed, tested, deployed, or used to create value for customers.

When AI strengthens the pump, the first result is often not a wider river. It is a flood downstream.

So the question for measuring AI cannot simply be, “How much time did one person save?” The more important question is whether that saved time traveled through the whole workflow and became a faster or better result—or enabled a result that was previously impossible.

If it did not, Copilot merely made the old process run harder.

## “Less than 1%” is a warning, not a statistic

Many people still use generative AI by opening a chat box, asking a question, waiting for an answer, and copying that answer into another application. The model has no long-term company memory. It does not know the history behind a decision, cannot continuously watch the outside world, and lacks permission to carry out the next action. When each conversation ends, the temporary team that a person and AI had just formed dissolves.

If we call someone who can use memory, tools, and multiple agents—working in parallel, checking results, and iterating from feedback—a “super individual,” it is tempting to say that most people may not yet be using even 1% of that capability.

But we need to be precise: “less than 1%” is not a measurable statistic about individual ability. It is better understood as a warning. Do not mistake an occasional conversation or a generated piece of copy for the upper limit of generative AI.

A more dependable reference exists at the organizational level. [In late 2024, McKinsey surveyed 238 executives and 3,613 employees](https://www.mckinsey.com/capabilities/tech-and-ai/our-insights/superagency-in-the-workplace-empowering-people-to-unlock-ais-full-potential-at-work/). Although almost every company was investing in AI, only 1% of leaders considered their organizations mature in AI deployment—meaning that AI was fully integrated into workflows and producing substantial business outcomes.

The scarce resource is not a model account. It is a method for connecting models to work.

A model supplies possibility. Turning that possibility into productivity also requires context, memory, permissions, tools, acceptance criteria, and feedback loops. Without them, even the strongest model must wait for a person to feed it each task. With them, the same model can begin to move from answering questions to owning outcomes.

That explains why two people using exactly the same AI may not differ by 20% versus 30%, but by an order of magnitude.

One person is waiting for an answer.

The other is orchestrating work.

## What does “400×” actually tell us?

Y Combinator president and CEO Garry Tan once compared his GitHub activity in 2013 and 2026 in a public talk, describing the change in output brought by AI as “roughly 400×.” It is a highly memorable number—and easily misread as a claim that AI can make everyone 400 times as productive.

It was not a rigorous productivity experiment.

Lines of code do not equal product value, and different years, projects, and languages cannot be compared directly. Tan later updated the calculation in his public [gstack project](https://github.com/garrytan/gstack), using logical code changes rather than raw line counts and explicitly noting limitations such as AI-generated code inflation. By his published method at the time, the annualized 2026 rate was about 810 times his 2013 rate. But he also stressed that the point was not how many lines anyone typed. The point was what shipped.

So 400, 800, or any other precise multiplier is not the important conclusion here.

What matters is that Tan did not merely place a chatbot next to his editor and type faster. He organized roles including product thinking, design, engineering management, code review, testing, security, and release into a virtual team that could be invoked and could check its own work. AI did not just answer, “How should I write this code?” It was placed inside a workflow from intent to delivery.

That echoes the new syntax of work described by CSDN founder Jiang Tao in his writing on silicon time:

> A person expresses intent → an agent understands and plans → agents execute in parallel → the person reviews the result → feedback is given.

The difference between two people using AI is not merely that one writes better prompts.

One treats AI as a source of answers. The other organizes AI into a production system.

A “super individual,” then, is not someone who can use many AI tools at once. It is someone who can translate intent into a network of tasks, let machines carry the execution, return evidence to human judgment, and avoid drowning in the information those machines produce. What founders lack is not another AI tool. It is an operating system for running the company.

## The unit of productivity has changed

Traditional companies measure capability through headcount, hours, and roles. One person has eight hours in a workday. A team has ten people. A piece of work passes through product, design, engineering, testing, and operations. The usual way to expand capability is to add people, then add layers of management to connect them.

Copilot extends this production function. A person remains one unit of labor, but can complete a little more work each hour with AI beside them.

An AI-native organization suggests another possibility. A person no longer maps to a single role. They become a source of intent, an orchestrator of agents, and an arbiter of results. Multiple agents can work on research, design, development, and validation at the same time. The knowledge a task needs does not have to be re-explained at every handoff; organizational memory can supply it continuously. Errors and feedback produced during execution can then improve the next run.

Output is no longer determined only by how many people work for how long. It also depends on the quality of human judgment, how much silicon time can be orchestrated, how many tasks can run in parallel, and how fast the feedback loops move.

The deepest change is not that the same person works faster.

It is that the subject of the work has changed.

The old pattern was “people complete tasks and AI helps.” More work will follow a different pattern: “AI executes tasks; people define intent, set boundaries, inspect evidence, and bear responsibility.” Humans do not leave the loop, but they no longer have to hold every turn. We call this position `Human on the Loop`: the person moves from step-by-step operation to supervision and arbitration.

This does not mean every task should be automated, or that AI should receive unlimited permissions. The opposite is true. As machines gain the ability to take more actions, the boundaries of human responsibility, stop conditions, and traceability must be designed more clearly.

Autonomy is not abandonment.

Real autonomy means not waiting for a push at every step while operating inside explicit boundaries.

## A company is not an old car with a turbocharger

Speaking about “Founder Mode” at YC Startup School, Jensen Huang offered a metaphor closer to an AI-native organization than the copilot model:

> A CEO is like an F1 driver. A founder is building the race car they will drive—and tailoring it to how they drive best.

The metaphor matters not because founders should control every detail, but because a company has never been a standard vehicle independent of its driver.

The steering, aerodynamics, suspension, tires, and pit crew are not separate tools. Together they form a system designed for a specific objective, track, and driving style. Replacing only the engine with a more powerful one may make the whole car harder to control. Copying another driver’s setup may not suit you.

The same is true of an AI-native company.

If a company’s advantage comes from a founder’s distinctive judgment about users, products, and risk, AI should not copy a generic set of “best practices.” Nor should it trap the founder at every approval point. It should allow that judgment to be expressed, preserved, and invoked so that it can shape more decisions.

The founder should not remain a bottleneck the company can never bypass. But the company should become a machine that amplifies the founder’s judgment.

This is the deepest divide between Copilot and AI-native.

Copilot assumes that the vehicle has already been built and needs a smarter passenger.

AI-native requires us to redesign the entire race car. Which signals should enter automatically? Which knowledge should persist? Which tasks can run in parallel? How will results be verified? When must a person take over? How should one failure improve the next run?

The question is no longer how one tool can help one role. It is how a company should operate.

## A harsh but useful test

To judge whether a company is AI-native, try a harsh thought experiment:

> If AI disappeared today, would the company merely slow down—or would its essential methods of memory, coordination, and execution stop working?

If the organization could continue operating through the same roles, meetings, documents, and approval processes, with employees simply spending more time, then it is probably still in the “AI-augmented” stage. It uses AI but has not redesigned itself around AI’s capabilities.

If removing AI would stop external signals from entering continuously, prevent knowledge from being connected automatically, end parallel task decomposition, break the loop between feedback and code, and force the organization to hire many people and rebuild whole processes, then the company may be developing an AI-native structure.

Of course, dependence on AI is not itself an achievement. Fragile automation that cannot be explained or stopped can also become indispensable. A complete definition of AI-native must include human responsibility, verifiable results, and recoverable governance. We will continue testing those elements in later experiments.

But the thought experiment forces us to face one fact honestly:

Installing Copilot adds a capability to the old company. Becoming AI-native means deciding again what the company is made of.

The first asks: what can AI help employees do?

The second asks: when knowledge, reasoning, and execution can all be orchestrated, which work must still be performed step by step by people? Which departmental boundaries still need to exist? What should become the company’s long-term memory? Where in the process should human judgment appear?

This is not a software upgrade.

It is an upgrade to the organization’s foundational assumptions.

---

Previous: [000 The Founder Was Away. The Company Kept Growing](000-founder-away.md)

Next: [002 Why Saving 30% of Your Time Still Isn’t Enough](002-why-saving-30-percent-is-not-enough.md)

[Star the repository](https://github.com/jackyhsu/ai-native-organization) to follow the next experiment.
