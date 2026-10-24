# Campus Gym Buddy

**Systems Analysis & Design | Team 10 | California State University, Los Angeles**

A student-focused platform concept for finding workout partners, forming small campus fitness groups, and organizing gym sessions.

**Project scope:** Academic systems analysis, requirements, functional modeling, and a Figma interface prototype. This repository contains design deliverables; it does not contain application source code, a deployed backend, or a verified campus login integration.

![Campus Gym Buddy interface designs](images/dashboard-preview.png)

## The Problem

Students may have access to a campus gym but struggle to find workout partners with similar goals, skill levels, and availability. The proposed system addresses coordination, confidence, and accountability through small campus workout groups.

## Proposed Features

- Student profiles with name, student email, skill level, workout goals, and verification status.
- A campus verification concept that restricts access to verified students.
- Workout group creation with a name, workout focus, skill level, and capacity.
- Groups limited to a maximum of five students.
- Group discovery and filtering by skill level, with requirements for workout-focus and capacity searches.
- Joining and leaving groups, with membership records and member counts.
- Gym session details including date, time, location, and associated group.

These are proposed requirements and prototype interactions, not claims of implemented production functionality. Improved participation and motivation are intended benefits, not measured outcomes.

## Explore the Project

| Deliverable | File |
| --- | --- |
| System proposal (PDF) | [Read the proposal](docs/system-proposal.pdf) |
| Editable system proposal | [Download the Word document](docs/system-proposal.docx) |
| Prototype screen export | [View prototype screens](docs/prototype-screens.pdf) |
| Final presentation | [Download the slides](presentation/campus-gym-buddy.pptx) |
| Interface overview | [View interface designs](images/dashboard-preview.png) |
| Use-case diagram | [View the use-case diagram](images/use-case-diagram.png) |
| Activity diagram | [View the activity diagram](images/activity-diagram.png) |

### Figma

- [Design file](https://www.figma.com/design/cQJASUKAZQzINnzF0PueTR/Campus-Gym-Buddy?node-id=2-3)
- [Interactive prototype](https://www.figma.com/proto/cQJASUKAZQzINnzF0PueTR/Campus-Gym-Buddy?node-id=249-19&scaling=contain&content-scaling=fixed&page-id=2%3A3)

These links were provided in the project proposal. Access permissions and current availability have not been independently verified. If access is restricted, use the included PDF and image previews.

## Data Model Overview

The proposal and presentation describe four core entities:

| Entity | Information represented |
| --- | --- |
| Student | Name, email, skill level, workout goals, verification status |
| Workout group | Group name, focus, skill level, capacity, status, creator |
| Group membership | Student/group association and join date |
| Gym session | Date, time, location, associated workout group |

Membership connects students and groups; a group may have multiple sessions. No database schema or SQL implementation is included in this upload.

## Functional Models

### Use Cases

The diagram identifies a Student and a Campus Verification System, with interactions for profile management, verification, group creation, group searches, joining, membership management, scheduling, and viewing details.

![Use-case diagram](images/use-case-diagram.png)

### Joining a Group

The supplied activity diagram follows dashboard access, group browsing, optional skill filtering, a capacity check, joining, member-count updates, and confirmation. Unavailable groups lead to an unsuccessful path.

![Group joining activity diagram](images/activity-diagram.png)

## Tools and Skills Demonstrated

- **Figma:** Interface design and prototyping.
- **Draw.io:** Functional modeling, as specified in the proposal.
- **Trello:** Team task tracking, documented in the supplied team board screenshot.
- **Systems analysis:** Business needs, system requests, and requirements.
- **Data modeling:** Entities, attributes, relationships, and business rules.
- **Communication:** Proposal writing, diagrams, and presentation materials.

## Team Credits

The final presentation credits:

- Brian Barrios-Hernandez
- Md Usman Goni
- Pablo Jacome

This is collaborative coursework. The supplied files do not establish a complete breakdown of individual contributions; this repository does not attribute the entire project to one member.

## Design Review Notes

The original deliverables are preserved as submitted. Some issues remain for a future revision:

- The presentation describes creator approval for joining; the supplied activity diagram and interface export show direct joining. This business rule needs to be reconciled.
- Template instructions remain in the system proposal.
- Some prototype labels, sample dates, and membership counts are inconsistent between screens.
- The use-case diagram's include/extend notation should be reviewed for direction and UML consistency.
- The proposal's bibliography is reproduced in the original documents and has not been independently verified.

## Status and Next Steps

This portfolio documents the design phase. Future development could implement authentication, persistent data storage, capacity enforcement, and tests for joining, leaving, and scheduling. Such implementation is outside the supplied materials.

## Academic Context

Prepared as a Systems Analysis & Design team project at Cal State LA. The materials do not establish university deployment or endorsement. No open-source license has been added on behalf of the team.
