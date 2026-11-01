# Milestone 2: Using Psychological Factors to Predict League of Legends Player Rank
 
**Student ID:** 23392966  
**GitHub Repository:** [https://github.com/lilian-kennedy/CT4101-Machine-Learning-Project](https://github.com/lilian-kennedy/CT4101-Machine-Learning-Project)

---

## 1. Project Structure
```text
├── data/
│   └── GamingStudy_data.csv    # Raw dataset (not tracked if restricted by licence)
├── notebooks/
│   └── milestone2_baseline.ipynb  # Milestone 2 Notebook
├── README.md                   # Project overview & instructions
└── requirements.txt            # Package dependencies
```

---

## 2. Setup & Run Instructions
Unzip the Submission File
```
# Windows cmdlet
Expand-Archive -Path "C:\path\to\file.zip" -DestinationPath "C:\path\to\destination"

# Unix-Based System
unzip filename.zip -d /path/to/destination
```

Enter directory of folder
```
cd -d /path/to/destination

```

Create Virtual Environment
```
# Unix Based system
python3 -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
.\venv\Scripts\activate
```

Download the dependencies
```
pip install -r requirements.txt
```

Run the NoteBook
```
jupyter notebook
```

In Notebook, select kernel and click "Run All"

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

NEED TO FIX:
Some user responses contain multi rank data ("Diamond 3 last season, placements currently")
Current function will only see "diamond" and will treat it as a high rank.
What if user input contains both past and present rank?

Data-preprocessing clean up:
1. create target var
2. clean data
3. drop unused cols

Data Split Plan:
Everything except LeagueBinary x=feature
target y = League_Binary
prolly do clasic 80/20
Will need to statify since classes are not balanced (58:42)
Absolute baseline will be DummyClassifier as planned in last checkpoint

What model?
reddit comment: https://www.reddit.com/r/MLQuestions/comments/s36g2q/how_to_choose_a_machine_learning_model/
```
You want to start by defining the problem. Is it regression / classification / clustering? What kind of data do you have - all numerical, some categorical?

Then identify the metric you want to judge your model by, and just try out a few models and measure that metric. Generally, you'll find that a few models just do reasonably well straight away and some don't. Narrow down your search to the highest scoring models. They're likely the ones suited to your problem
```

Tabular data

https://scikit-learn.org/stable/machine_learning_map.html
SVG first?