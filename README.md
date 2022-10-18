# QSS20 slides and activities

This public repo has content for the Fall 2022 iteration of `QSS20: Modern Statistical Computing` at Dartmouth College. The main components are slides and associated Jupyter notebook-based activities to practice Python or other concepts. The sections and skills covered are as follows.

## Data wrangling and visualization

### Introduction to pandas for data wrangling
  - **Activity**: [00_pandas_datacleaning_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/00_pandas_datacleaning_blank.ipynb)
  - **Data**: DC crime reports in 2020
  - **Concepts covered**:
    - Aggregation using `groupby` and `agg`
    - Lambda functions within aggregation
    - Recoding variables using `np.where`
    - Recoding variables using `np.select`
    - Recoding variables using `map` and dictionary
  - **Slides**: [02_qss20_f22_pandas.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/02_qss20_f22_pandas.pdf)
  - **Solutions**: [00_pandas_datacleaning_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/00_pandas_datacleaning_solutions.ipynb)
  - **Responses to class questions**: [00_classquestions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/00_classquestions.ipynb)

### User-defined functions
  - **Activity**: [01_functions_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/01_functions_blank.ipynb)
  - **Data**: DC crime reports in 2020
  - **Concepts covered**:
    - user-defined function to find matches within a broader pool of data
    - using list comprehension to apply a function iteratively over list elements
  - **Slides**: [03_qss20_f22_userdefinedfunctions.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/03_qss20_f22_userdefinedfunctions.pdf)
  - **Solutions**: [02_loopsfunctions_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/02_loopsfunctions_solutions.ipynb)

### Visualization with `plotnine`
  - **Example code**: [02_plottingexamples_plotnine.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/02_plottingexamples_plotnine.ipynb)
  - **Data**: DC crime reports in 2020
  - **Concepts covered**:
    - Plotting using the `plotnine` wrapper for R's `ggplot2`
    - Types of plots covered: line graph; bar chart; facetted line; line grouped/colored by attribute


## Workflow tools

### Shell & git
  - **Slides**: [04_qss20_f22_workflow.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/04_qss20_f22_workflow.pdf)
  - **Concepts covered**:
    - Cloning and committing from git on command line (shell)
    - Manipulating files from command line

### LaTeX
  - **Activity**: [03_latex_output_examples_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/03_latex_output_examples_blank.ipynb)
  - **Concepts covered**:
    - LaTeX and Overleaf syntax and workflow
    - Exporting tables from pandas to LaTeX
  - **Slides**: [05_qss20_f22_latex.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/05_qss20_f22_latex.pdf)
  - **Solutions**: [03_latex_output_examples_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/03_latex_output_examples_solutions.ipynb)


## Merging (exact and fuzzy) and regular expressions

### Exact merging
  - **Activity**: [04_merging_exact_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/04_merging_exact_blank.ipynb)
  - **Data**: San Diego business tax certificate data; Census NAICS code data
  - **Concepts covered**:
    - Data cleaning such as extraneous rows/columns
    - Recasting join cols to allow join (e.g., converting `int` to character)
    - `pd.merge` and different types of exact joins using join keys
    - Post-merge diagnostics
  - **Slides**: [06_qss20_f22_mergingexact.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/06_qss20_f22_mergingexact.pdf)
  - **Solutions**: [04_merging_exact_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/04_merging_exact_solutions.ipynb)

### Regular expressions
 - **Activity**: [05_basicregex_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/05_basicregex_blank.ipynb)
 - **Data**: Food Research Action Center (FRAC) data on district and school's election of community eligibility provision (CEP) for Free or Reduced Price Lunch (FRPL)
   - **Concepts covered**: 
     - Pattern construction using `re` module
     - `re.sub` for replacement
     - `re.findall` 
     - `re.match` and how to work with match objects using `.group()`
     - Throughout, review of list comprehension 
  - **Slides**: [07_qss20_f22_regex.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/07_qss20_f22_regex.pdf)
  - **Example code**: [06_merging_fuzzy_codeexample.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/06_merging_fuzzy_codeexample.ipynb)
  - **Solutions for activity**: [05_basicregex_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/05_basicregex_solutions.ipynb)

