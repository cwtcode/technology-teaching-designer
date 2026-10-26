# Technology Teaching Designer

An AI agent skill that helps primary and secondary teachers plan technology learning and create coherent teaching materials.

Start with what students should learn, plan how they will learn it, and decide what evidence will show their understanding. Then create the curriculum map, lesson plan, worksheet or presentation needed for teaching.

**Every lesson includes a suitable platform and at least one achievable task that students can complete and have assessed within the lesson.**

## What it can do

| Function | What you receive |
| --- | --- |
| Propose a curriculum map | A progressive sequence with prerequisites, learning outcomes, lesson allocations, platforms, tasks and assessment evidence. |
| Create a lesson plan | A timed plan with instruction, demonstrations, guided practice, inquiry, feedback, differentiation and checks for understanding. |
| Create a worksheet | Student instructions, scaffolded tasks, writing space, checkpoints, testing records and reflection, with separate teacher answers when requested. |
| Create a PowerPoint | Lesson slides with explanations, demonstrations, practice prompts and teacher notes, aligned with the lesson plan. |
| Suggest topics and demonstrations | Suitable options with learning purposes, prerequisites, preparation, likely difficulties and extensions. |

Use the skill to teach computing and technology, or to integrate technology into other subjects. Request one resource or a complete teaching pack.

## Quick start

After installing the skill in a supported host, try:

```text
Use $technology-teaching-designer to create a 40-minute S2 lesson
on sequence, selection and repetition. Students are beginners and
share computers in pairs. Recommend a platform and include one
completed task, success criteria and an individual exit check.
```

In ChatGPT environments where the skill is installed and available, select **@Technology Teaching Designer**. In Codex CLI or the IDE extension, mention **$technology-teaching-designer**.

For better results, provide:

- Subject, topic, form/year level and prior knowledge.
- Number and duration of lessons.
- Available devices, software and internet access.
- Curriculum requirements, teaching language and learning needs.
- Required outputs and any school templates or reference materials.

The skill uses available context and states reasonable assumptions when information is missing.

## Install and use

This repository contains skill instructions and reference materials. It requires an AI assistant that supports agent skills; it is not a standalone application.

### Local Codex installation

1. Download or clone the repository.
2. Keep `SKILL.md`, `references/`, `agents/` and any supplied assets together in a folder named `technology-teaching-designer`.
3. Place that folder in one of these locations:

| Scope | Location |
| --- | --- |
| Your local user account | `~/.agents/skills/technology-teaching-designer/` |
| One project | `<project-root>/.agents/skills/technology-teaching-designer/` |

Codex detects skill changes automatically. If the skill does not appear, restart Codex. You can also ask the built-in `$skill-installer` to install it from the repository URL once published.

