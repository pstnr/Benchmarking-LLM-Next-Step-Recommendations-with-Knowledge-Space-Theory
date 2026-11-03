# Benchmarking LLM Next-Step Recommendations with Knowledge Space Theory

Reproducible supplementary analysis by **Peter Steiner** and **Jan Hochweber**, Institute of Educational Psychology, St.Gallen University of Teacher Education (PHSG), Switzerland.

- Peter Steiner: [ORCID 0009-0001-5491-9464](https://orcid.org/0009-0001-5491-9464)
- Jan Hochweber: [ORCID 0000-0002-7855-2097](https://orcid.org/0000-0002-7855-2097)

The scientific analysis corresponds to the manuscript dated 29 September 2026. Release **v1.0.0** identifies the public supplement with updated documentation, citation metadata and licensing. An arXiv identifier has not yet been added.

## Reproduce the analysis

Requires **Python 3.10 or later** (originally tested with 3.12.10). The script uses only the Python standard library; no API keys or model calls are needed.

From the repository directory, run:

```sh
python reproduce.py
```

Alternatively, open [KST_Reproducible_Companion.ipynb](KST_Reproducible_Companion.ipynb) in Jupyter and run all cells in order. Jupyter is needed only for the notebook interface.

Inputs are embedded in both the script and notebook. Results are written to `reproduced_results/` relative to the current working directory. Re-running the analysis overwrites those outputs.

A successful run ends with:

```text
PASS: all six tables and overall/order/terminal statistics reproduce the archived analysis.
```

## Repository contents

| Path | Contents |
| --- | --- |
| `KST_Reproducible_Companion.ipynb` | Explanations, embedded inputs, analysis and verification in notebook form |
| `reproduce.py` | Standalone version of the analysis with embedded inputs |
| `domains/` | Four component catalogues, prerequisite relations, surmise matrices, and all 50 knowledge states with their outer fringes |
| `domains/domains_and_structures.md` | Readable description of the four domains and prerequisite graphs |
| `reproduced_results/` | Six CSV result tables, response-level metrics, and `verification.json` |
| `CITATION.cff` | Authors, ORCIDs and citation metadata for this supplement |
| `LICENSE` | MIT license for code |
| `LICENSE-CONTENT` | CC BY 4.0 notice for data and documentation |

## Scope and verification

The embedded data contain **2,400 recommendation sets** and **four prompt examples**. The analysis reconstructs knowledge spaces and outer fringes, scores recommendations, computes condition contrasts, and checks presentation agreement and terminal states.

Six result tables and the overall, presentation-agreement and terminal-state statistics are compared with embedded reference results from the archived analysis (absolute tolerance: `1e-12`). Figure data are exported; PDF figures are not rendered.

Full model-response texts and collection metadata remain in the study archive and are not part of this repository. The original API collection and response-schema validation are not repeated. The internal build scripts and source manifest are not distributed here and are not required to run this supplement.

## Citation

Steiner, P., & Hochweber, J. (2026). *Benchmarking LLM Next-Step Recommendations with Knowledge Space Theory: Reproducible supplement* (Version 1.0.0). https://github.com/pstnr/Benchmarking-LLM-Next-Step-Recommendations-with-Knowledge-Space-Theory

Machine-readable citation metadata are provided in [CITATION.cff](CITATION.cff). This citation identifies the supplement; the manuscript citation will be added once its publication identifier is available.

## Funding

The work on this chapter was funded by the SNSF, grant number 100019_219884.

## License

Code is licensed under the [MIT License](LICENSE). Data and documentation are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE-CONTENT).

For the mixed-content script and notebook, MIT applies to executable analysis code; CC BY 4.0 applies to embedded datasets, explanatory text, tables and outputs. See the license files for the precise scope. These licenses cover this supplement and do not set the license of the manuscript.