### Probabilistic merging/linkage
  - **Activity**: [06_merging_fuzzy_activity_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/06_merging_fuzzy_activity_blank.ipynb)
  - **Data**: public SD business tax certificate data; public PPP loan data on large loans
  - **Concepts covered**:
    - Regex for string cleaning
    - String distance/similarity measures: edit distance, jaccard, jarowinkler
    - `recordlinkage` package and steps in fuzzy/probabilistic matching
  - **Slides**: [08_qss20_f22_fuzzymatching.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/08_qss20_f22_fuzzymatching.pdf)
  - **Example code**: [06_merging_fuzzy_codeexample.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/06_merging_fuzzy_codeexample.ipynb)
  - **Solutions for activity**: [06_merging_fuzzy_activity_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/06_merging_fuzzy_activity_solutions.ipynb)


## Text as data

### Introduction to text mining
  - **Activity**: [07_textasdata_partI_textmining.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/07_textasdata_partI_textmining.ipynb)
  - **Data**: simplified data from airbnb NYC listings. Stored in `public_data/airbnb_text.zip`
  - **Concepts covered**:
    - Scoring based on dictionary of words
    - Part of speech tagging using `nltk`
    - Named entity tagging using `spaCy`
    - Sentiment analysis using `VADER`
   - **Slides**: [09_qss20_f22_textasdata.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/09_qss20_f22_textasdata.pdf)
   - **Solutions**: [07_textasdata_partI_textmining_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/07_textasdata_partI_textmining_solutions.ipynb)

### Topic modeling
  - **Activity**: [07_textasdata_partII_topicmodeling.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/07_textasdata_partII_topicmodeling.ipynb)
  - **Data**: simplified airbnb listings
  - **Concepts covered**:
    - Using `sklearn` to create a unigram document-term matrix
    - LDA topic modeling using `gensim`
    - Visualizing topics 
    - Obtaining top words per topic using `gensim`
    - Obtaining document-level topic probabilities using `gensim`
  - **Slides**: [09_qss20_f22_textasdata.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/09_qss20_f22_textasdata.pdf)
  - **Solutions**: [07_textasdata_partII_topicmodeling_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/07_textasdata_partII_topicmodeling_solutions.ipynb)


## APIs

### Introduction to APIs: NAEP data explorer; Yelp API
  - **Activity**: [08_apis_partI_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/08_apis_partI_blank.ipynb)
  - **APIs**: NAEP data explorer; Yelp API
  - **Concepts covered**:
    - Writing a query
    - Using `requests` to execute a query and return a response
    - Processing a response
    - Yelp Fusion API business search and reviews endpoints
  - **Slides**: [10_qss20_f22_APIs.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/10_qss20_f22_APIs.pdf)

### Twitter API with `tweepy` wrapper
  - **Example code**: [08_apis_partII_twitter_examplecode.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/08_apis_partII_twitter_examplecode.ipynb)
  - **Concepts covered**:
    - Authenticating
    - searching for tweets based on hashtag using `search_recent_tweets` method
    - searching for attributes of users tweeting
    - extracting followers of an account using `get_users_followers` method
    - extracting tweets from a specific user using `get_users_tweets` method
  - **Slides**: [10_qss20_f22_APIs.pdf](https://github.com/jhaber-zz/QSS20_public/blob/main/slides/10_qss20_f22_APIs.pdf)
  - **Blank activity**: [08_apis_partII_twitter_blank.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/08_apis_partII_twitter_blank.ipynb)
  - **Activity solutions**: [08_apis_partII_twitter_solutions.ipynb](https://github.com/jhaber-zz/QSS20_public/blob/main/activities/solutions/08_apis_partII_twitter_solutions.ipynb)


(more to come throughout the quarter)
