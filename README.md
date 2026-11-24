# PierDesign

**A rigid pier analysis tool for lateral loading**

PierDesign is a free engineering software tool developed for the analysis and design of rigid pier foundations subjected to lateral loading. It is intended for structural, geotechnical, and transmission line engineers involved in foundation design.

The software implements a displacement-based approach to evaluate the interaction between a rigid pier and the surrounding soil, building upon the BH (Brinch Hansen) method recommended by AS/NZS 7000 and the theoretical recommendations in IEEE 691.

<p align="center">
  <img width="1709" height="1117" alt="image" src="https://github.com/user-attachments/assets/44d04b9f-108f-4323-95c4-221f4cf24f22" />
</p>
<p align="center">
  <em>Figure 1. Input Tab of PierDesign.</em>
</p>

## Key Features

### 1. Pier Displacement Analysis

Calculates the lateral displacements at the top and bottom of the pier under applied loading, based on a rigid-body rotation assumption about a point of rotation located below ground level.

### 2. Ultimate Soil Resistance – BH Method

Applies the BH method referenced in AS/NZS 7000 to determine the ultimate lateral soil resistance. This resistance represents the limiting soil capacity rather than the actual soil reaction mobilised under a given loading condition.

### 3. Mobilised Soil Resistance

Evaluates the mobilised soil resistance along the pier based on its displacement profile, accounting for the non-linear relationship between pier displacement and soil resistance.

### 4. Pier Internal Force Analysis

Calculates the shear force and bending moment distributions along the pier based on the mobilised soil resistance, rather than assuming that the ultimate soil resistance is fully mobilised.

### 5. Input and Output File Management

Save project input parameters and calculation results to a file for record keeping, and project archiving. Saved input files can be reopened to retrieve previously defined analysis parameters.

---

## Engineering Approach

Conventional application of the BH method primarily focuses on determining the ultimate lateral soil resistance. However, the ultimate resistance does not necessarily represent the actual soil reaction developed under the applied loading conditions (see soil pressures in Figure 2).

Assuming that the ultimate soil resistance is fully mobilised may result in an overestimation of the soil reaction, potentially leading to conservative estimates of pier shear forces and bending moments and uneconomical reinforcement design.

PierDesign adopts a displacement-based approach to address this limitation:

1. Determine the ultimate lateral soil resistance using the BH method.
2. Establish the pier displacement profile based on the rigid-body rotation assumption.
3. Evaluate the mobilised soil resistance based on the displacement-dependent soil response.
4. Calculate the resulting shear force and bending moment distributions along the pier.

The theoretical framework is based on the recommendations in IEEE 691, with the aim of providing a more realistic assessment of soil–pier interaction under lateral loading.

<p align="center">
  <img width="1709" height="1117" alt="image" src="https://github.com/user-attachments/assets/3ba0643e-35f9-4381-a83e-28e279c8c33b" />
</p>
<p align="center">
  <em>Figure 2. Result Tab of PierDesign.</em>
</p>

## Reference Standards

The engineering approach draws upon the following standards:

- **AS/NZS 7000** – Overhead line design, including the BH method for ultimate lateral soil resistance.
- **IEEE 691** – Guide for Transmission Structure Foundation Design and Testing.

Users should refer to the relevant standards and original publications for the applicable design provisions and assumptions.

---

## Download

PierDesign is available as a free Windows application.

**[Download the latest release](https://github.com/transstructx/PierDesign/releases/latest)**

1. Download the latest Windows release ZIP file.
2. Extract the ZIP file to a local folder.
3. Run `PierDesign.exe`.

The published Windows package is intended to be self-contained, so a separate .NET runtime installation should not be required.

---

## Intended Applications

PierDesign is intended for engineering applications involving rigid pier foundations subjected to lateral loading, particularly:

- Overhead transmission line foundations.
- Rigid pier foundation analysis.
- Assessment of soil–foundation interaction.
- Evaluation of lateral displacement and internal forces.

---

## Limitations and Disclaimer

PierDesign is an engineering calculation tool intended to assist qualified engineers with foundation analysis.

The results should be independently reviewed and verified by the responsible engineer before being used for engineering design or construction.

Users are responsible for confirming that the assumptions, soil parameters, loading conditions, and applicable design requirements are appropriate for each project.

The software does not replace professional engineering judgement or the requirements of applicable standards and project specifications.

---

## Feedback and Contributions

PierDesign is an independently developed engineering tool, and feedback from structural, geotechnical, and transmission line engineers is welcome.

Suggestions, bug reports, and technical discussions are encouraged through the GitHub repository.

If you find PierDesign useful, please consider giving the repository a ⭐ Star and sharing it with fellow engineers.

---

**Developed by:** TransStructX  
**Project:** PierDesign  
**License:** To be specified
