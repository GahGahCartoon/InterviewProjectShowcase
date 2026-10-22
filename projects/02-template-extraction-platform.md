# Template-Based Document Extraction Platform

**Status:** Full-stack MVP

## Overview

I built a full-stack MVP that let users configure document templates, manage extraction workflows, and review extracted values through a user interface. The project addressed an important gap between an extraction model and a usable workflow: people needed a way to configure what should be processed and inspect the resulting values in the context of the source document.

The MVP was not presented as a production platform, and no claim is made about customer adoption or production traffic.

## My contribution

I developed the frontend using React, Vite, and JavaScript. I implemented UI flows for template configuration, extraction workflow scheduling and management, extracted-value review, result inspection, and document-position verification.

I integrated the frontend with backend cloud services and fine-tuned AI extraction models. This connected configuration and workflow controls with the extraction process and brought model results back into an interface where users could inspect both the values and their positions in a document. I do not claim sole ownership of any wider company platform or backend capability beyond the contributions described here.

## High-level workflow

User configures a document template → user manages or schedules an extraction workflow → backend services perform extraction → interface presents extracted values → user inspects values and their document positions

This description intentionally leaves out proprietary template definitions, internal business rules, and implementation details that are not supported for public disclosure.

## Technology

- React
- Vite
- JavaScript
- Backend cloud-service integration
- Fine-tuned AI extraction-model integration

The available brief does not establish a specific scheduler, database, cloud provider, queue, coordinate format, or backend framework, so none is attributed to the MVP.

## Engineering considerations

Making extraction configurable through an interface turned a model capability into a workflow that users could operate. Template configuration and workflow management provided control over what was processed and when, while result inspection made model output visible in its document context.

Document-position verification was especially relevant to the end-to-end experience: an extracted value on its own is less useful for review than a value that can be inspected against its source position. This does not imply a measured reduction in errors, but it explains why the review interface was part of the AI workflow rather than a separate presentation layer.

## Outcomes and limitations

I delivered an MVP combining template configuration, extraction workflow management, and visual result review. No quantified adoption, time saving, or accuracy improvement is available.

The brief does not establish production-scale validation or a completed production-readiness assessment. It also does not provide enough evidence to state which additional reliability, security, or testing work remained; those questions require further project detail rather than speculation.

## Evidence

This sanitised account describes the MVP and my contributions without publishing employer-owned code, real documents, proprietary template definitions, or internal business logic.
