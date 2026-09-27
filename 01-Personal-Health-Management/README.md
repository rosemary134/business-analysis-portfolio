# Personal Health Record Management - UI/UX & Business Analysis

**Role:** Business Analyst Intern
**Tech:** Figma, BABOK, Use Case, BPMN

## Overview
This project analyzed the business requirements and designed the
UI/UX for a personal health record management app, addressing a gap
in Vietnam's health-data ecosystem: medical records are scattered
across facilities, and existing e-BHYT / health-tracking apps
(VssID, VNeID) aren't optimized for personal record management.

## Problem
- Patient medical data fragmented across multiple healthcare facilities
- Electronic BHYT (health insurance) card adoption exists, but user
  experience around it remains inconsistent
- No single app lets users manage their full health record — insurance
  info, exam history, and upcoming re-exam schedules — in one place
- Health data is sensitive, so any solution needs security and
  privacy built into the design from the start, not added later

## Elicitation
Combined a real user survey with competitive analysis rather than
working from assumptions:
- **Online survey** (Google Forms), 40 valid responses — covering age
  distribution, current app usage, feature demand, and comfort with
  storing health data on a personal device
- **Competitive analysis** of VssID and VNeID's Sổ sức khỏe điện tử
  against the proposed feature set, to identify gaps rather than
  duplicate existing solutions

**Key findings:**

| Metric | Result |
|---|---|
| Currently use VNeID / VssID | 62.5% / 42.5% (10% use neither) |
| Top requested feature | "View exam details" — 50% |
| Comfortable storing health data on device | 77.5% (20% privacy-concerned) |

| Feature | VssID | VNeID (Sổ sức khỏe điện tử) | This project |
|---|---|---|---|
| Personal info | ✓ | ✓ | ✓ |
| BHYT card | ✓ | ✓ | ✓ |
| Exam history | ✓ | ✓ | ✓ |
| Exam detail view | ✓ | ✓ | ✓ |
| Health record | Limited | ✓ | ✓ |
| Re-exam reminder | Not a core feature | Not a core feature | ✓ |

The gap analysis directly shaped the scope: re-exam reminders became
a core feature specifically because neither existing app treats it
as one.

## Requirements approach

### Use Case Diagram
Defined 2 actors (User, Admin) and 4 use cases - View Personal Health
Record (includes View Personal Info, View Basic Health Info, View
BHYT Info), View Exam History (extends to View Exam Detail), View
Re-exam Reminders, and Manage Record Data (includes View Statistics,
Search Users, View User Record, Update Record Status) - using
include/extend to separate mandatory sub-functions from optional ones.
![BPMN](./UseCase-Personal-Health-Management-App.drawio.png)
### BPMN
Modeled the process with a business-level BPMN (User / System / Admin
lanes), scoped to decisions a non-technical stakeholder needs to
follow - implementation-level steps (database queries, data
retrieval) are intentionally left out and documented separately for
the dev team instead.

![BPMN](./BPMN-Personal-Health-Management-App.drawio.png)

Specified 6 functional requirements (e.g., "the system shall let users
view a detailed record of a specific exam visit") and 6 non-functional
requirements covering usability, performance, security, privacy,
consistency, and accessibility — with security and privacy defined
as first-class requirements from the analysis stage, given the
sensitivity of health data.

## Design
Built the information architecture around two distinct experiences:
- A mobile bottom-nav layout for User (home, exam schedule, exam book,
account, with a shortcut QR button for BHYT lookup). 
<img width="158" height="331" alt="image" src="https://github.com/user-attachments/assets/ca45f1a5-213f-4c57-9d5d-a71322c64fb3" />
<img width="158" height="331" alt="image" src="https://github.com/user-attachments/assets/46fc248c-dcbc-4070-a83b-eb16db532c76" />
<img width="158" height="331" alt="image" src="https://github.com/user-attachments/assets/7bf71938-f594-4e0e-bd15-4f97f0d4deff" />
- A desktop sidebar dashboard for Admin. Delivered as a connected Figma prototype
from wireframe through high-fidelity screens, with visual hierarchy
prioritizing the data users need to see first (name, facility,
exam date, BHYT status) over detail views.

## Result
Usability-tested with Guerrilla testing and a System Usability Scale
survey, n=25 participants, averaging **79.5/100** (range 72.5-85.0)
- most participants scored 75–85, indicating the core flows are
usable without heavy guidance.

## Reflection
This stage is a validated prototype, not a production system - it
isn't connected to a real database, and security requirements are
defined at the analysis/design level but not yet implemented or
tested on a live system. Usability testing was also done at a small
scale (Guerrilla testing), so it's a directional signal, not a
definitive usability claim. Both are named as next steps rather than
hidden gaps.

## Contact
linkedin.com/in/thao-nguyen-huong | nguyenhuongthao1304@gmail.com
