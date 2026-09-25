# Case Study 2: Qualifying a More Reliable Photoshop Automation Workflow

## Overview

My Photoshop mockup workflow had reached a point where repeated manual script handling was creating unnecessary friction.

AI-assisted tools could prepare technical work, but I was still sometimes acting as part of the execution chain by manually moving or launching scripts in Photoshop.

I wanted a more repeatable workflow that could carry out controlled Photoshop operations while reducing unnecessary manual intervention.

My role was to define the required behaviour, direct the investigation, review failures and verify whether the proposed workflow actually worked in the real application.

## The problem

The automation route needed to perform important Photoshop tasks reliably, including:

- opening the correct PSD;
- checking the expected document structure;
- locating an embedded Smart Object;
- opening and editing that Smart Object;
- saving the change back into the parent document;
- preserving protected areas of the mockup;
- saving the parent document as a new PSD;
- exporting a full-resolution image;
- reopening the saved file to confirm that changes persisted;
- completing the workflow without relying on me as the manual script-transfer step.

Some earlier execution routes had produced inconsistent behaviour, so simply generating a script was not enough.

The workflow itself needed to be qualified.

## AI-assisted investigation

I used ChatGPT and Codex to help investigate different Photoshop automation routes and structure controlled tests.

The aim was not to discard an existing working method simply because a newer method existed.

Instead, I wanted to establish:

1. which route could reliably perform the required operations;
2. what evidence was needed before calling it successful;
3. which existing method should remain available as a fallback.

Testing was carried out on non-production files so approved product files remained protected.

## Testing the workflow

A representative mockup was used to test the process from beginning to end.

The qualification test checked whether the workflow could:

1. open the specified PSD;
2. confirm the expected document structure;
3. identify and open the embedded artwork Smart Object;
4. edit and save the artwork;
5. confirm that the change propagated back to the parent PSD;
6. verify that protected areas had not changed unexpectedly;
7. save the parent document to a new file;
8. export a full-resolution PNG;
9. reopen the saved PSD and confirm persistence;
10. complete the process without requiring me to manually transport each script.

The representative test passed these operations in Adobe Photoshop 27.10.

## Handling an uncertain failure

An earlier test had produced a shutdown failure.

Rather than automatically declaring the new automation route unreliable, further testing attempted to reproduce the problem.

The failure did not reproduce consistently.

I therefore treated it as an unresolved intermittent event rather than promoting a one-off result into a confirmed defect.

This distinction mattered because the purpose of the testing was not to force either a PASS or FAIL.

It was to establish what the evidence actually supported.

## Qualified workflow

The testing established a modern Photoshop scripting route as the primary method for this workflow.

The older working route was retained as a fallback instead of being removed merely because a newer method had passed testing.

The resulting approach was:

- PSJS / UXP-based Photoshop automation as the primary route;
- COM + JSX retained as a fallback;
- real Photoshop verification required before automation is considered qualified;
- tests performed away from approved production files;
- existing working methods preserved until their replacement is genuinely proven.

## Trialling another AI operator

I have also been testing a Windows-connected Grok bot as a bounded secondary AI operator.

This is deliberately treated as an experiment rather than part of the qualified Photoshop automation system.

In one trial, Grok prepared a Photoshop script package for a mockup task.

I then manually ran the supplied script in Photoshop and reviewed the resulting image rather than assuming the generated script had succeeded simply because it completed without an error.

That route produced a usable visual result.

## Knowing when a tool failure is not a product failure

I also tested whether Grok could operate Photopea through a remote browser.

Those trials exposed several environment and tooling limitations.

For example:

- an embedded Photopea route failed before the PSD workflow started;
- a direct browser route reached Photopea but could not reliably pass the PSD through the browser file picker;
- another transport experiment failed before the PSD could be loaded.

In each case, the PSD itself had not been meaningfully tested.

I therefore did not classify those results as failures of the PSD or Photopea.

They were recorded as failures of the current operator or transport environment.

The unsuccessful route was then stopped rather than repeatedly retried without new evidence.

## What this demonstrated

This project demonstrated:

- breaking a manual workflow into individual testable operations;
- defining success criteria before changing a system;
- using AI-assisted tools to investigate technical alternatives;
- testing on protected non-production files;
- distinguishing repeatable failures from isolated incidents;
- distinguishing tool/environment failures from product failures;
- checking persistence rather than only the immediate output;
- retaining a fallback instead of replacing working systems unnecessarily;
- comparing different AI tools according to what they can actually do;
- stopping unsuccessful routes when the evidence does not justify continuing;
- documenting what has and has not genuinely been verified.

## Role transparency

I did not independently engineer or hand-code the Photoshop automation system.

I used ChatGPT, Codex and, experimentally, Grok Bot for technical investigation, scripting assistance and controlled workflow tests.

My role was to identify the workflow problem, define the required behaviour, decide what needed verification, review the evidence, reject unsupported conclusions and determine whether the resulting process genuinely worked.

## Technical context

- Adobe Photoshop 27.10
- PSJS / UXP primary automation route
- COM + JSX fallback
- Embedded Photoshop Smart Objects
- ChatGPT and Codex
- Windows-connected Grok Bot trials
- Non-production testing and manual visual QA
