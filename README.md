# Supplementary analysis

*Benchmarking LLM Next-Step Recommendations with Knowledge Space Theory*  
Manuscript: 29 September 2026.

Python 3.10+ (tested: 3.12.10); standard library only.

Run all cells in `KST_Reproducible_Companion.ipynb`, or execute:

```sh
python reproduce.py
```

Inputs are embedded. Results are written to `reproduced_results`; subsequent runs overwrite these outputs.

The analysis includes knowledge spaces, outer fringes, response-level metrics, condition contrasts, presentation agreement and terminal states. Six result tables and the overall statistics are checked against the archived analysis. Figure data are exported; PDF figures are not rendered.

The embedded data contain 2,400 recommendation sets and four prompt examples. Full response texts and collection metadata remain in the study archive. Model calls and the original schema validation are not repeated.

`source_manifest.json` records source-file SHA-256 checksums. `build_supplement.py` rebuilds the notebook and script from the original repository.

`domains/domains_and_structures.md` contains all four component catalogues and prerequisite graphs. The same content is included in the notebook. `domains/` also includes the source CSV/JSON files, surmise matrices and all 50 knowledge states with their outer fringes.
