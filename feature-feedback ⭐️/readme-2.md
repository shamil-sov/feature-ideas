# In-App Feature Feedback

## Can this be a standalone feature?

🔴 No. It should be a shared platform capability that any feature can use.

## Draft UI

![In-app feedback prompt, optional reason, stored data, and internal dashboard](image.png)

## The idea

Occasionally ask users for quick feedback after they use a feature:

- 👍 Love it
- 😐 It’s okay
- 👎 Needs improvement

If they choose a negative rating, they can select a reason and optionally add a short comment.

## When it appears

The prompt can appear after an AI video, profile summary, hashtag generation, new onboarding flow, or another experimental feature.

Feedback should always be quick, optional, and shown occasionally rather than after every use.

## Feedback flow

1. The feature finishes.
2. BandLab asks for a simple rating.
3. A negative rating can open quick reasons such as inaccurate result, unexpected content, hard to use, or too slow.
4. The user can add an optional comment.
5. BandLab confirms that the feedback was received.

## Shared feedback service

Instead of building a separate system for every feature, all features can send feedback to one service.

Each entry could include:

- Feature name
- Rating
- Optional reason and written feedback
- Timestamp
- Platform and app version
- Useful user or feature context, where appropriate

An internal feedback page can show totals and let teams filter by feature, rating, date, user segment, and platform. Teams could also export results for deeper analysis.

## Why it matters

Analytics show what users did, but not always how they felt. An AI video may be generated successfully while still feeling irrelevant or disappointing.

In-App Feature Feedback could:

- Separate technical success from user satisfaction
- Show perceived quality, usefulness, and common frustrations
- Help teams improve AI, experimental features, and new flows faster
- Add user sentiment to existing usage data
- Catch poor experiences before they make users stop using a feature

## First version

- Add the prompt to selected feature journeys.
- Support three rating options.
- Let users add an optional reason or comment.
- Store feedback in the shared service.
- Provide an internal page for viewing and filtering responses.
