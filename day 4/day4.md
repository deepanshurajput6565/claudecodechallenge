Here's a rundown of today's session:
What you built/learned:

Role-Based Prompting (Day 3 recap territory) — assigning Claude a persona changes depth and specificity of output; you turned it into a LinkedIn post with a comparison visual.
Prompt Engineering fundamentals — weak vs. engineered prompts, and the Clarity/Specificity/Goal-Driven framework, packaged into a matching post + light blue graphic.
AI Personality Profile experiment — used Claude to analyze your own working style based on how you've been prompting and building; got the "Prompt Architect" framing and a stylized (non-photorealistic) character illustration.
Elite AI Career Strategist roadmap (Day 4) — the most technical build today:

Used a structured 4-question elicitation flow (situation → skills → goal → timeline) before generating anything
Had Claude apply visible Chain-of-Thought reasoning (position → strengths → gaps → path → priorities → projects → networking → milestones)
Generated an actual one-page A4 PDF (not just an image) using HTML/CSS rendered through WeasyPrint — your first PDF deliverable in this series, versus the SVG/JPG images from earlier days



Key observations from today:

Emoji breaks PDF rendering — Noto Color Emoji causes a font-subsetting crash in WeasyPrint; the fix was swapping emoji for custom inline SVG icons, which also gave a cleaner, more "consulting report" look than emoji ever could.
Fixed pixel heights are fragile — hardcoding height: 80px on a flex box works only until content grows past it, then it silently overlaps instead of erroring. min-height or no fixed height at all is safer for text-heavy layouts.
Elicitation-before-generation produces sharper output — asking 4 targeted questions before building the roadmap meant zero generic filler in the final result.
