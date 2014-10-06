---
title: "5 Process and Analysis"
---

Once the raw data are collected, the processing and analyzing phase of a longitudinal study forms the heart of the data work. This work is often internal to the project and usually precedes public dissemination or subsequent research with the data. The inputs often consist of raw data collected in Step 4, but can also include other forms of data that are linked, merged, or otherwise used to process, analyze, or improve the data at the core of the project.

5.1 INTEGRATE DATA

This step may involve joining data from parallel collection streams as well as joining collected data with external data. Joining data may involve transformations to harmonize data with different units of measurement or classification and coding schemes. Different streams of data may have been collected at different levels in a hierarchy of units of analysis – e.g., for households and for persons in households. Preserving software code used to integrate data is an important part of documenting the data.

5.2 CLASSIFY & CODE

Some data may need classification and coding. Open-ended questions, for example, may need to be processed by trained coders. Training may need to begin before production data are available. Supervision of coding may need to be set up. A study may involve qualitative data analysis techniques coding audio or video. Automated techniques such as text mining may be applied to classify chosen units of analysis. These actions may result in new variables (see 5.5 below). Parameter settings used to perform automated processing should be documented.

5.3 EXPLORE, VALIDATE AND CLEAN DATA

Almost all data will have some degree of error. Statistical and visualization techniques may be employed to search for problems. These activities can also generate measures of data quality, which should be documented.

5.4 IMPUTE MISSING DATA

Data collection projects almost universally experience instances of missing data or data that are inconsistent, logically impossible, or are otherwise in need of improvement. To overcome this limitation, various methods of data imputation are often used. In brief, data imputation involves the creation of data based on a set of rules that are clearly specified and intended to produce results that are scientifically valid. The creation of an entirely synthetic dataset may be viewed as an extreme form of data imputation, in that all the records in a completely synthetic dataset are imputed.

An exploration of the reasons for missing data can be crucial. If the occurrence of missing values relates to some aspect of the study or subjects, interpretation of an analysis may be impossible.

The methods used for imputation are described in DDI as GenerateInstructions, which are referenced from the variable using the ImputationReference element. If imputation methods change across the waves of a study, this would be documented in the comparison of the variables (see Ionescu et al. 2010).

5.5 CONSTRUCT NEW VARIABLES AND UNITS

Transformations may be applied to combinations of variables to produce new variables, as in the computation of scales, or the computation of a BMI score from weight and height. Classification and coding (see step 5.2) may have generated new variables. Some variables may need to be transformed to different units of measurement, or perhaps transformed to fit a different distribution.

For certain types of data, automated procedures may construct new variables. Pairwise distance measures, for example, can be processed by a multidimensional scaling program to produce spatial dimension variables. Parameters used in such procedures should be documented. New units of analysis may need to be generated. Transcripts for persons might need to be transformed to make paragraphs or sentences the unit of measurement for some text mining techniques.

5.6 CALCULATE WEIGHTS

In order for statistics to accurately reflect each universe measured, one or more weights may need to be calculated for observations.

5.7 CALCULATE AGGREGATES

Aggregate measures, e.g., counts, mean, median, low, high, and so on, may be calculated across combinations of classification variables. Sets of aggregates and associated classification variables may be output as data cubes. Where there are confidentiality constraints with the data, care may need to be taken to not produce aggregates which can reveal data about individual observations, for example the one person over 100 years old in a particular geographic unit.

5.8 ANONYMIZE DATA

Anonymization is a complex process potentially involving legal issues which vary across political boundaries. Techniques may involve removing or recoding variables deemed to be personal identifiers (government-issued ID numbers, specific geographic location, etc.). Other computational techniques may involve suppressing data in cells with small counts in data cubes (see step 5.7). Statistical techniques which may add noise to the data may be employed to prevent disclosure (see, for example, Eurostat, Statistical Disclosure Control).

Different sets of data may be produced at different levels of anonymization, each having different access policies.

5.9 FINALIZE DATA OUTPUTS

Data outputs may need to be transformed from the form convenient to the tools used for the steps above to forms appropriate for distribution. Some analysts may need the raw or cleaned raw data. Others may be able to use data with just direct identifiers removed. Public datasets may have more thorough anonymization applied. Summary datasets or graphics may be produced for publication. Data and metadata may have been maintained in a relational database for processing and analysis and need to be exported into more open formats for distribution, a DDI XML file, for example. Plans may also be made to make data available through an online service, or through the Semantic Web (see the Wikipedia article “Linked data”).

