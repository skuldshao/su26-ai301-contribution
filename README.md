# Contribution [#]: [Let user reprocess audio transcription]

**Contribution Number:** [1]  
**Student:** [Wanru Skuld Shao]  
**Issue:** https://github.com/BasedHardware/omi/issues/4601  
**Status:** [Phase I / Phase II / Phase III / Phase IV] [In Progress / Complete]

---

## Why I Chose This Issue

## Why I Chose This Issue

I chose issue #4601 "Let user reprocess audio transcription" because it
builds directly on a feature pattern that already exists in the codebase —
users can currently reprocess a conversation summary, and this issue asks
for the same capability applied to the raw audio transcription. That makes
it a good scope for me: the request isn't an open-ended new system, it's
extending an established flow, so I have a working reference to study and
mirror rather than inventing an approach from scratch.

I'm interested in this because:
1. omi's transcription pipeline runs through speech-to-text providers
   (Deepgram, Speechmatics, Soniox) on a Python/FastAPI backend, and I want
   to learn how a production app wires real-time STT together with an option
   to re-run it on stored audio.
2. The "reprocess summary" feature gives me a concrete pattern to match,
   which lowers the risk of a first contribution going off in the wrong
   direction.
3. It's a clear, user-facing improvement — the issue notes the live sync
   transcription has been failing often lately, so a manual reprocess option
   has obvious value rather than being a cosmetic change.
4. It touches both the backend (triggering a re-transcription job on saved
   audio) and the Flutter app (surfacing a "reprocess transcript" action in
   the UI), so I get exposure to an end-to-end change instead of an isolated
   snippet.

From reading the issue, I understand the current problem is that once a
conversation's transcription comes back poor, the user is stuck with it —
there's no way to ask the system to transcribe the stored audio again. My
contribution would let the user re-run transcription to get a better result,
reusing the existing reprocess-summary mechanics as the model.

[Next step before claiming the issue: leave a comment introducing myself and
confirming with a maintainer that it's still open and unassigned, and ask
which module the existing reprocess-summary logic lives in.]

---

## Understanding the Issue

### Problem Description

[In your own words, what's broken or missing?]

### Expected Behavior

[What should happen?]

### Current Behavior

[What actually happens?]

### Affected Components

[Which parts of the codebase are involved?]

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
