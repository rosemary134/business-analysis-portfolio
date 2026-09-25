# NauCom - Cooking Recipe Android App

**Role:** Project Lead, Business Analyst, UI designer (Team of 3)  
**Tech:** Java, Android Studio, Spoonacular API, Firebase, Google Translate API

## Overview
NauCom is an Android application that helps users discover cooking
recipes based on available ingredients, plan meals, and manage their
favorite dishes - with full Vietnamese language support via
translation integration.

## Problem
Vietnamese users relying on international recipe databases like
Spoonacular face a language barrier, while busy households often
waste food from unused ingredients. NauCom addresses both with
ingredient-based recipe discovery and automatic Vietnamese translation.

## Elicitation
The idea originated from the team itself - one member regularly cooked
and kept having to pull recipe information from multiple scattered
sources. The team scoped the brief from that real friction point; our
academic supervisor's role was limited to confirming the topic was
suitable, not shaping the requirements.

## Requirements approach
Requirements were captured in a BRD (10 functional requirements,
MoSCoW-style priority), broken into 7 use cases, and detailed as user
stories with Gherkin acceptance criteria. Business-level BPMN diagrams
model the authentication and recipe-search processes at the process
level intended for stakeholders; a separate technical activity diagram
documents the implementation flow for the dev team.

## Documentation
- [BRD](./BRD-NAUCOM-001.pdf): Business Requirements Document and Functional Requirements
- [Use Case Diagram](./Use-Case-Diagram/): System interactions between actors and features
- [User Stories](./User-story.pdf): Functional requirements in user story format
- [BPMN & Activity Diagram](./BPMN-&-Activiti-Diagram.pdf): Business-process-level flows (authentication, recipe search) and Technical sequence flow for the dev handoff

## My Role - Business Analyst
- Led requirement elicitation, user story creation, and functional requirements
  specification for recipe search, meal planning, and authentication
- Modeled business processes with BPMN and technical implementation flow
  with activity diagrams, kept as separate artifacts for their intended audiences
- Designed wireframes and led sprint planning under Agile/Scrum workflow
- Oversaw development using Firebase Authentication, Firestore, and
  third-party API integration

## Figma UI Design
- UI Design: bit.ly/naucomapp-figma

## Features
- Recipe search via Spoonacular API
- Meal planning calendar
- Firebase Authentication & Firestore sync
- Favorites & search history
- Vietnamese recipe translation

## Result
All planned features were completed and functional, with data flows
tested manually across the app before final submission.

## Reflection
Revisiting this project after mentor feedback, I corrected two
modeling issues: the use case diagrams had over-decomposed input
fields into separate use cases, and two diagrams mislabeled a
technical sequence flow as BPMN. Both are now modeled at the correct
level for their intended audience — a distinction that now carries
into how requirements are documented across all of this portfolio's
projects.

## Status
✅ Completed - Team Project (3 members)

## Contact
linkedin.com/in/thao-nguyen-huong | nguyenhuongthao1304@gmail.com
