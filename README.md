<div align="center">

![ucl-banner-land-black-rgb-2](https://user-images.githubusercontent.com/128257431/231888788-6d0e133b-edf5-4b0e-aaac-2d332f867deb.gif)

# UCL Project Metagenomics
</div>

Undergraduate research project in metagenomics

> ⚠️ **Disclaimer:** This project was completed during my undergraduate degree and may contain mistakes as my scripting skills were just at beginner level.

In this Git repository, the files used and figures produced for the Advanced Research Project in Metagenomics for BIOC0023 course at UCL (3rd-year module) are stored.

## Repository Structure

- Code for this project is available as `.ipynb` file (`Andrej_QIIME2_PE_ENA.ipynb`)
- The code for R, along with all the generated data and figures produced for this paper, is in: `Code_Files_Figures`

## Project Information

- QIIME2 pipeline for clustering and data processing
- Visualization in R Studio code

### Project Summary

This study investigated gut microbiome differences between Parkinson's disease (PD) patients and control subjects, as well as changes over time. Significant differences were found in gut microbiome composition between PD and control groups, supporting the existence of a correlation between Parkinson's and certain microbiome changes. No significant differences were observed between the original samples and samples taken two years later, suggesting that microbiome changes could be slow or initiated by a single triggering event. Future research should focus on longitudinal studies, alternative approaches like animal models, and refining study designs to better understand the relationship between the gut microbiome and PD.

### Workflow

1. Collection of fecal samples from PD patients and control subjects at two time points, baseline and 2 years later.
2. DNA extraction and 16S rRNA gene sequencing to analyze gut microbiome composition.
3. Comparison of alpha and beta diversity, using Jaccard distance and Bray-Curtis dissimilarity, to assess differences between PD and control groups.
4. Analysis of phyla abundance, including the twelve most abundant phyla, Actinobacteria, and Verrucomicrobia.
5. Examination of potential links between gut microbiome changes and Parkinson's disease, with suggestions for future research directions.

<div align="center">
<b>Graphical Abstract</b>
</div>

<div align="center">
<img width="790" alt="Screenshot 2023-04-13 at 22 09 35" src="https://user-images.githubusercontent.com/128257431/231883530-128099b4-4698-4753-ada3-4afd0bb8299c.png">
</div>




<div align="center">
Figures
</div>

<details>
<summary>Phyla abundance in control and PD groups</summary>
<br>

*Overall, the figure serves to highlight the differences in phyla abundance between control and PD groups, pointing to potential targets for future research, diagnostic markers, or therapeutic interventions.
*The figure presents a comparison of the relative abundance of bacterial phyla in the gut microbiomes of control and PD groups.
*Parts A, B, and C each focus on different aspects of phyla abundance:

### A. The twelve most abundant phyla:

<p align="center">
  https://user-images.githubusercontent.com/128257431/231890316-d0760f39-3a0f-4da0-b4bd-0778f33518f9.png
</p>

This part of the figure showcases the twelve most abundant bacterial phyla found in both control and PD groups.
The data is presented in a bar chart format, with the x-axis representing the phyla and the y-axis representing the relative abundance levels.
Differences in the relative abundance of specific phyla between control and PD groups can be observed, providing insights into the potential association between gut microbiome composition and Parkinson's disease.

### B. Abundance of Actinobacteria in control and PD groups:

<p align="center">
  https://user-images.githubusercontent.com/128257431/231890492-605580c2-f95e-4fe0-81a2-46974ce26df4.png
</p>

This part of the figure focuses on the abundance of the Actinobacteria phylum in control and PD groups.
A bar chart is used to visualize the data, with the x-axis representing the two groups (control and PD) and the y-axis representing the abundance levels.
A comparison of the abundance levels of Actinobacteria between control and PD groups may help identify its potential role in the disease.

### C. Abundance of Verrucomicrobia in control and PD groups:

<p align="center">
  https://user-images.githubusercontent.com/128257431/231890680-a30d3f42-3abf-497c-9f93-b347cc1466fc.png)
</p>

This part of the figure examines the abundance of the Verrucomicrobia phylum in control and PD groups.
The data is presented in a bar chart, with the x-axis representing the two groups (control and PD) and the y-axis representing the abundance levels.
Comparing the abundance levels of Verrucomicrobia between control and PD groups may provide insights into its possible involvement in Parkinson's disease.

</details>


<details>
<summary> Quality Control of Sequencing Data </summary>

This figure displays the quality control of the sequencing data obtained from the samples in the study. Proper quality control is essential for obtaining accurate and reliable results in microbiome research.

The figure presents a visualization of the distribution of sequence quality scores across the length of the sequenced reads. The x-axis represents the position in the read, and the y-axis represents the quality score.

A higher quality score indicates a lower probability of error in the base call. The quality scores are color-coded to provide a clear understanding of the overall quality of the sequencing data. This information is crucial for ensuring the reliability of the data and the conclusions drawn from it.
<p align="center">
  <img src="https://github.com/Andrej-Hric/UCL_Project_Metagenomics/blob/main/Code_Files_Figures/fig1.png" alt="Quality Control Figure">
</p>


</details>

<details>
<summary> Alpha Diversity in Control and PD Groups </summary>

This figure showcases the alpha diversity of the gut microbiomes in control and PD groups. Alpha diversity is a measure of the diversity within individual microbial communities and is commonly used to compare the richness and evenness of microbial populations.

The data is visualized using box plots, with the x-axis representing the two groups (control and PD) and the y-axis representing the alpha diversity values. Each box plot provides information on the median, quartiles, and potential outliers of the alpha diversity values for each group.

By comparing the alpha diversity between control and PD groups, the figure helps to identify potential differences in the richness and evenness of the gut microbiomes between the two groups. This information may provide insights into the association between gut microbiome composition and Parkinson's disease.

<p align="center">
  <img src="https://github.com/Andrej-Hric/UCL_Project_Metagenomics/blob/main/Code_Files_Figures/AlphaDiv.png" alt="Alpha Diversity Figure">
</p>

</details>






<details>
<summary> Beta Diversity in Control and PD Groups </summary>


This figure illustrates the beta diversity comparison between control and PD groups, providing insights into the differences in gut microbiome composition between the two groups.

The data is visualized using a scatter plot where each point represents an individual's gut microbiome. Points are colored according to their group affiliation (control or PD), enabling a clear distinction between the two groups.

The x-axis and y-axis represent the principal coordinates (PCoA) derived from the Jaccard distance and Bray-Curtis dissimilarity matrices, respectively. These two metrics are employed to measure the dissimilarity between microbial communities:

- **Jaccard distance**: This metric measures the dissimilarity between two sets by comparing the presence or absence of taxa. The Jaccard distance ranges from 0 to 1, with 0 indicating complete similarity and 1 indicating complete dissimilarity between the two sets.
- **Bray-Curtis dissimilarity**: This metric takes into account both the presence or absence of taxa and their relative abundance. The Bray-Curtis dissimilarity also ranges from 0 to 1, with 0 indicating complete similarity and 1 indicating complete dissimilarity between the two sets.

By comparing the distribution of control and PD groups within the scatter plot, the figure highlights the significant differences in beta diversity between the two groups. This observation suggests that Parkinson's disease is correlated with changes in the gut microbiome composition.

<p align="center">
  <img src="https://github.com/Andrej-Hric/UCL_Project_Metagenomics/blob/main/Code_Files_Figures/BetaDiv.png" alt="Beta Diversity Figure">
</p>


</details>



