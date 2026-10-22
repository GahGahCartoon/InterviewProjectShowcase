# Computer Vision Model Suite for Scanned Documents

**Status:** Models built and evaluated, with Docker-based model hosting; deployment status is not specified for every model

## Overview

I built and evaluated computer vision models for three scanned-document tasks: signature detection, checkbox detection/classification, and signature similarity comparison. The work included scanned-image preprocessing, task-specific model development and evaluation, and Docker-based model hosting.

These were distinct technical problems. Detection locates an object or region, classification assigns a task-specific category, and similarity comparison estimates how closely two signature representations resemble one another. They should not be described or evaluated as if they were interchangeable.

## My contribution

I worked with Python and PyTorch to build and evaluate models for the three tasks. I prepared scanned images for inference through preprocessing and worked on Docker-based hosting so model capabilities could be run as services or integrated into a broader document-processing workflow.

My contribution covered model work and hosting, but the available resume brief does not establish that every model reached production. I therefore do not generalise one model's deployment status, evaluation conditions, or result to the entire suite.

## High-level workflow

Scanned image → preprocessing → task-specific model inference → task-specific output → evaluation or integration into a document-processing workflow

The exact output and integration path depended on the task. No universal output schema or identical downstream integration is claimed for every model.

## Technology

- Python
- PyTorch
- Scanned-image preprocessing
- Docker-based model hosting

Specific architectures, training losses, dataset sizes, thresholds, and serving frameworks are intentionally not assigned to the models because those details are not provided in the public brief.

## Engineering considerations

Each task required evaluation against its own objective. A detector's localisation behaviour, a checkbox classifier's category decisions, and a signature-comparison model's similarity output answer different questions. A single aggregate figure cannot establish identical performance across them.

Signature similarity comparison also has an important scope boundary: it is not, by itself, verified identity authentication, fraud detection, or forensic signature verification. Those claims would require different evidence, controls, and evaluation protocols.

## Outcomes and limitations

The resume reports over 95% accuracy on selected tasks under controlled scanned-document conditions. This is a selected-task result, not a claim that every model achieved the same performance or that the result generalises to arbitrary images.

The public brief does not provide per-task metric definitions, test-set sizes, class balance, threshold settings, or precision/recall-style measures. It also does not identify which individual models were deployed to production. Those limitations prevent a more granular comparison without inventing evidence.

## Evidence

This case study contains no customer images, proprietary training data, model weights, or internal evaluation samples. It is a sanitised account of the tasks, contribution, technology, and resume-reported outcome.