For current installation and distribution guidance, see [OpenAI’s skill documentation](https://learn.chatgpt.com/docs/build-skills). ChatGPT installation and availability depend on the host and distribution method; a GitHub upload alone does not install the skill in an account.

### File generation and research

The host assistant needs suitable file-generation tools to create editable DOCX worksheets and PPTX presentations. The skill directs it to use available document and presentation workflows, including visual checks. Without those tools, it can provide structured content and explain the limitation.

Web access supports current platform recommendations, curriculum verification and emerging-technology research. When unavailable, the skill should identify unverified details rather than claim they are current.

## How lessons are designed

The default sequence is:

1. **Introduction and instruction:** activate prior knowledge and establish learning goals.
2. **Worked example and demonstration:** explain decisions and invite predictions.
3. **Guided practice and application:** provide manageable steps, then reduce support.
4. **Evaluation, feedback and improvement:** test against criteria and act on feedback.
5. **Conclusion and reflection:** check individual understanding and identify next steps.

Teachers can repeat or adapt stages to suit the lesson.

### A completed task with evidence of learning

For each lesson, the skill specifies the platform, task, minimum finished output, time allowance, success criteria and evidence to collect. Longer projects have a completed, assessable milestone in each lesson.

A working product or submitted file does not, by itself, demonstrate understanding. Pair and AI-assisted tasks include individual evidence such as an explanation, prediction, adaptation or test.

### Inquiry and student agency

Choose structured, guided or open inquiry according to students’ readiness. Activities can include predict–observe–explain, debugging investigations, comparing solutions, investigating user needs and generating questions.

Students make decisions about methods, tests, evidence and revisions, with appropriate teacher guidance.

### Learning theories and anticipated difficulties

The skill connects relevant design choices with perspectives such as cognitive load theory, constructivism, social constructivism, self-regulated learning and self-determination theory. It treats Bloom’s taxonomy as a framework for cognitive demand.

It anticipates possible misconceptions and classroom barriers, pairs them with observable signs, and suggests scaffolds and teacher responses. These are hypotheses to check; theoretical alignment does not establish lesson effectiveness.

## Curriculum progression

A suggested computing pathway moves through computational thinking, block-based programming, connections between representations, text-based programming, AI-assisted development and bounded agentic workflows.

Placement depends on readiness as well as age. Pseudocode can accompany programming rather than serving as a compulsory gateway. AI literacy, information literacy, digital citizenship and responsible use can develop throughout.

Curriculum planning can draw on Hong Kong, Singapore, US and UK references while distinguishing local requirements from enrichment programmes and international guidance. UK planning identifies the relevant nation; US planning considers state or district requirements where needed.

## AI framework alignment

Lessons about AI must map objectives, activities, completed tasks and assessment evidence to selected competencies in both:

- [OECD/European Commission AI Literacy Framework (2026)](https://doi.org/10.1787/65cd27d4-en): **Engage with AI, Create with AI, Manage AI and Shape AI**, with Basic, Intermediate and Advanced learner expectations.
- [UNESCO AI Competency Framework for Students (2024)](https://unesdoc.unesco.org/ark:/48223/pf0000391105): **Human-centred mindset, Ethics of AI, AI techniques and applications, and AI system design**, with Understand, Apply and Create progression levels.

The frameworks and their levels remain distinct. Select relevant competencies for each lesson and build wider coverage across the curriculum. An AI-generated app does not automatically demonstrate AI-system-design competence.

The detailed mapping belongs in teacher notes. UNESCO’s separate teacher framework can inform teacher preparation; it does not replace student outcomes. Framework alignment is a planning requirement of this skill, not official certification or endorsement.

## Information and media literacy

Teach information and media literacy as standalone lessons or embed it within subject learning. Topics include source evaluation, fact-checking, media representation, attribution, privacy, digital wellbeing and responsible sharing. AI use is optional.

For Hong Kong planning, the skill references the **“Information Literacy for Hong Kong Students” Learning Framework (2024)** and its key-stage targets. Materials distinguish authentic sources from fictional teaching cases and allow evidence-based uncertainty.

## Default lesson plan format

Lesson plans follow a school-style layout:

- A centred class and subject title.
- A lesson information table: date, time, class, venue, teacher, chapter, topic, prior knowledge and learning objectives.
- A lesson outline with **Time | Content | Activity | Remarks**.
- Supporting teacher notes for platform setup, assessment, differentiation and rationale where needed.

The default is A4 portrait with Times New Roman body text, grey table headings and simple borders. A teacher’s current instructions or supplied template take precedence.

## More example prompts

### Curriculum map

```text
Use $technology-teaching-designer to propose an S1–S3 technology
curriculum with 20 lessons per year. Show prerequisites, platforms,
one assessed task per lesson and readiness checks. Include programming,
AI literacy, and information and media literacy.
```

### Aligned worksheet and presentation

```text
Use $technology-teaching-designer to create a student worksheet,
separate teacher answers and a PowerPoint for this lesson plan.
Keep the examples, task IDs and success criteria consistent.
Provide editable Word and PowerPoint files where supported.
```

### AI-assisted development

```text
Plan two 40-minute S2 lessons on evaluating AI-generated code.
Map the objectives to OECD/EU and UNESCO student competencies.
Include independent tests, human decisions and individual explanations.
```

### Standalone media literacy

```text
Create a 40-minute S2 lesson on deciding whether to share an online
claim. Use a prepared paper source pack, include peer feedback,
and assess an individual evidence-based decision.
```

### Improve a lesson after teaching

```text
Students followed the demonstration but struggled to adapt the code.
Review these exit responses and revise the scaffolding and task.
Separate observed evidence from possible explanations.
```

## Repository contents

Place this README alongside `SKILL.md` at the repository root. Keep the accompanying resources together when distributing the skill.

| Path | Purpose |
| --- | --- |
| `SKILL.md` | Main instructions and task routing. |
| `agents/openai.yaml` | Host-facing skill metadata. |
| `assets/` | Supplied visual assets, where included. |
| `references/curriculum-progression.md` | Curriculum maps and progression. |
| `references/lesson-design.md` | Lesson planning, platforms and assessed tasks. |
| `references/lesson-plan-format.md` | Default school lesson-plan layout. |
| `references/learning-and-inquiry.md` | Learning rationale, inquiry and agency. |
| `references/materials.md` | Worksheets, answers and presentations. |
| `references/anticipation-and-quality.md` | Anticipated difficulties and quality checks. |
| `references/information-and-media-literacy.md` | Embedded and standalone literacy teaching. |
| `references/ai-framework-alignment.md` | OECD/EU and UNESCO alignment requirements. |
| `references/worked-example.md` | An illustrative alignment example. |

## Review and contribute

Review generated materials before classroom use, including subject accuracy, curriculum fit, reading demand, timing, access and assessment. Report actual classroom evidence when requesting improvements; the skill does not guarantee learning outcomes.

Useful contributions include anonymised teaching examples, clearer scaffolds, accessible layouts, verified curriculum updates and feedback on task feasibility. For an issue or pull request, describe the teaching context, request, observed output and suggested improvement. Keep student information and private school documents out of public examples.
