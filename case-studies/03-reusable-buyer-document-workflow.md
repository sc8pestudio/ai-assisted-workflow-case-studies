# Case Study 3: Designing and Qualifying a Reusable Buyer-Document Workflow

## Overview

Creating a new digital mockup product also meant creating buyer-facing documentation, including instructions and licence information.

Doing this manually for every product created a risk of carrying old product details into a new document, such as the wrong product name, aspect ratio, dimensions or layer information.

I wanted a repeatable system where approved document layouts could remain stable while the details for each product were supplied separately.

My role was to define what information needed to remain fixed, what should change per product, what errors needed to be detected and what evidence was required before generated documents could be approved.

## The problem

The documents needed to remain visually consistent across products while still containing accurate product-specific information.

The main risks included:

- stale product names from an earlier mockup;
- incorrect aspect ratios;
- incorrect dimensions;
- outdated Photoshop layer names;
- duplicated wording;
- missing or incorrect preview images;
- layout changes causing clipping or poor spacing;
- manually correcting generated PDFs instead of fixing the underlying reusable system.

The aim was therefore not simply to automate PDF creation.

The system needed to make repeated document production safer.

## Designing the reusable workflow

I used ChatGPT and Codex to help turn the existing approved buyer documents into a reusable workflow.

The system separated:

- stable Buyer Instructions and Licence layouts;
- shared formatting and resources;
- a small structured configuration for each product;
- an external preview image;
- automated quality checks.

For a new product, the variable information could be supplied through configuration rather than manually editing the document layout.

Examples of product-specific inputs included:

- buyer-facing product name;
- ratio and dimensions;
- relevant layer information;
- preview image;
- preview caption where needed.

This reduced the number of places where product details had to be manually changed.

## Automated quality checks

The generator was designed to check its own output for common errors.

Checks included:

- stale product names;
- incorrect ratios;
- incorrect dimensions;
- incorrect layer names;
- legacy wording;
- page count;
- whether the generated documents opened correctly;
- detectable clipping and layout problems;
- rendered comparison images;
- output inventory and file integrity.

The generated documents were kept in a non-production area until they had passed both technical and visual review.

## Testing against an approved reference

The first qualification test used an already approved mockup document set as the reference.

The generated Buyer Instructions and Licence documents matched the approved reference in wording and rendered appearance.

A rendered comparison of all four pages showed zero differing pixels at the tested resolution.

Automated stale-data and safety checks also passed.

The approved source/reference documents remained unchanged during testing.

## Technical PASS was not final approval

A successful automated comparison was not treated as sufficient on its own.

The four generated pages were also visually reviewed.

The review checked for:

- clipping;
- spacing problems;
- hierarchy changes;
- awkward layout;
- buyer-facing visual differences.

Only after both the automated checks and the visual review passed was the reusable generator considered qualified for the tested document set.

## Finding a reuse problem later

When the generator was used for another product ratio, it exposed an important reuse problem.

One Buyer Instructions page repeated part of the product description, effectively adding the ratio twice.

Instead of manually editing the finished PDF and treating the problem as solved, the issue was traced back to the reusable content rule.

A controlled correction was made for the test output, while the reusable master was flagged for review before generating the next product ratio.

The workflow reinforced a standing rule:

- check product name;
- ratio;
- dimensions;
- layer names;
- and stale content

before treating a newly generated document as complete.

## Why this mattered

The useful result was not simply faster document creation.

The workflow reduced the risk of human copy-and-paste errors while preserving a consistent buyer experience.

It also separated three different responsibilities:

1. reusable layout;
2. product-specific data;
3. quality assurance.

That meant a new product could be configured without redesigning the documents each time.

## What this demonstrated

This project demonstrated:

- turning repeated manual work into a structured process;
- separating stable templates from variable product data;
- identifying where copy-and-paste errors could occur;
- defining automated QA checks;
- testing generated outputs against an approved reference;
- combining automated checks with human visual review;
- tracing errors back to reusable rules rather than simply patching finished outputs;
- protecting approved source documents during experimentation;
- documenting what had actually passed before allowing reuse.

## Role transparency

I did not independently program the document generator.

I used ChatGPT and Codex for workflow design support, technical implementation and automated testing.

My role was to define the document requirements, identify product-specific data, decide which errors the system needed to detect, review generated outputs and determine whether the result was accurate and suitable for buyer use.

## Technical context

- reusable Buyer Instructions and Licence templates;
- structured per-product configuration;
- external preview assets;
- automated stale-data and layout QA;
- rendered reference comparison;
- human visual approval;
- non-production testing before release.