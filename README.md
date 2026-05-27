# Temp_Pred_Evo

Summary:
Global warming is reshaping food webs globally. Rapid evolution has been proposed as a buffer against climate change, but how simultaneous shifts in biotic and abiotic environments may influence evolution, is unknown. Using experimental evolution and mathematical modeling in microbial food webs of prey algae and ciliate predators, we tested 1) how temperature affects prey evolution, and, 2) how the food-web context––i.e., predator identity, abundance, and competition among predators–– mediates prey evolutionary dynamics. We found that temperature alone does not drive prey evolution unless predators are present, and food-web context determines ensuing evolutionary dynamics. These seemingly complex evolutionary responses are predictable from the joint effects of temperature-dependent but predator-specific predation rates, and the emergence of temperature-dependent prey plasticity. We reveal that evolutionary outcomes under warming are shaped by the broader food web context of species, suggesting that the same species may exhibit different eco-evolutionary responses in different food webs under novel climates.

This repository has the following files:

- Density data for protists studied: **Protist_density.csv**
- Chlamydomonas reinhardtii data from flowcytometry: Chlamy_data_1.csv, Chlamy_data_2.csv, Chlamy_data_3.csv. Flow cytometry measurements for Chlamydomonas reinhardtii collected on experimental days 5, 10, and 15. Each row represents a single-cell measurement. 881,857 observations × 11 variables.
  - `FSC_H` — Forward scatter height (numeric, continuous); proxy for cell/clump size.
  - `FSC_A` — Forward scatter area (numeric, continuous); used with FSC_H to detect multicellular clumping.
        - `Day` — Experimental day of sampling (integer; 5, 10, 15).
        - `Block` — Experimental block assigned as a random effect in all mixed models (character; A, B).
        - `Jar` — Individual replicate jar ID (integer; 1–96).
        - `Rep` — Replicate number within treatment (integer; 1–6).
        - `Temp` — Temperature treatment in °C (integer; 19, 22, 25).
        - `Trt` — Predator treatment, including single-predator (Tetrahymena, Glaucoma, P. caudatum) and competition pairs (character; Control, Tetra, Glauc, P.cau, TetraP.cau, GlaucP.cau).
        - `PredComp` — Whether a second predator competitor is present in the jar (character; No, Yes).
        - `Strain` — C. reinhardtii strain identity, either the flagella-deficient mutant or the fluorescent wild type (character; VFL1-1, WT-mNG).
- Chlamydomonas reinhardtii data from flowcytometry: Chlamy_day0_data_submission.csv
- R Code that reproduces all analyses presented in the main text and Appendix: Clean_Code_Temp_Pred_Evo.R
- Supplementary materials on the swimming ability of C. reinhardtii WT and vfl1-1 mutant: WT_10x_Appendix_V.mov, vfl1-1_10x_Appendix_V.mov
