# Hi, I'm dgun89 👋

Data scientist at a metabolomics research institute in Japan (Kazusa DNA Research Institute), working on **metabolomics** with data science and machine learning.

## Research focus

I work on the **reliability of chemical knowledge in databases and LLMs**, with two connected goals:

1. **Illuminating the dark metabolome** — annotating and classifying the large fraction of metabolites that remain unverified or unclassified in current databases.
2. **Grounding & identifier reliability** — cross-database identifier resolution is fragile (even with RAG) and degrades on long-tail metabolites (cf. MetaBench, Lu et al., 2025, arXiv:2510.14944). I study where LLM- and DB-based grounding breaks, working toward a **well-grounded multi-omics reference DB**.

An underexplored axis: gene–RNA data is abundant, but the **RNA–protein–enzyme** layer remains data- and DB-sparse.

## Projects

These three repositories form one pipeline — build a trustworthy DB, predict the unknowns, and stress-test the retrieval layer.

| Repo | What it does | Role in the story |
|------|--------------|-------------------|
| [metabolite-study](https://github.com/dgun89/metabolite-study) | Resolves chemical identifiers for human/mouse serum metabolites across PubChem, KEGG, HMDB, ChEBI, UniChem, COCONUT, BRENDA; rule-based endogenous/exogenous classification with enzyme mapping (~900 compounds). | **Foundation** — produces the reference DB and surfaces the *dark metabolome* (unverified compounds). |
| [DarkMet](https://github.com/dgun89/DarkMet) | Predicts endogenous vs. exogenous origin from SMILES alone (Random Forest + Morgan fingerprints, HMDB 5.0 labels, ROC-AUC 0.98). | **Illuminating the dark** — classifies the unverified compounds; also uncovered and conservatively corrected systematic label noise. |
| [lipidomics-ai-agent](https://github.com/dgun89/lipidomics-ai-agent) | Personal learning repo evolving RAG → GraphRAG (Neo4j) → tool-using agent. | **Reliability** — characterizes three failure modes (grounding failure, over-refusal, retrieval instability) and the LLM identifier-merging problem. |

## Skills

Python · Machine Learning · RAG / GraphRAG · LC-MS/MS metabolomics

Korean (native) · Japanese · English

📫 Reach me via GitHub