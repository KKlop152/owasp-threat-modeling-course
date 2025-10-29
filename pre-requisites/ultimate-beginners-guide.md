# ****Ultimate Beginner's Guide to Threat Modeling**** #

https://shostack.org/resources/threat-modeling

Threat modeling is the measure twice, cut once of cybersecurity. Structured techniques help you understand the danger so you can create a focused defensive security strategy.

Threat modeling isn’t a new idea. However, when Adam published [his threat modeling book in 2014](https://shostack.org/books/threat-modeling-book), the term wasn’t used as regularly as it is today. Digital transformation, complex, interconnected environments, and the evolving threat landscape have changed this, especially when looking at the increased number of security incidents. From the Food & Drug Administration (FDA) to the National Institute of Standards and Technology (NIST) to the Center for Internet Security (CIS), organizations that set out security standards increasingly focus on the importance of threat modeling. And in 2022, customers are expecting and demanding that your products be secure. It’s now a crucial part of engineering.

If you’re new to threat modeling, you probably want to understand the basics. The good news is that anyone can learn threat modeling. The better news is that as you practice, you can find and catch issues before they turn into real problems.

To understand this practical discipline, there is no try. Eventually, it might help for you to know the definitions, theories, philosophies, effective approaches, and well-tested techniques so that you can build your brain’s muscle memory. You might learn to avoid traps. But for now, a little simple exploration will pay off.

Sections in this Article

1. Introduction
2. What is Threat Modeling?
3. What is the difference between Threat Modeling and Risk Management?
4. Why is Threat Modeling important?
5. What are the 4 Steps of Threat Modeling?
6. Why are there so many threat modeling methodologies?
7. What are the most common threat modeling techniques and methodologies?
8. Who can use threat modeling?
9. Shostack + Associates: Learn Threat Modeling from the Expert

## What is Threat Modeling?

Threat modeling is a family of structured, repeatable processes that allows you to make rational decisions to secure applications, software, and systems.

When you use the threat modeling process, you create consistent, repeatable steps for thinking through what can go wrong with — the cybersecurity impact arising from malicious actors successfully attacking — a software, application, or system that you're building, designing, or deploying.

A threat is a suggestion that something unpleasant or violent will happen, and in technology, it’s an action that can cause harm. For example, “Her parents carried out their threat to take away her cell phone if her grades didn't improve,” or “Anyone can connect to the API and run commands without authentication.” Different sub-communities in security also use threat to mean a threat actor.

### How do I get started Threat Modeling?

Most modern threat modeling approaches follow Shostack’s Four Question Framework:

- What are we working on?
- What can go wrong?
- What are we going to do about it?
- Did we do a good job?

Getting started can be as simple as asking those four questions. As you do, specific techniques can help you answer each question. For example, we often see data flow diagrams used to address “what are we working on?” (Data flow diagrams, or DFDs, are so associated with threat modeling that they’re sometimes called threat model diagrams. Sometimes the diagram is even confused for the whole threat model.)

Sometimes, threat modeling can be as simple as asking the Four Questions, and that’s way better than no threat modeling at all. If you want to get started quickly, then you can read our free whitepaper, [Fast, Cheap and Good](https://shostack.org/files/papers/Fast-Cheap-and-Good.pdf) to contextualize and start building your own process.

## What is the difference between Threat Modeling and Risk Management?

Before going deeper into what threat modeling _is_, you need to understand what it _isn’t_. Although you threat model as a complement to your risk management program, the two serve different functions.

- **Threat modeling**: identification of attack types that malicious actors can use to compromise software, applications, and systems. Often done by engineers and/or security staff.
- **Risk management**: decisions about the trade-offs and ways to deal with the identified problems and threats. Often done by risk management staff or lawyers.

Basically, you need to engage in threat modeling to understand what can go wrong so that you can make informed decisions about how to treat the problems.

Typically, once you identify a threat, you’ll determine whether to:

- **Avoid the risk**: If the risk is greater than the potential reward, you can decide not to implement the software, application, or feature.
- **Address the risk**: After identifying the threat, you change the design or operational processes to reduce the risk.
- **Accept the risk**: If the threat is real but has a low probability or impact, you can decide to accept the costs of something going wrong.
- **Transfer the risk**: If the threat is something that someone else is better equipped to handle, you can make them responsible for it, like providing end-users or customers a terms of service and licensing agreement or purchasing insurance.
- **Ignore the risk**: If you want to pretend the threat doesn’t exist, then you can ignore it, but this decision often means you open yourself up to legal liability or compliance violations. (This is included with tongue in cheek.)

## Why is Threat Modeling important?

Threat modeling is important in two sets of ways. The first set is about delivering great products to your customers. And again, in the 2020s, that includes security. The second set is handling emergent regulations.

Since threat modeling focuses on “what can go wrong,” it allows you to take actions that protect your software, applications, and systems.

### Proactively Address Security Bugs

Threat modeling can help you find design and [security](https://shostack.org/blog/the-security-principles-of-saltzer-and-schroeder) issues. When you do this before you even write a line of code, you can fix the problem proactively, saving time and money.

### Understand Security Requirements

When you model threats and decide what to do with them, you clarify your security and technical requirements. Clear requirements allow you to create a consistent set of security features and properties.

### Engineer and Deliver Better Products

With well-defined requirements and early design review, you reduce the amount of re-designing, re-factoring, and security bug fixing. You deliver a better and more secure product faster and cheaper.

### Frame Risk

Before you even get to the risk management process, you need to frame risk based on assumptions about your environment. With threat modeling you:

- Make assumptions about threat sources
- Identify threat scenarios or threat events
- Apply the scenarios or events to your environment looking for how they can impact your assets

### Simulate Attacks

To make sure that your security team can protect against attacks, you need to train them. Whether you’re using tabletop exercises, red team exercises, or some combination, you use cyber threat modeling to help create the scenarios by:

- Identifying threat actor profiles/characteristics
- Simulating attack scenarios that these actors can use in your environment
- Seeing how well your defenses hold up

### Choose Security Tools

Threat modeling helps you determine whether you need additional security measures or tools. You can characterize threats based on the type of asset they impact, like ones that help with threats to:

- Devices
- Applications
- Networks
- Data
- People

### Can Threat Modeling Help Me Address New Regulations?

Yes. New regulations are increasingly focused on cyber threats to software development and software supply chains. NIST’s new Secure Software Development Framework (SP 800-218) has a focus on threat modeling, and OMB memo [M-22-18](https://www.whitehouse.gov/wp-content/uploads/2022/09/M-22-18.pdf) requires those to sell to the government to provide “a statement attesting that the software producer follows secure development practices.”

On September 14, 2022, Section IIIA of that memo started a set of clocks that require compliance with those attestations effectively within 120 days (roughly, January, 2023) which means that if you sell to the US government, or sell to those who sell to the US Government, you need to get started.

## What are the 4 Steps of Threat Modeling?

Although different threat modeling techniques exist, they all boil down to the same basic [Four Question Framework](https://shostack.org/training). Each question prompts different activities or steps in the threat modeling process.

### What are we working on?

The first step is defining what you’re working on. For example, you might choose to model:

- What you’re working on this sprint or improvement
- Software or applications
- Enterprise architecture
- Operational technology
- Mobile apps
- [Internet of Things (IoT)](https://shostack.org/blog/iot-security-threat-modeling/)

When you decide [_what_ you’re working on](https://shostack.org/blog/sketching-video/), you also start to build models. Diagrams are models of what you’re working on. A lot of people confuse form and function here. What's important is creating [data- and process-flow diagrams](https://shostack.org/blog/data-flow-diagrams-3-0/) that help you share what’s in your head with the people around you.

### What can go wrong?

Once you know what you’re working on, you can start thinking about all the different [things that can go wrong](https://shostack.org/blog/what-can-go-wrong-authentic-thoughts/). If you’re a glass-half-empty person, this is where you’ll shine. The glass-half full folks will creatively brainstorm.

Some considerations include:

- Who’s the intended user?
- What’s the intended use?
- Can an unintended user get access to it?
- Can someone use it in an unintended way?

### What are we going to do?

The question “what can go wrong” helps you figure out the threats. When you look at what you’re going to do, you address each threat.

Some types of actions include:

- **Mitigating threats**: Make it harder for someone to take advantage of a threat.
- **Eliminating threats**: Remove the feature or interface that creates the threat.
- **Transferring threats**: Have someone else be responsible, like having a customer change default settings.
- **Accepting threats**: Recognize that the time and effort to mitigate or eliminate the threat undermines the purpose of the project.

While these _sound_ like, and are aligned to, risk management strategies, they are subtly different. Remember: threats are the things that _can_ go wrong. Risk management focuses on the likelihood and impact of threats. You can use implicit agreement when choosing because it can be faster and easier than formal risk management approaches.

### Did we do a good job?

Finally, you need to validate your threat model by checking your work to make sure it’s as complete as possible.

This step includes checking:

- **The model**: make sure it matches what you built, starting with the diagram.
- **Each threat**: review that you found all the possible threats and did the right thing with them.
- **Tests**: ensure you have a good test to detect the problem, one that is in line with other software tests and the risks that failures expose.

## Why are there so many threat modeling methodologies?

You could ask “why are there so many programming languages?” or “why are there so many agile methodologies like scrum or extreme programming?” We adopt how we threat model to many aspects of development: what we’re working on and how we’re working on it impact how we should threat model it. Bringing a one-size-fits-all threat modeling technique may mean it doesn’t fit how we’re doing the other work, and so we develop new methodologies that are aligned.

## What are the most common threat modeling techniques and methodologies?

Data flow diagrams, STRIDE and kill chains are the top three most common threat modeling techniques and make for great structured processes. Many threat modeling efforts start out “fast and cheap,” and there’s wisdom in starting there.

Threat modeling is a process, but like everything else, you can accomplish your goal in different ways. As you become more practiced, you may adjust the techniques that you use. Over time, you may need to customize your approach for your specific needs, but you should gain proficiency first so that you stay consistent.

Although many threat modeling methodologies exist, some are outdated and deprecated because people don’t use them anymore. In other cases, people strongly associate certain models with specific technology vendors which can be limiting if you don’t want to — or can’t afford to — purchase the specific tool.

As more privacy laws and security regulations go into effect, you should consider both security _and_ privacy threats during your modeling. Combining them saves you time, improving the return on your investment.

### Kill Chains (Recommended)

Kill chains are a great way to answer “what can go wrong?” While kill chains have gained a reputation centered on incident response, looking to understand how an attacker could engage in kill chain steps (listed below) with a system model can be very powerful. Those steps include:

- Deliver an exploit
- Exploit a target
- Persist or install
- Engage in command and control (and)
- Act on Objectives

### STRIDE (Recommended)

STRIDE is also a great way to answer “what can go wrong.” With the STRIDE technique, you look at different attack types that software tends to experience. These threats undermine the properties you want your system to have like:

- Spoofing violates Authenticity
- Tampering violates Integrity
- Repudiation violates Non-repudiation 🤷
- Information Disclosure violates Confidentiality
- Denial of Service limits Availability
- Expansion of Authority violates Authorization

STRIDE is an acronym that stands for the following types of threats

- **Spoofing**: pretending to be something or someone else
- **Tampering**: Making unauthorized changes to something
- **Repudiation**: Claiming that you didn’t do something or weren’t responsible for an event (doesn’t have to be lying!)
- **Information Disclosure**: Giving information to someone who shouldn’t see it
- **Denial of Service**: Absorbing a services necessary resources
- **Elevation of Privilege**: Allowing someone to do something that they’re not authorized to do

### Data Flow Diagrams (Recommended)

As mentioned above, data flow diagrams are highly associated with threat modeling, in part because they’re simple and in part because threats tend to follow data. They’re a great way to show “what we’re working on.”

### Message Sequence Diagrams (Recommended)

Message sequence diagrams, showing the flow of messages between systems, and are a great way to model, show, and analyze what a data flow diagram shows as a single arrow.

### Attack Trees (Deprecated)

Attack trees, sometimes called threat trees, are a threat modeling technique for organizing your thinking about what can go wrong, and a way to communicate your thought process. Sometimes combined with another methodology, attack trees visually represent how an attack would progress.

Often, you’ll have multiple attack trees for a single system because the trees start with the attack goal and then build the attack path from there. Depending on a system’s complexity, you might find potential attackers have multiple goals, requiring a new tree for each.

Since creating attack trees requires substantial security expertise, modern threat modeling experts use newer techniques that include a broader range of participants with more diverse skillsets.

### Common Vulnerability Scoring System (CVSS)

Although some people might consider the CVSS a threat model, it’s really a scoring system used that tells you a known vulnerability’s severity. While some people try to use a CVSS score as part of their threat modeling by combining it with threat intelligence to assess potential threats, others understand that threat modeling is often either more proactive or more generalized, or both. CVSS inhibits both. Aspirationally, CVSS might help you organize and prioritize answers to the question “what are we going to do about it?”

### Damage potential, Reproducibility, Exploitability, Affected users, Discoverability (DREAD) (Deprecated)

DREAD focuses on impact and risk, not identifying threats. In the past, people used DREAD to help organize and prioritize answers to the question, “what are we going to do about it?”

Today, threat modeling experts rarely use this methodology. As originally published, DREAD provoked arguments over how people should score risk and impact. Although recent variants attempted to provide scoring rubrics, the method still lacks the ability to help you define factors for impact and likelihood that relate to a formal risk management approach.

Once you identify the threat, you assess:

- **Damage potential**: What can happen if the event occurs
- **Reproducibility**: How easily someone can replicate the attack
- **Exploitability**: How easily a threat actors can launch an attack
- **Affected users**: What percentage of users would be affected by the attack
- **Discoverability**: How easily an attacker can locate a vulnerability

### CMU's Hybrid Threat Modeling Method (hTMM)

hTMM combines three different threat modeling techniques:

- STRIDE
- Security cards
- Persona non grata (PnG)

The hTMM process:

1. Identifies the system
2. Applies Security Cards based on developers’ suggestions
3. Removes unlikely or unrealistic threat actor personas
4. Summarizes the results of the analysis
5. Moves on to a formal risk assessment

These five process steps relate to the Four Question Framework by breaking out the “what can go wrong, into a filtering step and a risk assessment step. However, it lacks the retrospective “how did we do” and cross checking.

### LINDDUN

LINDDUN is a threat modeling approach that can be used to enumerate privacy answers to the “what can go wrong” question. It was explicitly modeled on STRIDE.

LINDDUN stands for the following violations of privacy properties:  
  **L**inkability  
  **I**dentifiability  
  **N**on-Repudiation  
  **D**etectability  
  **D**isclosure of Information  
  Content **U**nawareness  
  Policy and Consent **N**oncompliance

### NIST 800-154 (Draft Publication)

Never formally published, NIST released [Draft Special Publication 800-154, “Guide to Data-Centric System Threat Modeling”](https://csrc.nist.gov/CSRC/media/Publications/sp/800-154/draft/documents/sp800_154_draft.pdf) in March 2016. Acting as an educational reference rather than a technical guide, the publication outlines four primary steps:

1. Identify and characterize the system and data of interest
2. Identify and select the attack vectors to be included in the model
3. Characterize the security controls for mitigating the attack vectors
4. Analyze the threat model

### Operationally Critical Threat Asset and Vulnerability Evaluation (OCTAVE) (Deprecated)

With the OCTAVE threat modeling framework, your business or operational units work with the people responsible for information infrastructure to address information security needs.

The OCTAVE framework has three phases with multiple processes embedded within each phase:

- Phase 1: Build Enterprise-Wide Security Requirements
- Phase 2: Identify Infrastructure Vulnerabilities
- Phase 3: Determine Security Risk Management Strategy

The OCTAVE methodology was quite labor intensive, and OCTAVE-ALEGRO was released to “streamline and optimize” the process.

### Persona non Grata (PnG)

PnG helps you answer the question, “can someone use this in an unintended way?” With this approach to threat modeling, you review a human attacker’s:

- Motivation
- Skills
- Goals

### Privacy Impact Assessments (PIA)

The PIA process is similar to and different from security threat modeling. While it systematically identifies and evaluates issues, its goal is mitigation. Since PIAs are often done by lawyers, the evaluation is often less technical.

Typically, a PIA:

- Describes the project
- Describes the data flows
- Analyzes against Information Privacy Principles
- Analyzes against other dimensions of privacy
- Analyzes the privacy control environment

While these are closely related to the Four Questions for Threat Modeling, they focus on privacy principles rather than threats. This shift may lead you to analyze the control environment rather than exploring different engineering approaches that could deliver value while collecting, processing, or retaining less data.

### Privacy Considerations for Internet Protocols

The Internet Engineering Task Force (IETF) published the informational “Privacy Considerations for Internet Protocols” in 2013, outlining security-privacy threats, pure privacy threats, and potential mitigation strategies.

The threats it lists are:

- Surveillance
- Stored data compromise
- Mis-attribution or intrusion
- Correlation
- Identification
- Secondary use
- Disclosure
- Exclusion (meaning users don't know that other may be collecting data)

### Process for Attack Simulation and Threat Analysis (PASTA)

PASTA is a risk-based, attacker-centric threat modeling methodology that incorporates business context and [collaboration](https://shostack.org/blog/collaboration-video/) between business, operational, technology, and risk professionals.

PASTA’s seven stages are:

1. Define objectives
2. Define technical scope
3. Decompose the application
4. Analyze threats
5. Analyze vulnerabilities
6. Analyze attack paths
7. Analyze risk and impact

### Security Cards

Unlike process-driven methodologies, the Security Cards technique uses a deck of 42 cards to create threat scenarios based on:

- **Adversary Motivations**: [reasons threat actors would attack a system](https://shostack.org/blog/modeling-attackers-and-their-motives/)
- **Adversary Resources**: Skills, hardware, and software actors might use as part of an attack
- **Adversary methods**: How threat actors might approach an attack, including using technology and social engineering
- **Human Impact**: What happens to people as the result of an attack

### Trike (Deprecated)

Trike is a risk-based security auditing framework used to describe a system's security characteristics from high-level architecture to low-level implementation details. Although Trike intended to automate threat generation, it hasn’t been updated since 2012.

The Trike model looks like this:

- Two threat categories, denial of service and elevation of privilege, help generate a set of threats
- Organize attacks into attack trees made up of tasks and subtasks
- Look for weakness in the system that allow an attack tree to work
- Review for vulnerabilities, unmitigated paths through an attack tree
- Implement safeguards that reduce risk

### Visual, Agile, and Simple Threat (VAST) (Vendor-associated)

The VAST method relies on using an automated tool to identify threats. The mode’s three pillars are:

- Automation
- Integration
- Collaboration

To use VAST, you need specific vendor-supplied threat modeling software.

## Who can use threat modeling?

Since threat modeling drives informed risk analysis, anyone can use threat modeling. Some common participants include:

### Software Development Teams and Testers

For people focused on creating software, threat modeling helps them find and address design issues early in the development process so that they can build security directly into the Software Development Life Cycle (SDLC). By delivering and deploying more secure software, they more effectively meet customer requirements and expectations.

### Systems Architecture and Operations Teams

Threat modeling helps people who bring together software components to address threats when they:

- Design systems
- Select components
- Prepare for deployment

With threat modeling, they can find security and privacy threats so that they can make informed tradeoffs that address how to handle threats.

### Project Managers

Project managers hate the unexpected delays that come from penetration tests security reviews, and other things that happen late in a project leading to re-work. When done early, threat modeling helps identify future issues, and allows you to incorporate them into planning. It’s a little like “measure twice, cut once.” It takes a little longer per element, but the overall project gets done faster with less waste.

### Penetration Testers

Every penetration tester does some threat modeling, even if it’s very informal. They construct a mental model of “what I’m attacking,” generate and test hypotheses about “what can go wrong,” and then deliver a report with advice about what to do about those things.

### Security Teams

Threat modeling gives security experts a way to enhance their productivity and bring security into the development, operation, and release of their organization’s processes. Most software and applications are built around business or organizational realities that require tradeoffs. Security professionals can use threat modeling to build cyber resilient systems across people, processes, and technology.

### Business Managers and Executives

While executives don’t need to understand the technical parts of threat modeling, they do need to make informed decisions about risk. [When business executives use threat modeling](https://shostack.org/blog/how-executives-can-use-threat-modeling/), they know what can go wrong with their technical systems so that they can make a choice about it or how to defend them. Business perspectives on which threats matter are also tremendously valuable for prioritization of remediation work.

## Shostack + Associates: Learn Threat Modeling from the Expert

Adam Shostack is a leading expert on threat modeling who has authored and contributed to multiple [books about the topic](https://shostack.org/books). He brings his 25+ years of experience to his threat modeling courses, delivered both [online](https://courses.shostack.org/) or [in-person](https://shostack.org/coaching) for groups of 50 or more.

For more information about how Shostack & Associates can help your team level up their threat modeling skills, [contact us today](https://shostack.org/contact) or join one of our mailing lists to receive upcoming course announcements or hear about new things he’s creating.
