The March Machine Learning Mania 2024 competition on Kaggle challenges participants to forecast outcomes of the NCAA Division 1 Men’s and Women’s basketball tournaments using historical data. Participants will submit a portfolio of up to 100,000 brackets for each tournament. The evaluation metric is the Average Brier Bracket Score, which measures the accuracy of probabilistic predictions for each round. Each team must follow valid tournament paths in the predictions. Submissions are made via Kaggle Notebooks and must adhere to specific runtime and data usage rules. The competition runs from February 27, 2024, to April 10, 2024, with $50,000 in prizes awarded to the top entries.


Project Overview:
Data Preparation:

Teams Data: Loaded and processed data related to NCAA basketball teams, including their IDs and win ratios for the latest season.
Tournament Slots: Loaded and filtered tournament slots for the latest season, identifying the structure of rounds and matchups.
Simulation Setup:

Seeds Data: Loaded and organized seed information for both men's and women's tournaments, which determines the initial matchups.
Simulation Functions: Defined functions to simulate matchups based on win ratios and determine winners for each slot in the tournament brackets.
Simulation Execution:

Run Simulation: Executed simulations for both men's and women's tournaments across multiple brackets (10,000 simulations per tournament).
Result Compilation: Compiled simulation results into a structured DataFrame (submission) containing columns for tournament type, bracket number, slot, and winning team.
Output:

CSV Export: Exported the final simulation results to a CSV file (submission.csv), which includes details of all simulated brackets for both men's and women's tournaments.
Results:
Output File (submission.csv):
Contains 1,260,000 rows (representing each simulated matchup result).
Columns include Tournament (M for Men's, W for Women's), Bracket (simulation number), Slot (specific tournament slot), and Team (winning team ID).
Conclusion:
The project successfully simulated the NCAA basketball tournament for both men's and women's brackets.
Each simulation (10,000 per bracket) provided a probabilistic outcome for each matchup based on team win ratios.
The CSV output (submission.csv) can be further analyzed or used for reporting and decision-making processes related to NCAA basketball tournaments.
This project demonstrates the use of data analysis and simulation techniques to predict tournament outcomes based on historical team performance metrics.
