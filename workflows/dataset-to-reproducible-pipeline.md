# Dataset to Reproducible Pipeline Workflow

## Goal
Turn a public or local neuro dataset into a fully reproducible analysis pipeline.

## Steps
1. Scout dataset (openneuro-nwb-scout or dandi-nwb-scout skill).
2. Validate with bids-validator skill.
3. Ingest metadata into neuro-dataset.schema.json.
4. Choose pipeline (mne-eeg-pipeline or custom).
5. Run pipeline with logging.
6. Generate neuroimaging-qc-report and reproducibility report.
7. Export to claim graph in research-intelligence-systems if applicable.

## Agent Orchestration
Use bids-nwb-specialist + mne-pipeline-engineer + reproducibility-engineer.

## Example
"Take this OpenNeuro ds003645 dataset, validate, run basic ERP pipeline with MNE, produce QC and repro report."

## Usefulness
Makes open data actually usable for agents and humans. Directly supports open science and the neuroscience vertical.