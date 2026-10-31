Personal Notes:

When setting up the environment, needed to connect venv directly using excecutable path. Before submitting run on spare computer to check this isn't a common issue

highestleague has all null values, will drop
idk what story is with unnames:0? need to research. 
Solution: https://stackoverflow.com/questions/36519086/how-to-get-rid-of-unnamed-0-column-in-a-pandas-dataframe-read-in-from-csv-fil

Update: ...solution actually not relevant, that is for saving file to csv, not opening. Can just drop columns when doing cleaning
League and Degreee have some large gaps, prolly represent non-competitive gamers

Concerning to see 650 missing values for social phobia, but at least no blanks for anxiety and life satisfaction

total missing cells: 21709

Need to figure out how to deal with number gaps? Maybe impute? What about categorical gaps?
Will need to clean league, way to automate?
Research:
https://www.codebegun.com/learn/data-analytics/data-cleaning/standardizing-text-data
https://towardsdatascience.com/5-methods-for-filtering-strings-with-python-pandas-ebe4746dcc74/
https://stackoverflow.com/questions/39724182/pandas-and-apply-function-to-match-a-string
https://stackoverflow.com/questions/11350770/filter-pandas-dataframe-by-substring-criteria
https://stackoverflow.com/questions/67228468/pandas-dataframe-column-value-conversion-from-string-to-binary
