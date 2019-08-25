# poppit
The codes and data are for target estimation for protein/peptide drugs.

The basic principle: 
Target identification and validation is crucial during the process of drug research and development (R＆D). 
Besides the disease relevance, successful drug targets generally have some common features different from other non-target proteins. 
Systematic summary of the features of successful drug targets and further computationally estimating whether a protein is proper 
to be used as a drug target (i.e. target prediction) based on these features will greatly improve efficiency and success rate of 
target selection.
These codes are used for target estimation for protein/peptide drugs.
Briefly, the target predition model was constructed by naive Bayes classifier to integrate multiple features. 




Input: input.txt, protein list represented by SP_AC, one protein per line
Output: peptide_target_estimation_score.txt for peptide drugs' target estimation
				protein_target_estimation_score.txt for protein drugs' target estimation
				
How to use:
Please install ActivePerl version 5.16 or above in your windows or Linux system

Write your interested protein list into "input.txt" file 
Run the script "target_estimation_protein.pl" for protein drugs or "target_estimation_peptide.pl" for peptide drugs
Then the target estimation scores will be given in "peptide_target_estimation_score.txt"/"protein_target_estimation_score.txt"

The target estimation score is just the "combined_LR".
In the result file, known targets for protein/peptide drugs (i.e. target proteins of FDA-approved protein/peptide drugs) 
(represented by "golden" in the file) are always given on the top, followed by other proteins with predictd "combined_LR".



!The codes and data are for academics. For commercial use, please contact us!
If you use the related codes and data, Please cite our paper. 


Contact: liuzy1984@163.com (Zhongyang Liu, Beijing Proteome Research Center, Beijing, China)
2019.8.23
