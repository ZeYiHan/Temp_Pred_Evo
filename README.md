# Temp_Pred_Evo

Summary:
Global warming is reshaping food webs globally. Rapid evolution has been proposed as a buffer against climate change, but how simultaneous shifts in biotic and abiotic environments may influence evolution, is unknown. Using experimental evolution and mathematical modeling in microbial food webs of prey algae and ciliate predators, we tested 1) how temperature affects prey evolution, and, 2) how the food-web context––i.e., predator identity, abundance, and competition among predators–– mediates prey evolutionary dynamics. We found that temperature alone does not drive prey evolution unless predators are present, and food-web context determines ensuing evolutionary dynamics. These seemingly complex evolutionary responses are predictable from the joint effects of temperature-dependent but predator-specific predation rates, and the emergence of temperature-dependent prey plasticity. We reveal that evolutionary outcomes under warming are shaped by the broader food web context of species, suggesting that the same species may exhibit different eco-evolutionary responses in different food webs under novel climates.

This repository has the following files:
- R project file: **clean_code_Temp_Pred_Evo.Rproj**
- Density data for protists studied: **All_protist_density.csv**
  - `Day` — Experimental day of sampling (integer; 0, 5, 10, 15).
  - `Day_f` — Experimental day as factor, mirrors Day (integer).
  - `Jar` — Individual replicate jar ID (integer).
  - `Block` — Experimental block assigned as a random effect in all mixed models (character; A, B).
  - `Temp` — Temperature treatment in °C (integer; 19, 22, 25).
  - `Temp_f` — Temperature treatment as factor, mirrors Temp (integer).
  - `Trt` — Predator treatment, including single-predator and competition pairs (character; Tetra, Glauc, P.cau, TetraP.cau, GlaucP.cau).
  - `Rep` — Replicate number within treatment (integer; 1–6).
  - `Species` — Protist species identity (character; Tetra, Glauc, P.cau).
  - `PredComp` — Whether a second predator competitor is present in the jar (character; No, Yes).
  - `Dens` — Population density in individuals per ml (numeric, continuous).
- Chlamydomonas reinhardtii data from flowcytometry, seperated into 3 files for uploading: **Chlamy_data_1.csv**, **Chlamy_data_2.csv**, **Chlamy_data_3.csv** are flow cytometry measurements for Chlamydomonas reinhardtii collected on experimental days 5, 10, and 15. In total 881,857 observations × 10 variables. **Chlamy_day0_data.csv** contains Day 0 (initial) flow cytometry data for *C. reinhardtii* from stock culture. All treatment starts from the same stock culture. Each row represents a single-cell flow cytometry measurement.
  - `FSC_H` — Forward scatter height (numeric, continuous); proxy for cell/clump size.
  - `FSC_A` — Forward scatter area (numeric, continuous); used with FSC_H to detect multicellular clumping.
  - `Day` — Experimental day of sampling (integer; 0, 5, 10, 15).
  - `Block` — Experimental block assigned as a random effect in all mixed models (character; A, B).
  - `Jar` — Individual replicate jar ID (integer).
  - `Rep` — Replicate number within treatment (integer; 1–6).
  - `Temp` — Temperature treatment in °C (integer; 19, 22, 25).
  - `Trt` — Predator treatment, including single-predator (Tetrahymena, Glaucoma, P. caudatum) and competition pairs (character; Control, Tetra, Glauc, P.cau, TetraP.cau, GlaucP.cau).
  - `PredComp` — Whether a second predator competitor is present in the jar (character; No, Yes).
  - `Strain` — C. reinhardtii strain identity, either the flagella-deficient mutant or the fluorescent wild type (character; VFL1-1, WT-mNG).
  
- R Code that reproduces all analyses presented in the main text and Appendix: Clean_code_Temp_Pred_Evo.qmd
- Rendered Quarto file in html format: Clean_code_Temp_Pred_Evo.html
- Mathematical model output for Figure 2a–b: **model_Control.csv**, **model_Glauc.csv**, **model_Pcaud.csv**, **model_Pcaud.csv**
- Supplementary materials on the swimming ability of C. reinhardtii WT and vfl1-1 mutant: **WT_10x_Appendix_V.mov**, **vfl1-1_10x_Appendix_V.mov**
