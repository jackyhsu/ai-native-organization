# We Thought We Didn’t Need Engineers—Until We Found a 30,000-Line File

English | [中文](../zh-CN/stories/002-we-thought-we-didnt-need-engineers.md)

**Status: 💥 Failed**

**By Jacky Hsu**

For a short period, we believed we might not need engineers.

The belief did not come from a presentation about the future of work. It came from watching software appear far faster than we thought possible.

Ingora began with two senior product and technology leaders carrying much of the product direction. We had spent years making product, platform, and technology decisions, but neither of us had recently built a mobile application from zero. We understood the map. We no longer had all the muscle memory required to walk every part of it.

That was one reason an outsourced engineering team made sense at the beginning. The team could build. The problem was that an early startup does not only need software delivery; it needs to turn uncertain ideas into things users can test, then change or discard those ideas immediately.

Every handoff added waiting. Every new test looked like a scope change.

Then AI lowered the cost of crossing the boundary ourselves.

During one hotel stay, I asked Codex to establish an Android development environment and build a rough application connected to a real-time voice model. The result was only a prototype, but it ran. I had not become an Android expert. I had become able to test a product judgment without waiting until I was one.

Soon afterward, my cofounder went much further. Using Codex for approximately three weeks, one person recreated much of the work that an outsourced team of more than ten people had spent roughly three months building, while adding other ideas we wanted to test.

This was **not a controlled productivity benchmark**. The scope, quality bar, engineering discipline, and long-term maintenance requirements were different. The AI-assisted version contained bugs and obvious signs of rapid vibe coding.

But for an early startup, it changed the time between a hypothesis and a user test from weeks to hours or days.

The feeling was intoxicating.

My cofounder said something close to: “It feels like we can build anything. Maybe we do not need engineers.”

The first sentence was partly true.

The second was dangerous.

## Every local answer looked reasonable

At first, the failures seemed small.

One feature broke, so we asked AI to repair it. The repair worked, but another feature failed. We repaired that one, and an earlier problem returned. Each conversation produced a confident explanation and a plausible patch. Locally, the answers often made sense. Globally, the product was becoming harder to understand.

During this period, we rarely opened the IDE or inspected the structure closely. The workflow felt too smooth: describe the feature, wait for generation, install the application, test what appeared on the screen. If it worked, we moved on.

Eventually, adding one more feature no longer felt safe. We opened the Android codebase for a serious inspection.

More than 30,000 lines of front-end code had accumulated in a single file.

There were no clear module boundaries. Calls to back-end services appeared in multiple places. A state change could affect features that looked unrelated. Each “quick fix” may have been a reasonable response to the immediate request, while making the whole system less maintainable.

The problem was not that the model had never heard of modularity, architecture, testing, or separation of concerns. If asked to explain those principles, it could do so very well.

The problem was the job we had given it.

We repeatedly asked for the next button, connection, feature, or fix. We had not given the system a durable architecture, sufficient context, or a development process that made long-term consistency part of every task. AI optimized for the visible success of the current request. No one was consistently responsible for the shape of the system after the next hundred requests.

Knowledge inside a model does not automatically become a constraint on the work.

## What we learned

AI dramatically raised the floor of what two experienced non-coders could build. It did not automatically raise the ceiling of what we could maintain as a reliable product.

Generating code and engineering a system are different activities.

Engineering includes deciding where boundaries belong, which shortcuts will collect interest later, what must be tested, and when a seemingly useful change should be rejected. Those judgments become more important—not less—when code can be produced quickly.

We changed direction. The answer was not simply a stronger model. We needed engineering judgment and an environment in which architecture, tests, review, and feedback constrained every change. We also needed engineers.

The episode changed our question from “Can AI write the code?” to “What system helps humans and AI keep the product coherent while both move quickly?”

## The next test

Speed helped us discover that our original development arrangement was too slow. Then speed helped us create a different failure.

The next experiment is to see whether every failure can become a durable constraint: a test, a rule, an architectural boundary, or a review trigger that reduces the chance of repeating the same class of mistake.

AI made it possible for us to build before we had rebuilt our engineering organization.

The 30,000-line file reminded us why an engineering organization exists.

---

Return to the [Experiment Roadmap](../roadmap/experiments.md).

[Star the repository](https://github.com/jackyhsu/ai-native-organization) to follow the next experiment.
