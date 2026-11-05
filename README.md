# Sukupolut

**Source-based genealogy, connected through people and places.**

Sukupolut is a Finnish-language local research application that turns historical records into connected, searchable observations. It brings together people, families, places and source references while preserving uncertainty and the original wording of each record.

## The problem

The same person may appear under different names, dates and households across historical records. A single corrected family tree can hide the evidence behind a conclusion. Sukupolut keeps the person, the source observation and the researcher's interpretation separate.

## What works today

- Source-specific entry forms for historical Finnish records.
- Person search, life events, family relationships and a family-tree view.
- Place hierarchies and map locations with source references.
- Migration records linked to departure and destination places.
- Corrections, duplicate-person merging and traceable source observations.
- Local SQLite storage and a separate read-only mode.

## Technical approach

| Area | Implementation |
| --- | --- |
| Backend | Python standard library and a local HTTP server |
| Database | SQLite with relational links and source observations |
| Interface | HTML, CSS and JavaScript |
| Maps | Leaflet |
| Data model | People and places separated from source-specific observations |

## Project status

Working local prototype, actively developed. Updated 5 November 2026. This is a personal software and data-modelling project, not a hosted multi-user service.

The application source code and research material are maintained privately. This public overview contains no research database or personal records.

## What this project demonstrates

Relational data modelling, translating research workflows into usable forms, Python development, handling inconsistent historical evidence and connecting structured data to a visual interface.

**Created by [Laura Paasonen](https://github.com/LaraDeWalt).**
