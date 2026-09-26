# AI-Assisted Workflow Case Studies

I am an artist and digital product creator with a practical interest in using AI and technical tools to solve real creative and business problems.

My work has gradually developed from creating and selling artwork into designing, testing and improving AI-assisted workflows for visual production, digital products, quality assurance, documentation and research.

My role in these projects is primarily workflow design, product ownership, requirements setting, visual and quality evaluation, testing, and AI-tool orchestration. I use AI tools to help with technical implementation, but I do not present AI-assisted code as independently hand-written engineering work.

## Case Studies

1. [Photoshop Frame Geometry and Visual QA](case-studies/01-photoshop-frame-geometry-and-visual-qa.md)  
   Measuring and testing frame geometry, identifying visual defects, and separating technical verification from final visual approval.

2. [Photoshop Automation Workflow](case-studies/02-photoshop-automation-workflow.md)  
   Developing and testing a bounded AI-assisted Photoshop workflow with controlled changes, verification and human review.

3. [Reusable Buyer Document Workflow](case-studies/03-reusable-buyer-document-workflow.md)  
   Creating a reusable buyer-document process with consistent content, generated outputs and quality checks.

4. [Hermes Research and Evidence Workflow](case-studies/04-hermes-research-evidence-workflow.md)  
   Using a structured AI-assisted research process with defined evidence classes, staged evaluation and human approval.

## How This Work Evolved

My workflow work grew out of a practical problem in my own art business.

I create physical artwork using oils, acrylic, watercolour, printmaking and epoxy, and I have also created digital artwork using AI image-generation tools. Whether the original work was physical or digital, it still needed to be presented convincingly for sale online.

For physical artwork, that meant photographing the finished piece and then presenting it in a suitable frame or interior setting. For digital artwork, the same presentation problem remained: each piece needed a room and frame that suited the artwork, supported it visually and helped show it at its best without becoming the focus itself.

I found that existing mockups and frame assets were not consistently available with the exact aspect ratios, artwork openings, mount proportions, frame proportions and presentation styles I needed.

That led me to begin experimenting with my own frame and mockup creation.

Early AI-assisted Python and Pillow experiments used scripts to place and draw frames, mounts, artwork, shadows, textures and reflections over room images. Some of the early frames worked structurally but looked too artificial or plastic, so visual realism became as important as getting the geometry right.

In March and April 2026, I explored this further through **Japandi Mockup Studio**, an AI-assisted browser-based mockup tool developed with AI assistance, including Cursor. It allowed me to choose rooms and artwork, work with single, double and triple frame arrangements, adjust the framed composition, preview it and export an image. A surviving 5,000 × 5,000 export confirms that at least one image export completed successfully.

But a successful export was not the same as a commercially convincing result. The frame appearance still exposed problems with artificial-looking edges, materials and finishes. That pushed the work towards correcting frame geometry and experimenting with real donor textures, including beech wood, to create more believable frame surfaces.

I also developed a series of AI-assisted room-placement tools to turn visual artwork positioning into measured coordinates. The workflow evolved from a single-room guide into reusable print-size and frame-footprint tools, then into a Universal Auto Detect version designed to recognise the source image size and generate consistent placement guidance across different square room-image sizes. Earlier saved placement records document use of the workflow, while the final Auto Detect version survives as inspected code rather than a runtime-verified finished product.

Repeated problems with alignment, artwork openings, pale edges, proportions and other visual inaccuracies then pushed the work towards increasingly measured geometry and controlled visual QA.

From there, the workflow developed into more reusable production methods involving controlled frame assets, Photoshop Smart Objects, Photoshop and Photopea testing, buyer documentation, automated checks and structured review.

The same underlying approach later expanded beyond visual production into AI-assisted research and evaluation, including the Hermes workflow documented in the fourth case study.

**art creation → online presentation → mockup problems → browser and scripting experiments → realism and donor-frame work → measured visual QA → reusable production systems → structured AI-assisted research and evaluation**

## How I Work With AI

I use AI as part of a structured working process rather than treating its outputs as automatically correct.

