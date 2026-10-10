# Spam calibration research supplement

Reproducibility materials for **Ham Calibration Budgets and Score Tail Failures in Low False Positive Spam Filtering**.

## Download

**[Download the complete experiment and manuscript ZIP](https://github.com/ianliuy/spam-calibration-supplement/releases/download/v1.0.0/spam-calibration-review-supplement.zip)** (61,904,643 bytes, about 62 MB).

[Versioned release page](https://github.com/ianliuy/spam-calibration-supplement/releases/tag/v1.0.0). The ZIP is a release asset; GitHub's automatic "Source code" archives contain only this repository's landing-page files.

SHA-256:

```text
c480abce7a13be735917c68ba2ab67480ac81a608a28b96464d787fcbf37ee71
```

## Contents

- Current four-page PDF, editable Word document and Markdown source, including references.
- Preserved extended six-page account and full diagnostic figures and tables.
- Experiment scripts, frozen protocols, dependencies, public-data acquisition information and original dataset archives.
- Five fixed splits, three training/calibration allocations, 45 model fits, 78,315 operating points and 705 summary rows.
- Split membership, numerical outputs, deterministic refit comparisons and validation records.
- A manifest containing byte sizes and SHA-256 hashes for 465 files.

## Reproduce

Extract the complete ZIP to a new folder and start with `REPRODUCTION-REVISION2.md` at its root. Use Python 3.13 and install `requirements.txt` into a virtual environment. The numerical study needs CPU Python, not any model API or the local review runtime.

For a dependency-free integrity check, run from the extracted folder:

```text
python scripts/verify_supplement.py
```

The reproduction guide includes commands for the separate numerical audit, refit and manuscript checks. Machine-specific shared-resource wrappers apply only to the original multi-project Windows machine; portable alternatives are documented. Rendering the editable document with the original renderer requires Microsoft Word on Windows. The archived final PDF and inspected page images can be read without Word.

## Data and scope

The two datasets are [SMS Spam Collection](https://doi.org/10.24432/C5CC84) and [Spambase](https://doi.org/10.24432/C53G6X), from the UCI Machine Learning Repository. Their CC BY 4.0 attribution and original notices are retained in `data/provenance.json`, dataset archives and source records. Dataset terms apply to their respective materials; this landing page does not grant an additional blanket license over the whole archive.

The five partitions share their source corpora, and calibration draws overlap. They are descriptive dependent comparisons, not independent studies. This is a research-materials release, not a statement that the manuscript has been accepted or published by a conference.

This version preserves the existing ZIP unchanged. Statements inside it about local-only availability and no prior upload describe its preparation state; this release makes that snapshot publicly downloadable. Historical review records remain tied to their original artifact hashes. The four-page edition's numerical/source and every-page visual checks are under `evidence/four-page-2026-10-09/`.
