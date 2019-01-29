Assignment 1
============

 

Instruction
-----------

Use the information from the lecture, the WTCCC’s genome-wide association study
paper: \<https://www.nature.com/articles/nature05911 \>to answer the following
questions. **Please also provide the specific location of the information in the
paper, such as the section and page number.**

 

Submission
----------

-   Due Date: 23-Jan-2019

 

Questions
---------

1.  What type of study design was used in this study?

> case-control study

2.  What is the inclusion and exclusion criteria of the study population? Choose
    two diseases mentioned in the paper and provide the detail of inclusion &
    exclusion criteria.

_From the online method section_

  **BD inclusion criteria** 
    1. Age > 16
    2. living in mainland UK and of European descent
    3. Have a lifetime diagnosis of a bipolar mood disorder according to Research Diagnostic Criteria

  **CAD inclusion criteria**
    1.had a validated history of either myocardial infarction or coronary revascularization (coronary artery bypass surgery or percutaneous coronary angioplasty) 
    2. Developed the CVD event in (1) before their 66th birthday

  **CD inclusion criteria** 
    1. attendees at inflammatory bowel disease clinics in and around the five centres which contributed samples to the WTCCC (Cambridge, Oxford, London, Newcastle, Edinburgh)
    2. Have a confirmed diagnosis of Crohn’s disease (CD) using conventional endoscopic, radiological and histopathological criteria
  
3.  Was the age distribution of each disease group comparable to the age distribution of the control groups?

    1.  What statistical test can you use to compare the age distribution between the two groups?

    > To compare the age distribution between two groups, we can use Chi-square test or Fisher exact test if the number of counts tends to be lower than 5 per cell. 

    2.  Which disease groups had significantly different age of distribution than controls? Also provide the statistical evidence for the comparison.
        
        **From the supplementary table 1 in supplementary information** 
                
        Group    |     UKBS (Chi-Sq)     |     58C (Fisher Exact) |
        ---------|:---------------------:|:----------------------:|
        BD       | 0.220                 | 1
        CAD      | 0.220                 | 1
        HT       | 0.220                 | 1
        RA       | 0.241                 | 1
        T1D      | 0.265                 | 0.4
        T2D      | 0.220                 | 1

3.  Pick 1 disease with different age distribution between patients and control group. Discuss how the different in age distribution might affect the results of genetic association.

> Fortunately, none of the disease had statistically different age distribution compared to the control. If the age is associated with the disease status, and the controls were younger than cases, these controls might develop the disease later on. Therefore, we would have misclassified some cases as controls, and we would have introduced the misclassification bias in our study. This would lessen the effect estimates of the genetic markers that we have tested for association toward the null (OR =1). 
However, as age is not associated with the genotype, although age might be associated with the case-control status, our association results will not be confounded by age.

4.  Besides age, were there any other confounding factor(s) in the design of this study?

> For genetic association study, the most common confounding factor is population substructure (also called population stratification). See the discussion in "Geographical variation and population structure" of the main text. 

5.  What is the approach that we might be able to control those confounding factors?

> We can control for the population substructure by choosing controls with similar ancestry to the cases. For example, sampling the same ethnic group or from similar geographical region. Addition control for population substructure can be done by adjusting for the population structure during the analysis. However, if the cases and controls are drastically different, adjusting for the popopulation substructure may not correct all effects of confounding.

6.  For the strongest association signal for coronary artery disease,

    1.  what is the location of this SNP?
    
    >    rs1333049 is located on chromosome 9p21 between 21.93 - 22.12 Mb region
    
    2.  Is there a gene nearby?
    
    >From [dbSNP](https://www.ncbi.nlm.nih.gov/snp/rs1333049#seq_hash), zoom out to 30% and add the gene track to mini browser, you can see _CDKN2BAS_ as the closest annotated gene 5\' of this SNP.
    
    3.  Was the SNP known or has any biological mechanism to affect the gene function?
    
    > There was no clinical singificant of the SNP reported. Prior to 2007, there was no publication mentioned this variant. However, after 2007, several papers have identified this variants associated with several cardiovascular disease and metabolic traits.
    
    4.  Is it biologically plausible that we found this SNP associated with CAD?
    
    >It was not obvious how _CDKN2BAS_ might cause coronary artery disease. Hence, one might argue that there was no biological basis for the association of this variant and coronary artery disease. However, with amounting evidence replicating the association results of this variant and coronary artery disease. The association should be real and not mearly a false positive association found by chance.