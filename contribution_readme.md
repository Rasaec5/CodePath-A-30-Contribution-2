# Contribution [2]: [[Issue Title](https://github.com/ESCOMP/CTSM/issues/3693#top)]

**Contribution Number:** [2]  
**Student:** Clayton Williams  
**Issue:** https://github.com/ESCOMP/CTSM/issues/3693  
**Status:** [Phase I]

---

## Why I Chose This Issue

While Fortran is new to me I was reading through the code and it looks a lot like Progress which I have some experience with from work. I think this will be a good issue for me to try something a little bit more challenging and try learning something new.

---

## Understanding the Issue

### Problem Description

The issue asks to refactor duplicated "move excess soil water upward" logic that currently appears in three places (twice in SoilHydrologyMod.F90, once in SoilWaterMovementMod.F90) into a single shared function. The code checks each soil layer for oversaturation and, if found, shifts the excess water up one layer (or off as runoff if it's the top layer). It's tagged as a code-health cleanup, must remain bit-for-bit identical to current behavior, and is labeled "good first issue" / "size: small," though it's unassigned with no urgent milestone.

### Expected Behavior

use 1 module to perform the repetitive task

### Current Behavior

seperate functions to perform the same task

### Affected Components

SoilHydrologyMod.F90, SoilWaterMovementMod.F90

---

## Reproduction Process

### Environment Setup

[Notes on setting up your local development environment - challenges you faced, how you solved them]

### Steps to Reproduce

1. [Step 1]
2. [Step 2]
3. [Observed result]

### Reproduction Evidence

- **Commit showing reproduction:** [Link to commit in your fork]
- **Screenshots/logs:** [If applicable]
- **My findings:** [What you discovered during reproduction]

---

## Solution Approach

### Analysis

[Your analysis of the root cause - what's causing the issue?]

### Proposed Solution

[High-level description of your fix approach]

### Implementation Plan

Using UMPIRE framework (adapted):

**Understand:** [Restate the problem]

**Match:** [What similar patterns/solutions exist in the codebase?]

**Plan:** [Step-by-step implementation plan]
1. [Modify file X to do Y]
2. [Add function Z]
3. [Update tests]

**Implement:** [Link to your branch/commits as you work]

**Review:** [Self-review checklist - does it follow the project's contribution guidelines?]

**Evaluate:** [How will you verify it works?]

---

## Testing Strategy

### Unit Tests

- [ ] Test case 1: [Description]
- [ ] Test case 2: [Description]
- [ ] Test case 3: [Description]

### Integration Tests

- [ ] Integration scenario 1
- [ ] Integration scenario 2

### Manual Testing

[What you tested manually and results]

---

## Implementation Notes

### Week [X] Progress

[What you built this week, challenges faced, decisions made]

### Week [Y] Progress

[Continue documenting as you work]

### Code Changes

- **Files modified:** [List]
- **Key commits:** [Links to important commits]
- **Approach decisions:** [Why you chose certain approaches]

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**
- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained

[What you learned technically]

### Challenges Overcome

[What was hard and how you solved it]

### What I'd Do Differently Next Time

[Reflection on your process]

---

## Resources Used

- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
