# IPL-ball-by-ball-win-predictor
 ***IPL Ball-by-Ball Win Probability Predictor
** Project Overview

This project builds a Machine Learning model that predicts the probability of the batting team winning an IPL match at any ball of the game using historical ball-by-ball data.

**By analyzing match conditions such as:

a)current score

b)balls remaining

c)current run rate

the model estimates the real-time win probability of the batting team.

This project demonstrates how Data Science and Machine Learning can be applied to sports analytics.

*** Dataset

The project uses two IPL datasets.

1️)***Match Information Dataset (basic_info.csv)

Contains general match details such as:

a)Match ID

b)City

c)Toss decision

d)Winner

e)Player of the Match

2️)***Ball-by-Ball Dataset (ball_by_ball_ipl_data.csv)

Contains detailed information for every ball in every match:

a)Batter name

b)Bowler name

c)Runs scored

d)Batting team

e)Bowling team

f)Total runs on each delivery

These datasets were combined to build the final machine learning dataset.

*** Feature Engineering

New match situation features were created from the raw data:

a)current_score → Total runs scored so far

b)ball_number → Current ball in the innings

c)balls_left → Balls remaining in the innings

d)current_run_rate → Runs scored per over

e)runs_per_ball → Average runs scored per ball

These features help represent the current match situation.

*** Machine Learning Model

The project uses:

a)Logistic Regression (scikit-learn)

b)Steps followed:

c)Data loading

d)Data cleaning

e)Feature engineering

f)Train-test split

g)Model training

h)Model evaluation

*** Win probability prediction

The model predicts:

1 → Batting team wins

0 → Batting team loses

*** Model Performance

Model Accuracy:

~64%

While simple, the model demonstrates how machine learning can estimate win probability during a cricket match.

Future improvements could increase accuracy by adding more features.

*** Example Prediction

Example match situation:

-Current Score: 178
-Balls Remaining: 24
-Current Run Rate: 11

Predicted Output:

-Win Probability: 45.79%

This means the batting team has about a 45.79% chance of winning given the match situation.

*** Visualizations Included

The notebook also contains several visualizations:

📊 Top 10 IPL Run Scorers

📊 Distribution of Win Probabilities

📊 Win Probability vs Balls Remaining

These help understand scoring patterns and model predictions.

*** Technologies Used

a)Python

b)Pandas

c)NumPy

d)Matplotlib

e)Scikit-learn

f)Jupyter Notebook / Google Colab

*** Future Improvements

a)Possible extensions to this project:

b)Add second-innings chase prediction

c)Include wickets remaining

d)Train advanced models such as:

e)Random Forest

f)XGBoost

g)Build a live match probability dashboard

h)Develop an AI-based alternative to the DLS method for rain-interrupted matches



-Author

DEV SHARMA

-Student interested in: Artificial Intelligence, Data Science, Sports Analytics

📜 License

This project is open-source and intended for educational and learning purposes.
