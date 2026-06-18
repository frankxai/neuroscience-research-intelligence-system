# MNE EEG Pipeline Skill

## Trigger
User has EEG data (BIDS or raw) and wants to run standard preprocessing and analysis.

## Inputs
- Dataset path (BIDS compliant preferred)
- Task description
- Channels of interest

## Steps (Latest Best Tech 2026)
1. Load with MNE-Python 1.8+ (use mne.io.read_raw for BIDS).
2. Preprocess: Filtering (1-40Hz), ICA for artifacts (latest ICA methods).
3. Epoching and averaging.
4. Time-frequency analysis with Morlet wavelets.
5. Source localization if MRI available (using MNE's forward models).
6. Generate QC report with latest visualization.
7. Export to NWB if needed using pynwb.
8. Log for reproducibility (use research-os contracts).

## Outputs
- Processed epochs, evoked responses.
- QC HTML report.
- Pipeline-run.schema.json output.

## Agent Usage
"Run mne-eeg-pipeline on this BIDS EEG dataset for oddball task. Use latest MNE features. Output structured."

## Excellence & Usefulness
Uses latest MNE features for high quality, reproducible EEG research. Integrates with bids-validator and neurodata-engineer.

Guardrail: Research only, no clinical.