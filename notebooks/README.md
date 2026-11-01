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

## 3. Assistance Declaration:
For this assignment, my main source of assistance was W3schools
https://www.w3schools.com/python/numpy/default.asp
https://www.w3schools.com/python/pandas/default.asp
https://www.w3schools.com/python/python_ml_getting_started.asp

I also found GeeksForGeeks an incredibly helpful source for learning model building using scikit
https://www.geeksforgeeks.org/machine-learning/learning-model-building-scikit-learn-python-machine-learning-library/

These sources were used to help me build the league to binary mapping function:
https://www.codebegun.com/learn/data-analytics/data-cleaning/standardizing-text-data
https://towardsdatascience.com/5-methods-for-filtering-strings-with-python-pandas-ebe4746dcc74/
https://stackoverflow.com/questions/39724182/pandas-and-apply-function-to-match-a-string
https://stackoverflow.com/questions/11350770/filter-pandas-dataframe-by-substring-criteria
https://stackoverflow.com/questions/67228468/pandas-dataframe-column-value-conversion-from-string-to-binary

AI usage was in the form of google search AI overview. When writing up the setup instrictions, I googled `windows vs linux unzip .zip file`. Google outputted an AI overview as well as normal search results which I used to get the unzip command for Windows.

Sources for Milestone 3:
https://www.reddit.com/r/MLQuestions/comments/s36g2q/how_to_choose_a_machine_learning_model/
https://scikit-learn.org/stable/machine_learning_map.html
