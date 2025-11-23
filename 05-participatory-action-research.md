# Chapter 5: Participatory Action Research for Sustainable Agile Workflows

## Introduction

To create truly human-sustainable Agile workflows in the era of Generative AI (GenAI), we must adopt a methodology that places the people involved at the center of the change process. Participatory Action Research (PAR) is a powerful framework that aligns perfectly with this goal. PAR is a collaborative approach to research and development that seeks to bring about social change and practical improvements through the active involvement of the community being studied (Reason & Bradbury, 2008). In the context of software engineering, PAR means that developers, product owners, and other stakeholders are not just subjects of study but are active co-researchers in shaping their own workflows and tools. This chapter explores how PAR can be applied to iteratively design, implement, and refine AI-integrated Agile processes, ensuring they are effective, ethical, and truly supportive of the teams using them.

## Case Examples

### Case Example 1: Co-Designing an AI Code Review Assistant

**Scenario**: A software team was experimenting with a new GenAI tool that automatically suggested fixes for common code quality issues. However, developers found the suggestions to be generic and often lacking context, leading them to ignore the tool.

**Intervention**: The team initiated a PAR project to co-design a better AI code review assistant. They held weekly "AI Review Workshops" where developers would bring examples of the AI's unhelpful suggestions. In these workshops, they collaboratively identified the specific context the AI was missing and brainstormed how to provide it. This feedback was then used to fine-tune the AI model's prompts and rules, effectively "teaching" it the team's specific coding conventions and architectural patterns.

**Outcome**: The AI's suggestions became significantly more relevant and helpful. The PAR process not only improved the tool but also fostered a sense of ownership and empowerment among the developers. They were no longer passive recipients of AI suggestions but active participants in shaping the tool's behavior. This aligns with the principle of action research fostering collaboration between researchers and practitioners to improve software engineering practices (Sjöberg et al., 2005).

### Case Example 2: Iteratively Improving an AI-Powered Sprint Planning Tool

**Scenario**: An Agile team was using an AI tool to help with sprint planning by estimating task durations and identifying dependencies. While the tool was often accurate, it sometimes failed to account for human factors like team morale or upcoming holidays, leading to unrealistic sprint commitments.

**Intervention**: The team adopted a PAR cycle to improve the tool's utility. At the end of each sprint retrospective, they dedicated time to a "Sprint Planning AI Review." The team discussed where the AI's predictions had been accurate and where they had failed. They created a shared "human factors" log, which they used to adjust the AI's inputs for the next sprint's planning. For example, they might manually adjust the AI's capacity forecast based on known team events.

**Outcome**: The team's sprint planning became more realistic and sustainable. By treating the AI as a tool to be guided by human insight, they created a hybrid planning process that combined the AI's data-processing power with the team's contextual knowledge. This iterative refinement is a hallmark of both Agile methodologies and action research.

### Case Example 3: A PAR Approach to Ethical AI in HR Software

**Scenario**: A company was developing an AI-powered tool to help screen resumes and identify promising candidates. The development team was concerned about the potential for the AI to introduce bias into the hiring process.

**Intervention**: The team adopted a PAR approach that involved not just developers but also HR professionals, ethicists, and representatives from different employee resource groups. They conducted a series of workshops to identify potential sources of bias in their training data and in the features the AI was being asked to evaluate. This collaborative process led to the development of a "fairness checklist" that was used to audit the AI's recommendations.

**Outcome**: The PAR process uncovered several potential biases that the development team alone would have missed. For example, the AI was found to be down-ranking candidates from non-traditional educational backgrounds. By involving a diverse group of stakeholders, the team was able to build a more equitable and ethical AI tool. This demonstrates how PAR can be a powerful methodology for human-centered AI development that prioritizes fairness and ethical outcomes.

## Diagram: The Participatory Action Research Cycle in Agile
<!-- Note: This ASCII diagram will be converted to a high-quality image (e.g., PNG, SVG) for the final PDF publication. -->

```
+-------------------------------------------------+
|               1. Diagnose & Plan                |
|  (Team collaboratively identifies a problem     |
|   or opportunity in their AI-Agile workflow)    |
+--------------------------+----------------------+
                           |
                           v
+--------------------------+----------------------+
|                  2. Act & Observe                 |
|  (Implement a change or a new tool, and        |
|   observe its effects on the team's work)     |
+--------------------------+----------------------+
                           |
                           v
+--------------------------+----------------------+
|               3. Reflect & Evaluate             |
|  (In a retrospective, the team discusses      |
|   the outcomes and decides on next steps)     |
+--------------------------+----------------------+
                           |
                           ^
                           |
          +----------------+----------------+
          |         (Iterate the Cycle)          |
          +--------------------------------------+
```
**Figure 5.1**: The PAR cycle, adapted for an Agile context. This iterative process of planning, acting, and reflecting allows teams to continuously improve their AI-integrated workflows in a way that is grounded in their own experiences and needs.

## Exercises

### Exercise 1: Designing a PAR Workshop

**Task**: Imagine your team is about to adopt a new GenAI tool for generating unit tests. Design a 1-hour PAR workshop to be held after the first sprint of using the tool. Outline the agenda, key questions to ask, and the desired outcomes of the workshop.

*(A solution to this exercise can be found in the `history/solutions` directory of the book's companion repository.)*

### Exercise 2: Identifying an Opportunity for PAR in Your Workflow

**Task**: Reflect on your own (or a hypothetical) software development workflow. Identify one area where a GenAI tool is being used or could be used. Describe how you might apply the PAR cycle (Diagnose & Plan, Act & Observe, Reflect & Evaluate) to improve the integration of this tool in a human-centered way.

## Human-Sustainability Checks and Ethical Considerations

Participatory Action Research, by its nature, is a powerful tool for ensuring ethical and human-sustainable outcomes. However, the process itself requires careful consideration:

-   **Inclusivity and Power Dynamics**: Who gets to participate in the PAR process? It is crucial to ensure that all voices are heard, especially those of junior developers or team members from underrepresented groups who may feel less comfortable speaking up.
-   **Psychological Safety**: The PAR process must be conducted in an environment of high psychological safety, where team members feel safe to critique existing processes and tools without fear of blame or retribution.
-   **Transparency of Research Goals**: The goals of the PAR project should be transparent to all participants. Is the goal to improve team well-being, increase productivity, or both? A lack of clarity can lead to mistrust.
-   **Data Privacy and Anonymity**: When collecting feedback and observing workflows, it is important to protect the privacy and anonymity of the participants. Data should be aggregated and anonymized wherever possible.
-   **Long-Term Commitment**: PAR is not a one-off solution. It requires a long-term commitment from both the team and management to continuously iterate and improve. Without this commitment, the process can feel like a "flavor of the month" initiative.

## Summary

-   Participatory Action Research (PAR) is a collaborative methodology for improving workflows by actively involving the people who use them.
-   PAR aligns well with Agile principles due to its iterative and reflective nature.
-   The PAR cycle (Diagnose & Plan, Act & Observe, Reflect & Evaluate) provides a structured way to co-design and refine AI-integrated Agile processes.
-   Applying PAR can lead to the development of more effective, human-centered, and ethical AI tools and workflows.
-   Case studies demonstrate how PAR can be used to improve AI code review assistants, sprint planning tools, and ethical AI for hiring.
-   Successful implementation of PAR requires a commitment to inclusivity, psychological safety, transparency, and long-term iteration.

