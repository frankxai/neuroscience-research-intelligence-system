# BIDS Validator Skill

## Trigger
User has a dataset folder or wants to check BIDS compliance before analysis.

## Inputs
- Path to dataset directory
- Optional: modality (EEG, MRI, etc.)

## Steps
1. Run bids-validator (or equivalent tool) on the path.
2. Parse output for errors/warnings.
3. Map errors to actionable fixes using BIDS spec knowledge.
4. Generate BIDS QC report using templates from research-intelligence-os.
5. Suggest MNE or NWB conversion steps if needed.
6. Update reproducibility log.

## Outputs
- QC report (markdown or JSON)
- Fixed dataset recommendations
- Links to openneuro or DANDI scouts

## Agent Usage
"Validate this BIDS dataset for EEG. Output using bids-qc-loop workflow."

## Usefulness
Ensures datasets are ready for pipelines in mne-pipeline-engineer or neurodata-engineer agents.
Reduces errors in reproducible neuroscience research.