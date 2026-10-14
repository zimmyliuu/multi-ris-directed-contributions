# Research Code and Data for Multi-RIS Directed Contributions

**Associated manuscript:** Identifiable Directed Contributions in Multi-RIS Scattering: Receiver-Only Estimation and Calibrated Reliability  
**Author:** Ziming Liu  
**Affiliation:** BELL Honors College, Nanjing University of Posts and Telecommunications  
**Contact:** zimmyliuu@gmail.com

This repository accompanies the manuscript with a curated research implementation, frozen simulation results, calibration records, and figure-reproduction inputs. The scientific package contains 900 fresh geometries with four paired estimators per geometry.

## Download

**Version 1.0.0 DOI:** [10.5281/zenodo.23357653](https://doi.org/10.5281/zenodo.23357653), published 14 October 2026.

The complete scientific package is distributed as the release attachment **Research_code_and_saved_results.zip**.

- [Download Research_code_and_saved_results.zip](https://github.com/zimmyliuu/multi-ris-directed-contributions/releases/download/v1.0.0/Research_code_and_saved_results.zip)
- [Release v1.0.0](https://github.com/zimmyliuu/multi-ris-directed-contributions/releases/tag/v1.0.0)
- Archive size: **33,268,745 bytes**
- SHA256: `46c1861ced9a1b428d163c6a60309bb4378df7c10ca340d8b4294993d3807e19`

Release v1.0.0 is published, and the complete research package is available through the download link above. Download the attachment named **Research_code_and_saved_results.zip**. The automatically generated **Source code (zip)** and **Source code (tar.gz)** archives at this release contain only the repository's wrapper metadata and do not contain the research package.

The research ZIP contains 373 files: 372 files covered by its integrity manifest, plus the manifest itself. All 372 manifest sizes and SHA256 hashes were verified before repository preparation.

### Zenodo archive

The same scientific files are archived in [Zenodo record 23357653](https://zenodo.org/records/23357653) as **eight independent ZIP parts** plus `README_ZENODO_PARTS.txt`. Download all eight files named `Research_code_and_saved_results_part_01_of_08.zip` through `Research_code_and_saved_results_part_08_of_08.zip`, then extract every part into the **same new directory**, preserving relative paths. Each part is a valid ZIP; do not concatenate their binary contents.

Together the eight parts reproduce all 373 files in the original GitHub research ZIP byte for byte. The public Zenodo record's nine filenames, sizes, and MD5 checksums were checked against the prepared local distribution. The original single ZIP remains available from the GitHub release above.

## Integrity verification

Extract either the single GitHub research ZIP or all eight Zenodo ZIP parts into a new directory. From the extracted package directory, run:

```sh
python verify_integrity.py
```

This check uses only the Python standard library, does not require network access, and runs no simulations. Keep an unchanged copy of the extracted package before optional numerical reproduction, because historical reproduction scripts can overwrite outputs.

## Package map

Paths below are relative to the extracted research package.

| Path | Contents |
| --- | --- |
| `README.txt` | Package instructions, dependencies, provenance, and reproduction limitations |
| `MANIFEST_SHA256.json` | File sizes and SHA256 hashes |
| `DISTRIBUTION_PROVENANCE.json` | Original archive hashes and curation record |
| `research/outputs/ris_paper/confirmatory_trials.jsonl` | All 900 fresh confirmation geometries and four paired estimators |
| `research/outputs/ris_paper/results.json` | Summary statistics |
| `research/outputs/ris_paper/summary.csv` and `paired_comparison.csv` | Tabular results and paired comparisons |
| `research/outputs/ris_paper/frozen_plan.json` | Fixed study plan and frozen numerical source hashes |
| `research/outputs/ris_multi/calibration_mismatch.json` and `calibration_risk.json` | Saved independent calibration samples |
| `research/outputs/ris_multi/mismatch_models.json` and `risk_models.json` | Frozen screening and joint-risk rules |
| `research/outputs/ris_multi/sequence_main.json` | Bounded four-board extension |
| `research/work/ris_paper/` | Confirmation study and cubic-ridge comparator |
| `research/work/ris_multi/` | Forward model, receiver estimator, and reliability decisions |
| `figure_rebuild/` | Four-figure rebuilding code, saved inputs, and plotting instructions |

The package also preserves the earlier double-RIS, physical-model, and robust-estimation source and evidence used by the manuscript. Refer to its README for the pinned numerical environment and explicit reproduction commands.

## Scientific scope

The work concerns identifiable coexisting directed RIS contributions under a stated quasistatic scalar model with known absolute controls. The main evidence uses three RIS boards and separately calibrated joint coefficient-error screening. The package also includes the bounded four-board extension described in the manuscript.

Ordered targets are contributions to commuting Taylor coefficients, rather than separately observed Taylor coefficients. Reliability guarantees depend on the specified calibration distribution and acquisition conditions. The evidence does not establish general unknown-topology recovery, three-dimensional full-wave validation, or hardware performance. Later all-orders and RIS-count scaling studies are outside this package.

## Provenance

The research package was curated on 12 October 2026 from the frozen 3 October 2026 research archive. Retained scientific file bytes were preserved, and no new simulations or parameter tuning were performed during packaging or repository preparation.

The archive retains its historical supplement labels and preparation context for traceability. The associated manuscript title above identifies this repository's current research context. Old operational records, obsolete manuscript drafts, third-party full-text articles, and an unlicensed MATLAB reference file were excluded from the curated package.

Historical workspace-preservation checks can expect ancillary files that were deliberately excluded. Use the included `verify_integrity.py` and distribution manifest to verify this package; the package README explains the distinction.

## Citation and reuse

Citation metadata is provided in [CITATION.cff](CITATION.cff). Cite this archived version using DOI [10.5281/zenodo.23357653](https://doi.org/10.5281/zenodo.23357653):

Liu, Ziming. (2026). *Research Code and Data for "Identifiable Directed Contributions in Multi-RIS Scattering: Receiver-Only Estimation and Calibrated Reliability"* (Version 1.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23357653

No new reuse license is granted by this repository. Public availability alone does not confer a software or data reuse license. Contact the author for permissions.
