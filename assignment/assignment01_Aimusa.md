Assignment 1
============


Instruction
-----------

Use the information from the lecture, the WTCCC’s genome-wide association study
paper: [https://www.nature.com/articles/nature05911](https://www.nature.com/articles/nature05911) to answer the following questions. **Please also provide the specific location of the information in the
paper, such as the section and page number.**

 
Submission
----------

-   Due Date: 23-Jan-2019

 
Questions
---------

1.  What type of study design was used in this study?
Case-control study (from abstract)

2.  What is the inclusion and exclusion criteria of the study population? Choose
    two diseases mentioned in the paper and provide the detail of inclusion &
    exclusion criteria.
    ## The study population 
    (from Samples and experimental analyses; page 661-2 and Supplementary Table 4 Exclusion summary by collection; page 31)
- Inclusion criteria
    1.  Living within England, Scotland and Wales (Great Britain) and 
    2. The vast majority had self-identified themselves as white Europeans
- Exclusion criteria
    1. SNP call rate < 97% (missingness) or
    2. Heterozygosity > 30% or < 23% across all SNPs or
    3. External discordance with genotype or phenotype data or
    4. Individuals identified as having recent non-European ancestry by the Multidimensional Scaling analysis or
    5. Duplicates (the copy with more missing data was removed) or
    6. Individuals with too much IBS sharing (>86%); likely relatives 
    ### Coronary Artery Disease
    (from Methods CAD phenotype description in Methods)
    - CAD cases had a validated history of either myocardial infarction or coronary revascularization (coronary artery bypass surgery or percutaneous coronary angioplasty) before their 66th birthday. 
    - Verification of the history of CAD was required either from hospital records or the primary care physician. 
    - Recruitment was carried out on a national basis in the UK through a direct approach to the public via (1) the media and (2) mailing all general practices (family physicians) with information about the study, as previously described. 
    -   Only one subject from each family was included in the present study.
    ### Hypertension 
    (from Methods HT phenotype description)
    - HT cases comprised severely hypertensive probands ascertained from families with multiplex affected sibships or as parent???offspring trios. They were of white British ancestry (up to level of grand-parents) and were recruited from the Medical Research Council General Practice Framework and other primary care practices in the UK. 
    - Inclusion criteria: Each case had a history of hypertension diagnosed before 60 years of age, with confirmed blood pressure recordings corresponding to seated levels 150/100 mmHg (if based on one reading), or the mean of 3 readings greater than 145/95 mmHg. 
    - Excluded criteria: Self-reportedly consumed 21 units of alcohol per week and diabetes, intrinsic renal disease, have a history of secondary hypertension or co-existing illness.

3.  Was the age distribution of each disease group comparable to the age
    distribution of the control groups?

    1.  What statistical test can you use to compare the age distribution
        between the two groups?
        - Normal distribution: Student t-test
        - Abnormal distribution: Wilcoxon???s rank sum test (Mann-Withney U test)

    2.  Which disease groups had significantly different age of distribution
        than controls? Also provide the statistical evidence for the comparison.
    
        Since the study does not reveal p-value to compare difference of age distribution between case and control but from Supplementary Table 1, we can assume trends of age distributions and disease which had significantly different age of distribution than controls is T1D.

    3.  Pick 1 disease with different age distribution between patients and
        control group. Discuss how the different in age distribution might
        affect the results of genetic association.

        When try to plot graph of age distribution from data table 1 in supplementary. We can observe graph of T1D which different age distribution between case and control because age distribution in case have a tendency in age range <40 years old while control have a tendency in age range 40-49 years old.
        
4.  Besides age, were there any other confounding factor(s) in the design of
    this study?
	- Sex because in some disease such as CAD, we found this disease in male more than female. Therefore, if the study include male more than female, it may be found patients who has CAD more than expected.
	- Demographic because genetic isolation may be happened in some region. 
	- Life styles or environments such as smoking or alcohol use, medication history, exercise, diet because all of this can be risk factors to develop diseases.

5.  What is the approach that we might be able to control those confounding
    factors?
    
    We can control confounding factors from these methods include
	- Randomization balances both measured and unmeasured characteristics
	- Stratification involves dividing the study population into strata, and then weighing and combining the stratum-specific results.
	- Matching to evaluate the effect of treatment by comparing the treated and non-treated units.
	- Restriction
	In the study, using sex-differentiated test which is sensitive to associations of a different magnitude and/or direction in the two sexes.

6.  For the strongest association signal for coronary artery disease,

    1.  what is the location of this SNP?
        - Chromosome 9p21.3. The strongest signal is seen at rs1333049 (P = 1.8 x 10^-14), associations are seen for SNPs across > 100 kilobases. The region of interest contains the coding sequences of genes for two cyclin dependent kinase inhibitors, CDKN2A (encoding p16INK4a) and CDKN2B (p15INK4b).
    2.  Is there a gene nearby?
        - The gene nearby is MTAP which encodes methylthioadenosine phosphorylase, an enzyme that contributes to polyamine metabolism and is important for the salvage of both adenine and methionine.
    3.  Was the SNP known or has any biological mechanism to affect the gene
        function?
        - CDKN2A and CDKN2B have multiple isoforms, have an important role in the regulation of the cell cycle and are widely expressed, with CDKN2B known to be expressed in the macrophages but not the smooth muscle cells of fibrofatty lesions45. It is of interest that expression of CDKN2B is induced by transforming growth factor beta (TGF-) and that the TGF- signaling system is implicated in the pathogenesis of human atherosclerosis.
    4.  Is it biologically plausible that we found this SNP associated with CAD?
         - Yes, because this gene regulates expression of cofactor in pathway that can causes CAD.
