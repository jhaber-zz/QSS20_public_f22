# QSS20 slides and activities

This public repo has content for the Fall 2022 iteration of `QSS20: Modern Statistical Computing` at Dartmouth College. The main components are slides and associated Jupyter notebook-based activities to practice Python or other concepts. The sections and skills covered are as follows.

## Data wrangling, merging, and probabilistic linkage

- [00_pandas_datacleaning_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/00_pandas_datacleaning_blank.ipynb)
  - **Data**: DC crime reports in 2020
  - **Concepts covered**:
    - Aggregation using `groupby` and `agg`
    - Lambda functions within aggregation
    - Recoding variables using `np.where`
    - Recoding variables using `np.select`
    - Recoding variables using `map` and dictionary
  - **Slides**: [qss20_w22_unit2_pandas.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/w22_slides/qss20_w22_unit2_pandas.pdf)
  - **Solutions**: [00_pandas_datacleaning_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/00_pandas_datacleaning_solutions.ipynb)

- [01_example_plotting.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/01_example_plotting.ipynb)
  - **Data**: DC crime reports in 2020
  - **Concepts covered**:
    - Plotting using the `plotnine` wrapper for R's `ggplot2`
    - Types of plots covered: line graph; bar chart; facetted line; line grouped/colored by attribute


- [02_loopsfunctions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/02_loopsfunctions.ipynb)
  - **Data**: DC crime reports in 2020
  - **Concepts covered**:
    - `for loop` to find matches within a broader pool of data
    - user-defined function to find matches within a broader pool of data
    - using list comprehension to apply a function iteratively over list elements 
   -  **Slides**: [03_qss20_w22_unit3_loopvfunction.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/w22_slides/03_qss20_w22_unit3_loopvfunction.pdf)
   -  **Solutions**: [02_loopsfunctions_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/02_loopsfunctions_solutions.ipynb)


- [03_merging_exact_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/03_merging_exact_blank.ipynb)
  - **Data**: San Diego business tax certificate data; Census NAICS code data
  - **Concepts covered**:
    - Data cleaning such as extraneous rows/columns
    - Recasting join cols to allow join (e.g., converting `int` to character)
    - `pd.merge` and different types of exact joins using join keys
    - Post-merge diagnostics
   - **Slides**: [05_qss20_w22_unit5_mergingexact.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/w22_slides/05_qss20_w22_unit5_mergingexact.pdf)
   - **Solutions**: [03_merging_exact_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/03_merging_exact_solutions.ipynb)


- [04_basicregex_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/04_basicregex_blank.ipynb)
   - **Data**: Food Research Action Center (FRAC) data on district and school's election of community eligibility provision (CEP) for Free or Reduced Price Lunch (FRPL)
   - **Concepts covered**: 
     - Pattern construction using `re` module
     - `re.sub` for replacement
     - `re.findall` 
     - `re.match` and how to work with match objects using `.group()`
     - Throughout, review of list comprehension 
    - **Slides**: [06_qss20_w22_unit6_regex.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/w22_slides/06_qss20_w22_unit6_regex.pdf)
    - **Example code**: [05_merging_fuzzy_codeexample.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/05_merging_fuzzy_codeexample.ipynb)
  - **Solutions for activity**: [https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/04_basicregex_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/04_basicregex_solutions.ipynb)

- [05_merging_fuzzy_activity_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/05_merging_fuzzy_activity_blank.ipynb)
  - **Data**: public SD business tax certificate data; public PPP loan data on large loans
  - **Concepts covered**:
    - Regex for string cleaning
    - String distance/similarity measures: edit distance, jaccard, jarowinkler
    - `recordlinkage` package and steps in fuzzy/probabilistic matching
  - **Slides**: [07_qss20_w22_unit7_fuzzymatching.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/w22_slides/07_qss20_w22_unit7_fuzzymatching.pdf)
  - **Example code**: [05_merging_fuzzy_codeexample.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/05_merging_fuzzy_codeexample.ipynb)
  - **Solutions for activity**: [05_merging_fuzzy_activity_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/w22_activities/solutions/05_merging_fuzzy_activity_solutions.ipynb)

(more to come throughout the quarter)
