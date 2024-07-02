# Analysis of the TED database 

This repository includes a reproducible methodology for analysing the content of the [Tenders Electronics Daily (TED)](https://ted.europa.eu/en/) database, based on one or more user-defined topics of interest. The TED database includes public tenders by EU and Member States institutions above certain economic thresholds.

![image](https://github.com/eurogeoss/TED-analysis/assets/14758434/9d1fb1d3-3b27-4920-b7a2-6b5db431e44f)

The Jupyter Notebook [TED_analysis.ipynb](https://github.com/eurogeoss/TED-analysis/blob/main/TED_analysis.ipynb) contains the code snippets necessary to perform the analysis. The input consists of:

1) **Data Extract from TED** ([TED_database.csv](https://github.com/eurogeoss/TED-analysis/blob/main/TED_database.csv)): a portion of the TED database for years 2021-2022 limited to 8,000 rows;
2) **Keywords for Document Selection** ([keywords_final.xlsx](https://github.com/eurogeoss/TED-analysis/blob/main/keywords_final.xlsx)): a file containing the keywords used for filtering relevant documents from the TED database; this file also includes another sheet that specifies the rules for keywords aggregation and the questions for evaluation using a Large Language Model.

How it works: from a list of relevant keywords and rules defined in the keywords file, we created a procedure that: 

* searches and extracts TED documents relevant to our topic of analysis (in this example, topics around open source geospatial software, open geospatial data and open geospatial standards); and 
* refines the search using a Large Language Model (LLM), in particular the nous-hermes-2-mixtral-8x7b-dpo algorithm available in the GPT@JRC platform.

This framework can be readily adapted and applied to other cases with similar objectives.

This work was presented at the [FOSS4G Europe 2024](https://2024.europe.foss4g.org/) conference happened in Tartu, Estonia on 1-7 July 2024; the presentation slides are available [here](https://talks.osgeo.org/foss4g-europe-2024/talk/MTEYTZ/).
