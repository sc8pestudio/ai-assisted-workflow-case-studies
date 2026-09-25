# Case Study 1: Photoshop Frame Geometry and Visual QA

## Overview

I was developing a digital wall-art mockup and noticed that the frame, mount and artwork opening did not look consistently proportioned.

Rather than continue adjusting it by eye, I used AI-assisted tools to help analyse the geometry, define measurable requirements and test revised versions.

My role was to define what the finished result needed to achieve, review the outputs, identify failures and verify the final behaviour in Photoshop.

## The problem

The mockup needed:

- an exact 4:5 artwork opening;
- equal mount widths on all four sides;
- centred frame, mount and artwork geometry;
- no visible seams or halos;
- a buyer-editable Photoshop Smart Object;
- successful artwork replacement in the final PSD.

Initial analysis showed that the existing frame geometry could not satisfy all of those requirements at the same time without changing the frame proportions.

## AI-assisted investigation

I used ChatGPT to help turn the visual problem into a structured technical brief for Codex.

Codex then assisted with:

- measuring the existing frame geometry;
- checking aspect ratios;
- calculating revised dimensions;
- generating controlled test versions;
- reporting technical pass/fail conditions.

I did not treat the AI-generated result as automatically correct.

## A technically correct result that still failed

One version achieved the required numerical geometry:

- exact 4:5 artwork opening;
- equal mount widths;
- aligned centres.

However, visual review showed a visible seam where the reconstructed frame area met the wall.

Although the geometry passed, I rejected the version because the final image did not meet the visual-quality requirement.

This separated two different problems:

1. geometry;
2. compositing and realism.

## Iterative QA

The workflow became:

1. define measurable requirements;
2. generate a non-production test;
3. check numerical geometry;
4. inspect the rendered result visually;
5. reject any version that failed either test;
6. isolate the specific failure;
7. refine the next brief.

Later testing also showed that a reported Smart Object needed to be verified in actual Photoshop rather than accepted from an automated report alone.

## Verified experimental result

The successful Photoshop-native test was checked manually in Adobe Photoshop.

I verified that:

- the PSD opened correctly;
- the artwork layer was a genuine embedded Smart Object;
- double-clicking opened the editable artwork document;
- replacement artwork could be inserted and saved;
- the parent mockup updated correctly;
- the file could be closed and reopened successfully;
- multiple different artworks could be substituted;
- the artwork opening remained transparent beneath the editable artwork layer.

## What this demonstrated

This project was less about writing code and more about structured evaluation.

The key skills were:

- visual quality control;
- defining acceptance criteria;
- breaking a problem into separate testable parts;
- using AI tools to investigate technical problems;
- identifying false or incomplete passes;
- testing in the real target application;
- documenting what passed, failed and why.

## Role transparency

I did not independently program the technical solution.

I used ChatGPT and Codex as AI-assisted tools for investigation, structured briefs and technical implementation support.

My role was to identify the problem, define the required outcome, review the generated work, reject failures and verify that the final result genuinely worked.
