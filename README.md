# Neuroscience Research Intelligence System

**Helps researchers work across literature, datasets, BIDS/NWB standards, EEG/MEG/fMRI-style pipelines, reproducibility, and open science.**

## Purpose
Domain-specific system for neuroscience research intelligence. Research infrastructure only — no medical or clinical claims.

## How People Experience It
Neuroscientists:
- Scout literature and public datasets (OpenNeuro, DANDI).
- Validate BIDS compliance.
- Run reproducible pipelines with MNE-Python.
- Generate QC reports and NWB exports.
- Build claim graphs tied to personal research canon.

## How Agents Explore It
- neuroresearch.yaml
- agents/ (neuro-literature-scout, bids-nwb-specialist, mne-pipeline-engineer, neurodata-engineer, reproducibility-engineer)
- skills/ (paper-ingestion, openneuro-dataset-scout, dandi-nwb-scout, bids-validator, mne-eeg-pipeline, neuroimaging-qc-report)
- workflows/ (literature-to-claim-graph.md, dataset-to-reproducible-pipeline.md, bids-qc-loop.md)
- schemas/ (neuro-paper.schema.json, neuro-dataset.schema.json, pipeline-run.schema.json)
- notebooks/

**Example Prompt**:
"As mne-pipeline-engineer + bids-nwb-specialist, using latest MNE 1.8+ and BIDS 1.10 / NWB 2.7, process this EEG dataset. Generate QC report and export to NWB. Reference human-mind attention and perception models. Output pipeline-run.schema.json."

## Usefulness
- **Humans**: Makes complex neuro data work reproducible and faster.
- **Agents**: Specialized agents for standards-heavy domain.
- **Integrations**: Full stack with Research OS, Research Intelligence Systems, and personal Agentic Mind OS.
- **Latest Best Tech**: BIDS 1.10, NWB 2.7, MNE-Python 1.8+, SpikeInterface, DANDI, containerized pipelines, structured outputs.

See neuroresearch.yaml, AGENTS.md, HERMES.md, EXPERIENCE.md.

Guardrail: Research workflow infrastructure only.