I usually begin by defining the problem, the practical requirements and what a successful result needs to achieve. I use ChatGPT to help me structure ideas, investigate problems, turn requirements into clearer briefs and review evidence.

For bounded technical work, I use tools such as Codex, Cursor and other AI-assisted environments to help implement, inspect or test specific tasks. I review the results myself rather than treating generated code, technical reports or automated checks as final authority.

My role is to:

- define the problem and requirements;
- decide what needs to be tested or measured;
- give AI tools bounded instructions;
- review visual and technical outputs;
- identify failures, inconsistencies and unsupported claims;
- decide whether a result is actually acceptable;
- preserve evidence of what worked and what did not.

A technical PASS does not automatically mean a visual or commercial PASS. Something can be mathematically correct, successfully exported or technically functional and still be unsuitable for the product I am trying to create.

I also distinguish between work that I have personally designed, tested and approved and technical implementation produced with AI assistance. I do not present AI-assisted code as independently hand-written engineering work.

I remain the final decision maker: AI can generate, inspect, compare and suggest, but I decide whether the result meets the actual requirement.

## Tools and Environments

I have used different tools at different stages of this work depending on the problem being solved.

### Visual and production tools

- Adobe Photoshop
- Photopea
- Affinity Photo
- Python and Pillow
- browser-based HTML/React tools developed with AI assistance

### AI-assisted working tools

- ChatGPT - problem structuring, briefs, investigation, review and evidence checking
- Codex - bounded technical implementation, inspection and testing
- Cursor - AI-assisted development and iteration
- Claude - additional AI-assisted exploration, comparison and problem-solving
- Gemini - additional AI-assisted exploration, comparison and problem-solving
- Hermes Agent - structured research and evaluation workflows
- OpenRouter - model access used within research experiments
- Grok - limited manual comparison and evaluation work

### Image-generation and visual tools explored

- Midjourney
- NightCafe - experimentation with multiple underlying image-generation models
- Adobe Firefly
- Krea
- Microsoft Designer
- Google Whisk
- Flux by Black Forest Labs
- image generation within ChatGPT

The image-generation tools each had different strengths depending on the task. In my own testing, ChatGPT image generation worked particularly well for room mockups, while Midjourney was especially strong for artwork and convincing realistic textures. Other tools were useful in different situations, so I selected them according to the result I was trying to achieve.

### Automation experiments

I also explored **n8n** for coordinating digital-product and Etsy tasks. Surviving workflows show genuine experimentation and partial configuration, but I do not describe them as a verified production system because the evidence does not establish a successful end-to-end deployment.

## Skills Demonstrated

Across these projects, I have demonstrated skills in:

- defining requirements and acceptance criteria;
- workflow design and process improvement;
- visual quality assurance and comparative review;
- structured testing, defect identification and evidence-based decision making;
- directing AI tools with clear, bounded briefs;
- technical investigation using AI-assisted tools;
- Photoshop Smart Object and digital-product production workflows;
- image geometry, aspect ratios and presentation accuracy;
- reusable buyer documentation and quality-checking systems;
- automation design and evaluation;
- research synthesis and evidence classification;
- GitHub branch, pull-request and review workflows.

The common thread is not simply using AI tools. It is defining what needs to be achieved, testing whether the result actually meets that requirement, identifying where it does not, and improving the process until the outcome is reliable and usable.

## Working Principles

A few principles guide the way I approach these projects:

- define the requirement before trying to automate or implement it;
- use measurable acceptance criteria where they are useful;
- keep technical verification separate from visual and commercial approval;
- test important outputs in the real software or environment where they will actually be used;
- make controlled changes when investigating failures so the cause can be identified;
- protect working source files and test potentially destructive changes on copies;
- document failures, limitations and uncertainties rather than hiding them;
- preserve enough evidence for important decisions to be checked later;
- do not claim more than the available evidence supports;
- turn proven processes into reusable systems rather than repeatedly solving the same problem by hand.

The aim is not automation for its own sake. It is to develop processes that are accurate, understandable, repeatable and genuinely useful.