# Case Study 4: Designing and Evaluating an AI-Assisted Research Workflow with Hermes Agent

## Overview

I used the existing NousResearch Hermes Agent environment to explore a more disciplined way of carrying out AI-assisted commercial research.

My aim was to keep evidence, interpretation, uncertainty and human approval visible rather than treating a polished AI answer as automatically reliable.

I did not create, name or independently program Hermes Agent.

My role was to define the questions the workflow needed to answer, set requirements for evidence and review, work with AI-assisted implementation and testing tools, examine the results, identify failures and decide whether a proposed next step had enough support.

## The problem

A polished AI research answer can easily blur several different things together:

- measured figures;
- visible observations;
- inference;
- historical interpretation;
- missing information;
- recommendations.

This matters when researching product opportunities, marketplace activity, search visibility, positioning or pricing.

Search appearances do not prove sales.

A competitor's visible price does not establish profitability.

Several AI workers agreeing does not create independent evidence if they rely on the same sources or similar models.

I wanted a workflow that kept those distinctions visible before any commercial conclusion reached me.

## A staged research and review process

The Hermes work defined separate bounded roles or stages for:

1. Scout;
2. Evidence Clerk;
3. Commercial Reviewer;
4. Adversarial Reviewer;
5. Quality Control.

Project records report one bounded child research job progressing through those five stages before returning a RESEARCH MORE result for human review.

That provided evidence of a tested sequence, but it did not mean that every possible route had become a fully qualified autonomous system.

The separation itself was important.

Gathering information, classifying evidence, interpreting it commercially, challenging the interpretation and checking the result are different tasks.

No stage gained commercial authority merely by completing its part.

## Evidence rules

The workflow distinguished four main evidence classes:

- MEASURED DATA;
- OBSERVED EVIDENCE;
- INFERENCE;
- HISTORICAL INTERPRETATION.

Missing information could remain explicitly marked as UNKNOWN, NOT RECORDED or UNRESOLVED rather than being silently filled in.

Source, date and context mattered alongside the claim itself.

The workflow was designed to prevent a search result from quietly becoming a measured market figure, or an observation from becoming a sales conclusion simply because another AI worker repeated it.

Contradictions and absent evidence were intended to remain visible.

## Controlled model evaluation

OpenRouter was genuinely used for model access during Hermes testing.

A bounded workflow record assigned DeepSeek to the Scout role and GLM to later review stages.

Other models were also compared through controlled test packets.

These tests were useful for examining how different models handled:

- weak evidence;
- conflicting evidence;
- incomplete information;
- the need to return RESEARCH MORE rather than force a conclusion;
- structured output requirements.

A plausible answer was not enough to qualify a model for every role.

The comparisons did not establish one universally best model or a completed automatic provider-routing system.

## Using supporting AI tools

Different tools had different roles in the wider project.

ChatGPT supported planning, reasoning, workflow design, structured briefs and review.

Codex supported bounded technical investigation, implementation work, checks and testing.

Cursor was used for controlled implementation work and model benchmarking.

Claude had been used in earlier Hermes-related setup work, but was not part of the later tested research chain.

I also inspected Grok Marketplace bots and experimented with their research methods. This was limited comparison work rather than an integration of Grok into Hermes.

I treated outputs from these tools as work to review, not as interchangeable authorities.

## Challenging conclusions

An adversarial-review stage was intended to look for unsupported conclusions and evidence that could weaken the current interpretation.

This exposed an important limitation of multi-agent workflows.

Several AI workers can repeat the same unsupported assumption if they depend on the same source material or similar models.

Agreement therefore did not automatically count as independent corroboration.

Human scrutiny and source provenance remained important.

## Allowing the answer to be "RESEARCH MORE"

The documented Hermes recommendation vocabulary included:

- MAKE;
- TEST;
- WATCH;
- RESEARCH MORE;
- IGNORE;
- REPOSITION;
- REFRESH;
- STOP / RETIRE.

Having these states available did not mean every state had been exercised in a live commercial decision.

RESEARCH MORE was important because the workflow did not have to force every question into a positive or negative recommendation.

If the evidence was not strong enough, uncertainty could remain explicit.

## Bottleneck Belief refinement

I later worked on a Bottleneck Belief method for RESEARCH MORE cases.

