# 📄 Conservation relevant fine-scale distribution and habitat associations of threatened elasmobranchs in temperate nearshore waters

Repository containing analysis code, data, and supplementary materials supporting the paper:


**Conservation relevant fine-scale distribution and habitat associations of threatened elasmobranchs in temperate nearshore waters**  
Hopkins, C.R., Cullen, G., Flatt, R.L., Brooker, E.E., Bailey, D.M., and Burns, N.M.  
Submitted to Aquatic Conservation: Marine and Freshwater Ecosystems

---

## 📑 Abstract

Elasmobranchs are globally threatened and experiencing ongoing declines. Understanding threatened elasmobranch distribution is critical for developing effective marine conservation strategies. However, our knowledge of fine scale elasmobranch habitat association and distribution in temperate nearshore systems is limited. Here, we examined the presence, relative abundance and habitat association of sharks, skates and rays using benthic baited remote underwater stereo-video systems (SBRUVs). From 772 deployments (682 total hours, 53 minutes average soak time) across three years (2021-2023) and two Scottish sea lochs and adjacent bays, elasmobranchs were detected on 31.2% of deployments (n = 241). Our surveys detected six species of elasmobranchs, flapper skate (<i>Dipturus intermedius</i>), thornback ray (<i>Raja clavata</i>), spotted ray (<i>Raja montagui</i>), lesser spotted dogfish (<i>Scyliorhinus canicula</i>), spiny dogfish (<i>Squalus acanthias</i>) and porbeagle (<i>Lamna nasus</i>) representing 17.6% of the resident elasmobranch diversity reported to date in UK nearshore waters < 200 m depth. The species detected include two species listed as globally Vulnerable on the IUCN Red List, spiny dogfish and porbeagle and one Critically Endangered species, flapper skate. Critically Endangered flapper skate were detected in 5.2% deployments (n = 40) and were the only species recorded which did not show a relationship between the probability of presence and substratum type. Our findings provide critical data on the fine scale spatial distribution and substrate associations of elasmobranchs, which could be used to inform evidence-based conservation measures and support more consistent and targeted policy action for these species in Scotland.

---

## 📂 Repository Structure

```
.
├── Data/                              # CSV data files for species presence (link supplied)
  └── GIS_Data                         # Sample location metadata, environmental covariates and files used for mapping (link supplied)
├── LICENSE 
├── README.md
└── Temperate_elasmobranchs.Rmd        # Master RMarkdown script for entire analysis workflow
```

---

## 📝 How to Reproduce the Analysis

### 1️⃣ Clone this repository:
```bash
git clone https://github.com/NeilMBurns/Temperate_Elasmobranchs.git
cd Temperate_Elasmobranchs
```

### 2️⃣ Install R dependencies:
From within R:
```R
install.packages(c("INLA", "sf", "terra", "RColorBrewer"))
```

Optionally use `renv` or `packrat` for environment management.

### 3️⃣ Open `Scotland_sharks.Rmd` in RStudio and run code chunks sequentially.

This script:
- Reads and prepares elasmobranch presence-absence data
- Converts to spatial objects
- Summarises descriptive statistics and species richness by location and year
- Loads environmental spatial layers
- Fits spatial Bayesian models via R-INLA (model-fitting code follows the loaded data)
- Produces figures of species distribution, habitat associations and model predictions

Data import and outputs will be saved to directories as selected by the user.

---

## 📊 Data Availability

Code and data used to generate this manuscript’s analyses are available at:  
👉 https://doi.org/10.6084/m9.figshare.30366148.v1
    DOI: 10.6084/m9.figshare.30366148

---

## 📄 License

- The code in this repository is released under the MIT License
  
  👉  https://github.com/NeilMBurns/Temperate_Elasmobranchs?tab=MIT-1-ov-file.
  
  You are free to use, share and adapt the materials, provided appropriate credit is given to the original authors.
---

## 📣 Citation

If you use these materials, please cite:

```
###place holder #####
Hopkins, C.R., Cullen, G., Flatt, R.L., Brooker, E.E., Bailey, D.M., Burns, N.M. (2025). Conservation Relevant Fine-Scale Distribution and Habitat Associations of Threatened Elasmobranchs in Temperate Nearshore Waters. Aquatic Conservation: Marine and Freshwater Ecosystems. [DOI to follow].
```

---

## 📬 Contact

For questions, data access, or collaboration enquiries:

- **Dr Neil M. Burns** — neil.burns@glasgow.ac.uk
- Or open an issue on this repository

---
