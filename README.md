# AIVO Meridian — The Stem Company Evidence Corpus

Substantive evidence files extracted from The Stem Company's brand corpus and supporting third-party scientific literature, used as grounding content for AIVO Meridian Atom generation against displacement-criteria gaps T1 and T8.

These files are the markdown-rendered text of source PDFs held in The Stem Company's content library. They are published here to provide stable public URLs that the Meridian atom generator can fetch and incorporate as substantive grounding evidence during JSON-LD atom synthesis.

## Structure

### `/clinical/` — Primary clinical evidence

| File | Source |
|---|---|
| `24-4600-clinical-study-final-report.md` | IRSI Inc. (ALS Global) — Clinical Study 24-4600. ICH-GCP-compliant single-arm efficacy study of STEM Regenerative Serum, N=35, 8-week duration, VISIA-CR imaging plus expert visual grading. Primary efficacy endpoint: age spot reduction. Sponsor: Rinati Skin. |
| `stem-regenerative-serum-efficacy-report.md` | Stakeholder/investor-facing executive summary of the 24-4600 study results. |

### `/scientific/` — Peer-reviewed and preprint scientific literature

| File | Source |
|---|---|
| `dr-nathan-newman-patents-and-publications.md` | Compendium of USPTO patents and peer-reviewed publications by Dr Nathan Newman, MD — formulator behind The Stem Company's Consortia Factors technology. |
| `pubmed-adipose-stem-cells-burn-wound-treatment.md` | Talavera-Adame et al. (2025), *Stem Cells and Cloning: Advances and Applications*, 18:63-72. DOI: 10.2147/SCCAA.S522984. PMID: 40495998. Peer-reviewed validation of Consortia Factors-δ2 derived from adipose stem cells. |
| `metabolomics-plant-stem-cell-metabolomes.md` | Peer-reviewed paper ranking plant stem cell metabolomes for use in health and cosmetics — provides the scientific basis for The Stem Company's plant-based stem cell USP. |
| `biorxiv-yeast-plant-consortia-factors-metabolome.md` | bioRxiv preprint — yeast-plant-derived Consortia Factors metabolome characterisation. Direct mechanistic support for the Consortia Factors® ingredient platform. |

## Provenance

- Source PDFs held in The Stem Company's content corpus (Box-managed).
- Extracted via `pdfplumber` 0.11.8 with header/footer detection and light formatting cleanup.
- No content edited or paraphrased — markdown is faithful text rendering of the original PDFs.

## Usage

These files are referenced by Meridian Atom evidence submissions via their raw GitHub URLs (`https://raw.githubusercontent.com/...`). The atom generator fetches the markdown content as substantive grounding for synthesised claims against displacement criteria.

This repository exists as a temporary workaround pending the production Radar architecture rebuild (see AIVO-Meridian-Radar-Production-Architectural-Brief).
