# 2016 POTUS US Primary Election Results 

### Data Description

- The 2016 US Election dataset contains several main files and folders.
  - primary_results.csv: main primary results file
  - state: state where the primary or caucus was held
  - state_abbreviation: two letter state abbreviation
  - county: county where the results come from
  - fips: FIPS county code
  - party: Democrat or Republican
  - candidate: name of the candidate
  - votes: number of votes the candidate received in the corresponding state and county (may be missing)
  - fraction_votes: fraction of votes the president received in the corresponding state, county, and primary

- Demographics:
  - county_facts.csv: demographic data on counties from US census
  - county_facts_dictionary.csv: description of the columns in county_facts
  - A complete description of the `county_facts` can be found [`here`](https://github.com/Tsmith5151/2016-US-Election-ML/blob/master/county_facts_dict.csv)

- SQL Database:
  - database.sqlite: SQLite database containing the primary_results, county_facts, and county_facts_dictionary tables with identical     data and schema

#### Libraries:
  - `Python 2.7`
  - `Pandas`
  - `Numpy`
  - `SQLITE3`
  - To run `SQLITE3` in the `ipython notebook`kernel, install sql magic for IPython:
     ```python pip install ipython-sql```
  - Examples how to use ipython-sql can be foud [`here`](https://github.com/catherinedevlin/ipython-sql)

``` python
%load_ext sql
%sql sqlite:///database.sqlite
```
