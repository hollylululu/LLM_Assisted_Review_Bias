# 📘 LLM Assisted Review Bias

This repository supports research on **LLM-assisted literature review workflows**, with a focus on **evaluating potential bias** introduced during abstract screening and data extraction. It contains queries, search results, and downstream annotation outputs that can be used to analyze how large language models influence review decisions compared to traditional or human-only approaches.

---

## 📁 Repository Structure

```text
LLM_Assisted_Review_Bias/
├── Abstract_Screening_Results/
├── Data_Extraction_Results/
├── Query/
├── Search_Results/
├── Screening_Criteria/
└── README.md

```
## 📁 Directory Overview

### 1. Query/
Search queries used for retrieving literature from PubMed and Scopus. Query represented as a json dictionary. 

### 2. Search_Results/
1,172 articles in total.

Raw or processed search results corresponding to the queries, serving as inputs to screening and extraction steps.
- PubMed articles are uniquely identified by column: PMID
- Scopus articles are uniquely identified by column: EID

### 3. Abstract_Screening_Results/
161 articles in total.

Outputs from abstract screening tasks.

Articles' identifiers are embedded in column URL. Can retrieve the original PMID and EID from this colum. 

### 4. Screening_Criteria/
Inclusion and exclusion criteria used for human coders to screen the eligibility of the papers. Criteria is represented as json file, keys being "inclusion" and "exclusion", with criteria as lists. 

### 5. Data_Extraction_Results/
Results from structured data extraction tasks performed by human coders. 

## To-Do

### Data
- [ ] Extract PMID and EID from URL in Step 2. 
- [x] Add screening criteria as LLM prompts. 
- [ ] Add data extraction codebook as LLM prompts. 

### Analysis
- [ ] Preliminary LLM vs. human coder reliability for screening 
- [ ] Preliminary LLM vs. human coder reliability for data extraction