The idea was to identify the unresolved belief most capable of changing the current decision and then define one small, relevant evidence-gathering step.

A manual trial revealed another failure mode: research could begin generating more and more follow-up questions instead of reaching a useful stopping point.

That led to a single-hop stop rule.

A minimum prompt-level refinement was implemented, and a controlled Commercial Reviewer test produced one decision-changing belief and one bounded next research step while keeping execution authority at NONE.

The broader reusable child workflow had not yet completed full generic end-to-end qualification.

## Failure analysis

Not every Hermes test passed.

Later workflow attempts stopped at validation failures.

Those failures were useful.

Rather than treating a failed validation as proof that the whole system worked or did not work, the failure was preserved, inspected and addressed in bounded steps.

This helped distinguish:

- model-output problems;
- validator problems;
- workflow problems;
- missing evidence;
- unsupported conclusions.

It also reinforced the principle that a technical PASS and a commercially trustworthy result are not the same thing.

## Marketplace and SEO boundaries

Hermes was used for bounded marketplace research, while SEO, AEO and AI-search methods were also investigated.

I explored signals including:

- marketplace activity;
- competitor observations;
- keyword and search information;
- pricing;
- product positioning;
- search visibility;
- wider web research.

I did not treat these signals as proof of future sales.

A later review of retained research evidence reinforced this boundary: some visible observations remained supported, while stronger causal commercial conclusions did not.

This was not a finished SEO engine, automated competitor-monitoring product or sales-prediction system.

## Avoiding unnecessary architecture

The project also taught me that adding more AI infrastructure does not automatically improve a workflow.

I investigated questions around routing, retrieval and additional components.

A later comparison found no demonstrated benefit strong enough to justify adding another router on top of the existing Hermes and OpenRouter arrangement.

That was a useful result in itself.

The aim became to add technical complexity only when it solved a demonstrated problem.

## Human authority remained the boundary

AI workers could:

- research;
- organise evidence;
- analyse;
- challenge conclusions;
- perform quality checks;
- suggest further research.

They did not independently receive authority to:

- publish products;
- spend money;
- change protected systems;
- make final commercial decisions.

Human approval remained the controlling boundary.

## What this demonstrated

This project gave me practical experience in:

- working with an existing AI agent environment;
- defining bounded AI-worker responsibilities;
- designing staged research and review workflows;
- separating evidence from interpretation;
- defining evidence classes and missing-data rules;
- evaluating different models with controlled tests;
- using OpenRouter for model access;
- analysing model and validator failures;
- preserving source provenance;
- using adversarial review;
- recognising false agreement between AI workers;
- designing a RESEARCH MORE path;
- refining follow-up research around a Bottleneck Belief;
- recognising when further automation was not justified;
- keeping human approval as the final decision boundary.

## Project status and limitations

This was a developing and partially implemented research workflow rather than a finished commercial platform.

There was real implementation and testing, including controlled model evaluation, bounded workflow execution and prompt-level Bottleneck Belief work.

Other ideas involving further automation, routing, retrieval and SEO remained experimental, proposed or deliberately parked.

The full generic child workflow had not yet completed a fresh end-to-end qualification in the records reviewed.

I do not present this project as a finished SEO engine or autonomous commercial decision-making system.

Its value was the practical process of designing, testing and refining a more disciplined way to use AI for evidence-based research.

## Role transparency

I did not create or independently program Hermes Agent.

I used Hermes Agent, OpenRouter and supporting AI tools including ChatGPT, Codex and Cursor during the project.

Claude was used in earlier related setup work, while Grok was used for limited research-method comparison and experimentation.

My role was to identify the problem, define the research and evidence rules, specify worker responsibilities and acceptance boundaries, direct AI-assisted technical work, review outputs and failures, and decide what should be retained, changed, researched further or stopped.

## Technical context

- NousResearch Hermes Agent;
- bounded Scout, Evidence Clerk, Commercial Reviewer, Adversarial Reviewer and QC stages;
- OpenRouter;
- DeepSeek and GLM role experiments;
- controlled model benchmarking;
- ChatGPT;
- Codex;
- Cursor;
- limited Claude and Grok use;
- structured evidence classification;
- provenance and missing-data handling;
- fail-closed validation;
- RESEARCH MORE;
- Bottleneck Belief refinement;
- marketplace, SEO and AI-search research;
- human approval gates.
