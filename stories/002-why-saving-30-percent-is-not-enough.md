# 002 Why Saving 30% of Your Time Still Isn’t Enough

English | [中文](../zh-CN/stories/002-why-saving-30-percent-is-not-enough.md)

**By Jacky Hsu**

When my plane landed at Charles de Gaulle Airport in Paris, I turned on roaming and saw a message just one sentence long:

> It’s built. You can start testing.

I stared at the screen for a while.

Only a few hours earlier, before takeoff, I had discussed a new feature we wanted to test with my cofounder. In my head, I had already given it an optimistic timeline: if AI really helped, perhaps we could see a first version in three or four weeks.

Now I had just landed in Paris, and it was waiting for me to test.

I had traveled to speak at the GOSIM workshop. Before leaving, I had prepared to explain how AI was changing products and companies. But what changed my own understanding of an AI-native company was not a slide on the stage. It was the message I received at the airport.

For the first time, I saw clearly:

If we are still measuring AI by “how much time did it save?”, we may be asking the wrong question from the beginning.

## There is nothing wrong with 30%. It is simply too small.

When I worked on Microsoft Copilot, the most natural value proposition was to make employees more productive in their existing roles. If AI could organize information, summarize meetings, and produce a first draft—saving roughly 30% of the time on a task—that was already a compelling use case.

