# VNeID UX Research, Design & Evaluation
**Role:** Project Lead (University Scientific Research)  
**Tech:** Figma, Framer, SUS Framework, UEQ Framework

## Overview
VNeID is Vietnam's national digital identity app, used by 55M+
citizens. Despite its scale, the app faces significant usability
issues - particularly around authentication complexity and
accessibility for low-tech-literacy users.

This project led a full UX research cycle, including targeted
analysis of negative user feedback across app stores and social
media, to identify pain points and design evidence-based solutions.

## Problem
- 55M+ active users relying on VNeID for essential government services
- Complex, repetitive authentication flow
- Multiple usability issues affecting everyday use
- Low accessibility for users with limited tech literacy

## Elicitation
As a university scientific research project, the brief was
self-initiated - I identified VNeID's usability gap through its
scale and public complaint volume, then proposed the research scope
to my faculty advisor. From there, elicitation combined quantitative
and qualitative sources rather than a single method:
- **Online Survey** (n = 205)
- **Social Listening** (Facebook, TikTok) - 162 comments
- **App Store + Google Play Negative Review Mining** - 562 reviews

## Methodology
- **User-Centered Design (UCD)** — ISO 9241-210
- **Design Thinking** - Empathize, Define, Ideate, Prototype, Test
- **SUS (System Usability Scale)** - quantitative usability scoring
- **UEQ (User Experience Questionnaire)** - qualitative experience evaluation

## Solutions
Designed and prototyped **6 UX improvements** using Figma and Framer,
each tied back to a specific pain point surfaced in elicitation:

1. **Optimized Authentication** - one-time verification instead of
   repeated passcode entry, addressing the authentication-complexity
   complaints most cited in review mining
2. **Guided Checklist** - step-by-step instructions at the start of
   each procedure, targeting low-tech-literacy drop-off
3. **Draft Saving** - auto-save progress with a non-destructive "Back" button
4. **Chatbot Support** - integrated assistant for real-time help
5. **Offline Mode** - view saved documents without internet access
   directly addressing low-connectivity complaints from review mining
6. **Status Timeline** - color-coded tracking for application progress

## User Flow — from solution to implementable logic
To translate solutions #1 (Optimized Authentication) and #5 (Offline
Mode) into implementable logic, I mapped the full "Ví giấy tờ"
authentication flow for both connectivity states:

- **Online flow:** passcode verification with a failed-attempt
  limit before temporary account lock - a deliberate trade-off,
  accepting a small security cost for a large usability gain,
  validated against the failed-attempt lock mechanism.
<img width="7352" height="1814" alt="image" src="https://github.com/user-attachments/assets/8345ed28-7c2a-4ec5-b7e6-49617ed33d43" />

- **Offline flow:** falls back to locally cached documents
  instead of blocking access entirely, directly addressing the
  low-connectivity complaints surfaced in the negative-review mining.
<img width="6494" height="1934" alt="image" src="https://github.com/user-attachments/assets/4f9def74-c2ee-4618-b315-fbe678b94a6f" />

## Result
- Test participants: 51 (qualitative) + 61 (quantitative)
- Overall SUS Score: **88.25 / 100** - "Excellent" (Bangor scale)
- Low-tech-literacy users (SUS improvement): **42.5 → 77.5**

## Prototype

**Figma Prototype:**
- bit.ly/vneid-prototype-figma

**Framer:**
- **Offline Mode Prototype:** bit.ly/vneid-prototype-offline-framer
- **Chatbot Prototype:** bit.ly/vneid-prototype-chatbot-framer

## Reflection
The biggest lesson was translating research findings into
implementable decisions with real trade-offs - e.g., choosing
one-time verification over repeated passcode entry meant accepting
a small security trade-off for a large usability gain, a call that
only made sense once weighed directly against what the review
mining showed users actually struggled with.

## Contact
linkedin.com/in/thao-nguyen-huong | nguyenhuongthao1304@gmail.com
