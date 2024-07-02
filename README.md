# Analysis of the TED database 

This repository includes a reproducible methodology for analysing the content of the [Tenders Electronics Daily (TED)](https://ted.europa.eu/en/) database, based on one or more user-defined topics of interest. The TED database includes public tenders by EU and Member States institutions above certain economic thresholds.

![image](https://github.com/eurogeoss/TED-analysis/assets/14758434/9d1fb1d3-3b27-4920-b7a2-6b5db431e44f)

The Python notebook contains the code snippets necessary to perform the analysis. The input consists of:

1) Data Extract from TED: A dataset limited to 8,000 rows, as the repository does not allow files larger than 25 MB [b2g_es_award_notice_max5cpv.csv].
2) Keywords for Document Selection: A file containing the keywords used for selecting relevant documents [keywords_final.xlsx].
Additionally, the keywords file includes another sheet that specifies the rules for key aggregation and the questions for evaluation using the LLM algorithm.

