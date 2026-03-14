# Claude Skill: Professional UI / UX Critique

## Goal

Provide a professional, human-level critique of the user interface and user experience.  
The review should reflect the perspective of a **senior product designer or UX consultant**, not an automated or generic analysis.

The objective is to identify design weaknesses, usability issues, friction points, and areas where the product could be more intuitive, efficient, and polished.

The critique should feel like feedback from a **real design review**, not AI-generated commentary.

---

# Review Standards

Approach the critique as if reviewing a product for a professional design team.

Feedback should be:

- Direct
- Professional
- Constructive
- Specific
- Actionable

Avoid generic or obvious observations.

Focus on meaningful UX and design quality improvements.

Do not include filler statements such as:
- “This looks good overall”
- “Nice design”
- “Clean UI”

Only comment where improvement or clarification is useful.

---

# Fresh Review Requirement

Always evaluate the **current UI being shown**.

Do not rely on:
- earlier critiques
- previous design summaries
- prior conclusions

Treat every review as a **new design audit**.

Base feedback only on what is currently visible.

---

# What to Evaluate

## Visual Hierarchy

Assess whether the interface clearly communicates what matters most.

Look for:

- unclear primary actions
- competing visual elements
- weak hierarchy
- inconsistent emphasis
- poor use of spacing

Identify where user attention is likely to go first and whether that is correct.

---

## Layout & Structure

Evaluate how information is organized.

Check for:

- cluttered areas
- excessive whitespace
- inconsistent alignment
- layout imbalance
- poor grouping of related elements

Determine whether the interface feels structured and intentional.

---

## Navigation & Flow

Assess whether the user can move through the product easily.

Look for:

- confusing navigation
- unclear next steps
- hidden actions
- unnecessary friction
- too many steps for simple actions

Evaluate whether the workflow feels natural and efficient.

---

## Usability

Analyze how easy the interface is to interact with.

Look for:

- unclear button labeling
- misleading affordances
- actions that are hard to discover
- poor error handling
- unclear system feedback

Focus on real usability problems rather than stylistic opinions.

---

## Interaction Design

Review how elements behave when users interact with them.

Look for:

- missing hover or focus states
- unclear interactive elements
- inconsistent interaction patterns
- lack of feedback after actions

Identify areas where interaction clarity could be improved.

---

## Consistency

Evaluate whether the UI maintains consistent patterns.

Look for:

- inconsistent spacing
- inconsistent typography
- inconsistent button styles
- inconsistent terminology
- inconsistent component behavior

Consistency issues often reduce trust and usability.

---

## Information Density

Assess whether the UI contains:

- too much information
- too little context
- poorly prioritized content
- excessive scrolling
- unnecessary duplication

Identify where content can be simplified or structured better.

---

## Professional Design Quality

Evaluate whether the interface feels:

- polished
- intentional
- well-designed
- product-grade

Identify elements that feel:

- amateur
- unfinished
- visually unbalanced
- inconsistent with modern product standards

---

# Output Format

Produce feedback using the following structure.

# UI / UX Review

## Major UX Issues
Critical usability problems that should be addressed first.

- issue
- location
- why it hurts usability
- suggested improvement

## Design Weaknesses
Areas where the interface could be improved visually or structurally.

- issue
- location
- suggested improvement

## Interaction Issues
Problems with how the UI behaves when users interact with it.

- issue
- location
- improvement suggestion

## Clarity & Usability Improvements
Smaller but meaningful improvements that increase usability.

## Professional Polish Suggestions
Refinements that would make the interface feel more polished and intentional.

---

# Review Rules

- Provide honest critique rather than polite approval.
- Focus on usability and product quality.
- Avoid subjective aesthetic commentary without justification.
- Always explain *why* something is problematic.
- Suggest practical improvements where possible.
- Avoid generic design advice.

The feedback should read like a **professional design review delivered to a product team.**

## Fresh Analysis Requirement

Always perform a **fresh analysis of the current codebase** when running this skill.

Do NOT rely on:
- previous analyses
- cached reasoning
- earlier summaries
- previously reported issues

Before producing any findings:

1. Re-scan the relevant files in the repository.
2. Re-evaluate the current implementation.
3. Confirm that each issue still exists in the latest code.
4. Ignore previously reported issues unless they are verified again in the current code.

If the code has changed since the last review, treat the review as **a completely new audit**.

Only report findings that are **confirmed in the current codebase**.

## Review Procedure

Follow this process every time:

1. Discover all relevant files in the repository.
2. Read the files directly before making conclusions.
3. Analyze the actual implementation.
4. Only then produce the audit report.

Never assume behavior without reading the source code.

Always assume the code may have changed since the last run.

Never trust previous conclusions without verifying them again.