Public research later supported that direction. [Microsoft asked 147 participants](https://www.microsoft.com/en-us/worklab/work-trend-index/copilots-earliest-users-teach-us-about-generative-ai-at-work) to complete search, writing, and summarization tasks with or without Copilot. The Copilot group was 29% faster on average, with no significant difference found in accuracy or quality.

That result matters. It also makes it easy to stop there.

Being 29% faster means that a task that once took ten hours now takes about seven. The boundaries of the role remain mostly the same; execution simply speeds up. This is the “AI augmentation” described in 001: the driver, vehicle, and road all remain in place, while the copilot reduces some of the effort.

I brought the same mental model with me when I left Microsoft to start a company.

We would use AI, so we would be more efficient than previous startups. We would write documents faster, research markets faster, and build prototypes faster. If everyone improved by 30%, perhaps a ten-person company could produce what thirteen people once did.

That was already a good vision.

But what happened next did not feel like ten people becoming thirteen.

It felt as though the solid walls between roles had begun to disappear.

## We had judgment, but had lost the muscle memory of building

Before the company was formally established, our investor kindly proposed a fast-start mechanism: an outsourced team would begin software development before funding closed, key cofounders arrived, and the permanent team was recruited.

It was a sensible arrangement. A startup window does not wait for an organization chart to fill itself in. If we built the product first, we could test user reactions sooner.

After our first cofounder joined, only the two of us were carrying the product and technology direction. We were both veterans with one or two decades in technology, with experience in products, operations, strategy, and industry judgment. My cofounder had even led a team of around ninety people.

But we also had to admit an uncomfortable fact: we were a long way from our years of writing production code on the front line.

We understood how a mobile application was broadly assembled. We knew how cloud services, clients, and voice models needed to connect, and we could judge whether the user experience was good or bad. But to build an Android or iOS app from scratch, configure Azure and Alibaba Cloud resources, manage dependencies, run simulators, apply for an Apple developer account, and ship through TestFlight—we had concepts, not enough detailed practical ability.

We had a map, but neither of us had walked that road for a long time.

Outsourcing was therefore not a lazy choice. We believed it was a capability we had to buy.

We soon learned that buying “development capacity” was not the same as buying “the iteration capacity a startup needs.”

## The outsourcing team was not wrong. It was solving a different problem.

The speed and flexibility of the outsourced work gradually failed to meet our expectations. The first AI voice pipeline could run, but latency, interruptions, echo, and conversational naturalness were not good enough. More importantly, every new test direction came with a long wait between communication, scheduling, and a result we could see.

We needed to add a feature quickly to see whether children liked it. We needed to replace part of the voice pipeline to learn whether a bad experience came from the model, the network, or product design. We needed to abandon a poor result immediately instead of spending weeks developing it and then inventing reasons to defend the wrong direction.

Traditional software outsourcing seeks a different kind of certainty. Requirements are clarified first—ideally fixing the interface, interaction, and acceptance criteria—then person-days are estimated, development is scheduled, and delivery happens in stages. Constant scope changes usually mean uncontrolled costs, a broken plan, and unclear responsibility.

That process is not wrong.

But in an early-stage startup, the definition of the requirement is often not the input to development. It is the output of development and testing.

We do not know the right answer first and ask someone to build it. We must build several answers before we can know which one deserves to continue.

An outsourcing company sells “software completed to a definition.” At this stage, a startup needs to “use software to create the definition.”

The deepest conflict was not capability or attitude. It was the economics of waiting. For mature delivery, frequent change is waste. For a startup still exploring, waiting for validation is the largest waste of all.

Our meeting notes stated the problem directly: “The outsourced architecture limits iteration and prevents rapid validation of new features.” The team decided to begin an internal architecture and gradually replace the outsourced system.

Writing down that decision was easy.

We still had no engineers.

## The first boundary crossing, in a hotel room

The real turn began with a seemingly unrelated experience.

We had used Codex to install OpenClaw automatically. It did not merely tell me which commands to enter. It could inspect the environment, install dependencies, handle errors, and continue through the following steps. That gave me a bold idea: if it could prepare the runtime for unfamiliar software, could it also prepare a mobile development environment for me?

During a business trip, I decided to try from my hotel room.

I asked Codex to develop an Android application connected to what was then Azure Voice Live’s most advanced real-time voice model. I did not take an Android course first or spend days reading every SDK installation guide. Codex checked what was missing from my computer, installed development tools and packages, created the project, wrote code, ran the application, and handled problems along the way.

Before long, the Android application appeared in the simulator.

I spoke to it.

It answered smoothly.

As a product, it was still a rough prototype. From the company’s perspective, it crossed a capability boundary. A product leader who had not directly developed a mobile app in years completed a task that previously would have waited for an Android engineer—without first becoming one.

I did not suddenly learn every detail of Android development.

But I no longer had to learn every detail before I could begin testing a product judgment.

That hotel experiment became a catalyst in Ingora’s move toward an AI-native company.

## The message at Charles de Gaulle

Another extreme event made the change irreversible.

We asked the outsourcing team to test a new feature quickly, and they declined. From their perspective, it was another scope change. From ours, if we could not test a critical assumption, the company would keep moving in the dark.

My cofounder—who had led ninety people and had been away from hands-on development for years—faced a choice: keep waiting for someone else’s schedule, or build it himself.

He chose the latter.

Before I flew to Paris, I discussed a new test idea with him at the airport. Even with AI, I expected it to take three or four weeks. I lost access to domestic networks after takeoff. When the plane landed, the first message said: it is done; you can start testing.

That was only the beginning.

Before I returned from Paris, he had spent about three weeks working alone with Codex and had reimplemented the main work that an outsourced team of more than ten people had delivered over roughly three months. He also added many features we had long wanted to test.

We need to be honest: this was not a controlled engineering productivity experiment.

The two sides did not deliver identical scope, code quality, engineering standards, or long-term maintenance requirements. The rapidly AI-generated version showed obvious signs of vibe coding. The architecture had not been adequately planned; the code had many bugs; and testing, monitoring, security, and maintainability were far from a mature product. “Three weeks versus three months” cannot be turned into a repeatable productivity multiplier.

But for the startup at that moment, the metric that determined survival was not whether the code was already perfect.

It was whether we could finally turn a product hypothesis into something a user could experience within hours or days.

If the hypothesis was wrong, fail quickly.

If users did not respond, stop polishing it.

If the direction deserved to continue, then invest in engineering it properly.

Traditional processes try to reduce uncertainty during development. AI let us face uncertainty more cheaply. The first thing it changed was not the speed of writing code, but the speed at which the company could discover the truth.

We began to understand that a startup’s most important productivity measure is not how much code it writes per unit of time. It is how many wrong assumptions it eliminates.

## Stage one: do the same work faster

Looking back, our use of AI passed through three stages.

The first was the individual productivity gain represented by Copilot.

The role, task, and responsibility remain unchanged. AI helps with a first draft, a search, a meeting summary, or a piece of code. A product manager remains a product manager, a finance professional remains a finance professional, and an engineer remains an engineer. Each simply performs the same work faster.

This stage is the easiest to introduce and measure. A report that took three hours now takes two. A feature that took a week is written in four days. Thirty percent is the typical language of this stage.

It creates real value.

But it does not change how the organization makes the greatest use of capability.

If the company stops here, the old role boundaries, handoffs, and waits remain. Everyone hands work to the next person faster, then queues together at the next bottleneck.

## Stage two: one person crosses multiple functions

The second stage is not “doing more in the same role.” It is one person beginning to perform tasks that once belonged to different roles.

My cofounder went from carrying product, architecture, and management judgment to working across several functions:

- building Android and iOS applications like a developer;
- redesigning the system like an architect;
- deploying, configuring, and testing Azure and Alibaba Cloud resources like IT and cloud operations staff;
- reproducing problems and validating features like a test engineer;
- checking vulnerabilities, permissions, and AI compliance risks like a security and compliance specialist.

My own role was expanding rapidly too.

At Microsoft, I could focus mainly on product and strategy. After founding Ingora, I had to learn financing terminology and speak with investors; establish a Singapore parent company and a Chinese subsidiary and arrange corporate banking in both places; apply for domains and Microsoft 365 accounts; track industry news, regulation, and geopolitics; apply for an Apple developer account; find partners and hardware supply chains; speak at workshops; and apply for leadership programs with the founding team.

Eventually, I even had to empty the coffee grounds from the office machine.

Apart from that last task, I used AI to learn and seek guidance for almost every unfamiliar job—and in some cases let AI help perform it directly.

AI did not turn me overnight into a lawyer, accountant, cloud architect, or engineer. It lowered the threshold for entering an unfamiliar domain: explaining terminology, organizing steps, preparing materials, checking omissions, and acting directly when tools allowed. My role was no longer defined only by what I had been trained to do, but increasingly by what the company needed to solve at that moment.

This is the “super individual.”

A super individual is not someone who works exceptionally long hours or keeps ten chat windows open. It is a person with enough judgment to use AI to invoke capabilities once scattered across many roles and combine them toward one objective.

After completing the three-week development sprint, my cofounder told me:

> It feels like I can do anything. Maybe we don’t need engineers.

That feeling was very real.

It was also very dangerous.

## We are not deleting engineers. We are deleting tasks.

The rapid prototype showed that someone who had not coded directly for years could cross an old professional boundary with AI. Its bugs, confused architecture, and lack of testing demonstrated something equally important: producing code is not the same as building a reliable software system.

Engineers do not automatically lose their value because code becomes easy to generate. Quite the opposite. When code can be produced in volume, it becomes even more important to judge architecture, define boundary conditions, design tests, control permissions, respond to production incidents, and make systems maintainable over time.

Ingora later drew a direct distinction in its internal Agentic Engineering handbook: vibe coding raises the floor for “making something”; agentic engineering raises the ceiling for “turning it into a product.” The latter still requires specification design, plan supervision, diff review, testing strategy, and permission management.

So the more accurate claim is not “AI eliminates the engineering role.” It is:

> AI will first remove from the engineering role a set of tasks that previously had to be performed by hand.

The same change will affect product, operations, finance, legal, and management roles.

AI first removes information movement, format conversion, repetitive configuration, first-version generation, and mechanical checking. People remain to define objectives, make tradeoffs, bear responsibility, and design an environment in which AI can work dependably.

A role is a name for many tasks temporarily bundled together. When those tasks can be reassigned, the boundaries of the role naturally loosen.

CSDN’s Jiang Tao captured this well in his writing on silicon time:

> The fundamental unit of an organization is no longer the role. It is the task.

That sentence explains what happened to us. We did not suddenly acquire the complete expertise of ten professions. We broke work that once had to wait for ten different roles into units of capability that people, AI, and outside experts could share.

What was compressed was not the value of professional expertise.

It was the time spent waiting for a whole role to arrive before one professional task could be performed.

## Stage three: AI runs the workflow

After becoming super individuals, we entered a period of near-omnipotent excitement. One person could research, design, develop, deploy, test, and repair. Work that had once needed several departments appeared possible at a single desk.

Then a new bottleneck emerged.

As AI generated more code, reports, proposals, and recommendations, the volume that a person had to read and judge grew sharply too. If a person must discover and launch each task, supply its context, wait, check the result, and schedule the next step, that person’s attention will eventually be exhausted.

A super individual can still be the company’s single point of failure.

That revealed a third stage: instead of a person invoking AI task by task, AI runs a complete workflow inside explicit boundaries. The person defines intent, sets acceptance criteria, watches for anomalies, and approves or stops the process at critical points.

For example, a new feature need not wait for a person to push each step in sequence:

> Feature idea → testable specification → prototype → test run → failure evidence → result submitted for human judgment

In a mature system, agents can drive most steps in this chain. People do not leave responsibility, but they can leave the mechanical handoffs. This is the beginning of the move from `Human in the Loop` to `Human on the Loop`.

We had not reached that stage yet. The Android app built in a hotel room and my cofounder’s three-week sprint were closer to personal execution amplified dramatically by AI. They showed us stage three, but their bugs and disorder also warned us: without specifications, tests, permissions, and feedback, AI merely creates a new kind of technical debt faster.

A discussion of Harness Engineering put the problem clearly: when agents make slow progress early on, the model is often not the problem. The environment is underspecified. The real work is giving an agent tools, architectural context, and executable feedback.

The three stages are therefore not product versions that can be skipped:

1. **Task acceleration:** AI helps a role perform an existing task faster.
2. **Capability expansion:** a person uses AI to cross role boundaries and combine several traditional functions.
3. **Workflow redesign:** AI drives a sequence of tasks inside boundaries while people supervise the system and critical outcomes.

Thirty percent describes the first stage.

It cannot describe the new capability in stage two—“a person can now complete something they previously could not do at all”—much less the structural change in stage three, where work no longer waits for a person to push every step.

## From “I can do anything” to “how can the company run?”

After returning home, we could not return to our old idea.

I once thought AI would give a ten-person company the efficiency of thirteen people. Now two leaders who had not developed applications on the front line for years were experiencing something else: one person could cross several traditional functions, and a company could grow the ability to complete tasks before every key role had been hired.

Without AI, it is difficult for me to imagine how Ingora could have established the company, handled financing discussions, prepared accounts and cloud resources, found supply chains, tracked regulation, researched products, and tested software in such a short time.

But what changed us was not the number of hours saved.

It was that we stopped automatically interpreting “we do not have this role” as “this work cannot start.”

We began by asking: which capabilities does this task require? Which judgments must a person make? Which execution can AI perform? When must a real expert join to carry the missing professional responsibility?

That raised a larger question:

If individuals can become super individuals with AI, why should a company’s workflows still be designed around the roles, departments, and handoffs that existed before AI?

We had seen how one person could cross role boundaries.

What needed to change next was how people, people and agents, and agents with other agents form a company.

That leads to a different organizational metaphor: not a dinosaur whose commands travel from a brain through long nerves to its limbs, but an octopus whose arms can each sense and act while sharing one direction.

---

Previous: [001 Why Installing Copilot Still Doesn’t Make a Company AI-Native](001-why-copilot-is-not-ai-native.md)

Next: [003 Why Can’t Traditional Hierarchies Keep Up with AI Execution Speed?](003-why-traditional-hierarchy-cannot-keep-up.md)

[Star the repository](https://github.com/jackyhsu/ai-native-organization) to follow the next experiment.
