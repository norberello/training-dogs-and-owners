ReadMe file
Created on 2020-08-30 by Jeffrey R. Stevens (jeffrey.r.stevens@gmail.com)
Finalized on 2020-11-21

**********************************************************
If you use the data, please cite the following:
Stevens, J.R., Wolff, L.M., Bosworth, M., & Morstad, J. (2020). Dog and owner characteristics predict training success. PsyArXiv. https://doi.org/10.31234/osf.io/p4dc7
**********************************************************

Summary: We collected survey, behavioral, and hormonal data from 99 dog/owner pairs from the Prairie Skies Dog Training Canine Good Citizen classes from Jan 2018 − Oct 2019. We generated three data files: one for the primary survey, behavioral, and hormonal measures for each dog/owner pair, one with the survey item responses for calculating internal consistency reliability, and one with the behavioral data scores for calculating inter-rater reliability. For the primary analysis data file, each row represents all of a single participant's responses. For the survey item data file, each row represents a participant's responses to a particular survey. For the behavioral task data, each row represents a dog's responses for a single session.


License:
All materials presented here are released under the Creative Commons Attribution 4.0 International Public License (CC BY 4.0). You are free to:
    Share — copy and redistribute the material in any medium or format
    Adapt — remix, transform, and build upon the material for any purpose, even commercially.
Under the following terms:
    Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
    No additional restrictions — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.


Data files:
stevens_etal_data1.csv (primary behavioral, cognitive, and cortisol data set)
 id - Dog id number
 date - Date owner completed survey
 class - Obedience training class
 dog_age - Age of dog in years
 dog_sex - Sex of dog
 dog_neutered - Neuter status (neutered/spayed = Yes, intact = No)
 owner_gender - Gender of owner
 time_train_dog_weekly_num - Number of hours per week spent training
 dog_behavior_bennett_disobedient_score - Disobedience subscale of Bennett & Rohlf behavior scale
 dog_behavior_bennett_aggressive_score - Aggression subscale of Bennett & Rohlf behavior scale
 dog_behavior_bennett_nervous_score - Nervousness subscale of Bennett & Rohlf behavior scale
 dog_behavior_bennett_destructive_score - Destructiveness subscale of Bennett & Rohlf behavior scale
 dog_behavior_bennett_excitable_score - Excitability subscale of Bennett & Rohlf behavior scale
 dog_behavior_bennett_overall_score - Overall score of Bennett & Rohlf behavior scale
 dog_problematic_behaviors_hiby_score - Problematic behavior score of Hiby et al.
 dog_obedience_hiby_score - Obedience score of Hiby et al.
 dias_behavioral_regulation_score - Behavioral regulation subscale of DIAS from Wright et al.
 dias_aggression_score - Aggression subscale of DIAS from Wright et al.
 dias_responsiveness_score - Responsiveness subscale of DIAS from Wright et al.
 dias_overall_score - Overall score for DIAS from Wright et al.
 mdors_score - Monash Dog Owner Relationship Scale score
 personality_extraversion_score - Extraversion score from brief Big-Five personality scale Gosling et al.
 personality_agreeableness_score - Agreeableness score from brief Big-Five personality scale Gosling et al.
 personality_conscientiousness_score - Conscientiousness score from brief Big-Five personality scale Gosling et al.
 personality_stability_score - Stability score from brief Big-Five personality scale Gosling et al.
 personality_openness_score - Openness score from brief Big-Five personality scale Gosling et al.
 lotr_score - Life Orientation Test Revised score from Scheier et al.
 pss_score - Perceived Stress Scale score from Cohen et al.
 crt_score - Cognitive Reflection Task score from Frederick
 numeracy_score - Berlin Numeracy Test score from Cokely et al.
 latency_sit_mean - Mean latency between command and sit behavior (in seconds)
 latency_down_mean - Mean latency between command and down behavior (in seconds)
 cort1 - Cortisol levels before first class meeting (in ug/dL)
 cort2 - Cortisol levels after first class meeting (in ug/dL)
 cort3 - Cortisol levels before last class meeting (in ug/dL)
 cort4 - Cortisol levels after last class meeting (in ug/dL)
 cgc_test - Success in completing Canine Good Citizen test (Pass/Fail)

stevens_etal_data2.csv (item-specific data for calculating internal consistency reliability)
 survey - name of survey
 item_1 - item_13 - individual items (surveys differ on number of items, so NAs represent no items)

stevens_etal_data3.csv (behavioral (sit/down) data for calculating inter-rater reliability)
 block - Replication block (1, 2, or 3)
 coder - Coder ID
 date - Date of behavioral data collection
 id - Dog ID
 latency_sit - Latency between command and sit behavior (in seconds)
 latency_down - Latency between command and down behavior (in seconds)


R code:
 stevens_etal_2020_rcode.R - code for running computations and generating figures


R Markdown documents:
 stevens_etal_2020.Rmd - R Markdown document with R code embedded for main manuscript
 stevens_etal_2020_SM.Rmd - R Markdown document with R code embedded for supplementary materials


Instructions to reproduce results:
 To reproduce these results, first unzip stevens_etal_2020_rr.zip into a folder.  Then, ensure that a subfolder named "figures" is in the folder with all other files.  Next, open stevens_etal_2020_rcode.R and ensure that all packages mentioned at the top of the script are installed.  Once all packages are installed, run the script in R using "source("stevens_etal_2020_rcode.R")".

 Once the script runs without errors, you can compile the R Markdown document stevens_etal_2020.Rmd.  Open this file in RStudio and ensure that you have packages 'knitr' and 'rmarkdown' installed.  Once installed, use knitr to compile the document (control-shift-k).  Use the same process to compile stevens_etal_2020_SM.Rmd.
 
