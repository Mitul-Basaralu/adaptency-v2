# What I Contributed

*The contributions described below reflect my best recollection of my role in the project based on project documents, code contributions, meeting participation, and repository history.*

## Developing the Main Idea

The project's initial goal was to find a way to measure aspects of LLM performance that traditional benchmarks did not capture. During early brainstorming sessions, one team member proposed the idea of studying adaptation by introducing new information during generation. I supported this direction by researching existing literature and identifying related work that could help shape the project.

My primary contribution during this phase was conducting literature reviews and bringing relevant papers to team discussions. I researched evaluation frameworks such as MMLU (*Measuring Massive Multitask Language Understanding*) and other LLM benchmarking papers to understand how model capabilities were commonly measured and where gaps existed. Rather than focusing solely on final-answer performance, we became interested in measuring how a model responds when its context changes while it is already generating text.

I also researched Process Reward Models (PRMs), reward modeling approaches, and other evaluation methodologies that might help quantify adaptation. Through multiple rounds of discussion and iteration, we evaluated different ways to define and measure adaptation before converging on the final framework used in the paper.

One specific idea I proposed was the use of cosine similarity as a potential metric for measuring how generated outputs shifted toward newly injected context. Throughout the ideation process, I attended all project meetings, contributed feedback on proposed methodologies, and helped refine the research direction through discussion of both existing literature and new evaluation approaches.

## Initial Proof of Concept

After the initial research direction was established, I contributed to several early proof-of-concept efforts aimed at determining whether adaptation could be measured in practice. One area I explored was Process Reward Models (PRMs) and step-level reasoning evaluation. To support this investigation, I worked with the PRM800K dataset and wrote preprocessing code that extracted positively rated reasoning steps and converted them into a format suitable for experimentation. This work helped the team evaluate whether reward-model-based approaches could be used to quantify adaptation and reasoning behavior.

As part of this effort, I contributed to dataset preprocessing and training-data preparation by working with JSON and JSONL-based data pipelines. This included loading raw dataset files, filtering and restructuring examples, preserving relevant problem and answer information, and converting data into formats suitable for downstream experimentation and model training workflows.

In addition to researching evaluation methodologies, I also began developing an early proof-of-concept for measuring adaptation directly. Rather than working with a large benchmark dataset, the goal of this prototype was to test whether a model could successfully adapt to new information within a single problem and whether adaptation could be observed and measured in a controlled setting. I worked on the initial implementation and experimentation for this concept before development was later handed off to another team member.

Although these early approaches were ultimately not used in the final experimental pipeline, they helped the team evaluate multiple possible directions, identify limitations of alternative methodologies, and refine the framework that was eventually adopted in the paper.

## Project Collaboration and Paper Review

Throughout the project, I attended all team meetings and remained actively involved in discussions surrounding the research direction, methodology, and evaluation framework. In addition to my contributions during the ideation and proof-of-concept phases, I assisted with reviewing and editing the paper throughout its development.

While I was not primarily responsible for writing major sections of the manuscript, I provided feedback on drafts, reviewed explanations of methodology and results, and suggested revisions intended to improve clarity, organization, and overall readability. These reviews helped ensure that technical concepts were communicated more effectively and that the paper accurately reflected the goals and findings of the project.

As the project progressed and development responsibilities became more specialized, other team members focused primarily on dataset generation, adaptation experimentation, and implementation of the final evaluation pipeline. My role shifted more toward providing feedback, reviewing progress, participating in research discussions, and helping refine the presentation of the work.

Overall, my contributions centered on literature review, research ideation, metric development, proof-of-concept exploration, dataset preprocessing, project collaboration, and paper review.
