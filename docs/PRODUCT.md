# Product brief

[Overview](../README.md) · [User guide](../GUIDE.md) · [Roadmap](ROADMAP.md)

## Problem and first audience

Students juggle classes, assessment deadlines, preparation work and personal plans across multiple systems. Knowing a due date does not answer what to do next or where the work fits. Campus Rhythm starts with this planning gap rather than treating imported calendar entries as a finished plan.

The first audience is students, initially in an HKUST context with institution-specific import guidance. Expanding to people with tight schedules is a product direction, not a validated claim of fit across occupations or institutions.

## Intended experience

| Need | Product response | Decision rule |
| --- | --- | --- |
| Bring an existing semester into the app | Source-specific import guidance and preview. | The user selects records before saving. |
| Decide what needs attention | One explained next action on Today. | Consider available deadlines, remaining effort and preferences; unknown information stays explicit. |
| Make preparation possible | Keep due dates separate from work sessions. | Respect fixed commitments and saved rest windows in supported planning paths. |
| Correct the assistant | Reviewable drafts and supported undo. | A model response does not directly authorize a write. |
| Understand the week | Completion history and weekly review. | Recorded work and scheduled work remain different quantities. |
| Stay aware without oversharing | Opt-in reminders and native title-privacy controls. | Native behavior requires device acceptance. |

## An example journey

An illustrative student imports classes and deadlines, then reviews the items before saving. A project needs two hours of work; the student supplies the remaining effort and checks the suggested sessions against their fixed classes. After confirming a draft, they record progress, undo an accidental completion, and inspect the weekly review.

The product should reduce the amount of repetitive planning in that journey. It does not infer official assessment weights from a title, treat a planned session as finished work, or promise a correct interpretation of every free-text request.

## Current scope

The web prototype connects imports, calendar, assistant drafts, confirmation, task execution and review. A shared Expo/React Native implementation supports iOS development. Accounts and synchronization have implementation evidence but still need a broader unassisted, multi-device acceptance cycle.

Wellness and community are supporting directions. Native Apple Health reading exists, but real-device readings and useful health-aware scheduling remain unfinished acceptance. A complete social planner, continuous external calendar sync, connected Outlook/email access and autonomous replanning are not claimed as shipped.

## Research questions

1. Can a new student complete the first import without help?
2. Do they understand why Today recommends a particular action?
3. How often must they correct an assistant draft before confirming it?
4. Does the product reduce planning effort without increasing unwanted alerts?
5. Do recorded progress and weekly review support repeat use?

These questions need observed behavior and follow-up data. A prepared survey or a convenience sample alone does not demonstrate retention, wellbeing improvements or market demand.
