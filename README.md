# FIFA World Cup 2026 Flight Travel Analysis

## Project Overview
This project analyses whether flight travel distance may have an impact on team performance during the FIFA World Cup 2026 group stage.

Because the tournament is hosted across the United States, Canada, and Mexico, teams may need to travel significant distances between match locations. This notebook calculates the flight distance between host cities and compares travel distance with match outcomes and group stage progression.

## Research Question
Does travel distance affect team performance in the FIFA World Cup 2026 group stage?

## Analysis Summary

The project investigates two main areas:

Individual match travel distance and match outcome
Compares travel distance before matches with whether teams won, lost, or drew.
Uses box plots and a Mann–Whitney U test.
Total group stage travel distance and tournament progression
Calculates each team’s total travel distance across the group stage.
Compares teams that advanced with teams that were knocked out.
Uses box plots, Q-Q plots, Welch’s t-test, and Cohen’s d effect size.

## Key Findings
Teams that won matches generally had a lower median travel distance than teams that lost or drew.
However, the difference was not statistically significant.
Total travel distance was also not significantly different between teams that advanced and teams that were knocked out.
Overall, the analysis suggests that flight travel distance alone was not meaningfully associated with group stage performance.

## Tools and Libraries Used
Python
Pandas
NumPy
Matplotlib
SciPy
KaggleHub
Jupyter Notebook

## Project Structure
FIFAWorldCup2026FlightTravel/
│
├── README.md
├── FIFAWorldCup2026FlightTravel.ipynb
├── requirements.txt
│
├── data/
│   └── host_cities.csv
│   ├── matches.csv
│   └── teams.csv
│
└── airports/
    └── airport_data.py

## How to Run This Project
Clone the repository:
git clone https://github.com/jonathanthk/FIFAWorldCup2026TravelTimeAnalysis.git

Open the project folder:
cd FIFAWorldCup2026TravelTimeAnalysis
Install the required libraries:
pip install -r requirements.txt

Open the notebook:
jupyter notebook FIFAWorldCup2026FlightTravel.ipynb
Run the cells from top to bottom.

## Notes and Assumptions
The analysis focuses only on group stage matches.
Travel distance is calculated using airport-to-airport flight distance.
Travel from airports to hotels or stadiums is not included.
The analysis assumes teams start at their first match location and finish at their final group stage match location.
Some placeholder playoff team names were manually replaced with teams that were drawn.

## Limitations
Flight distance does not fully capture travel fatigue.
Other factors such as squad quality, rest days, weather, injuries, and tactics are not included.
The analysis does not include time zone changes, airport waiting times, or ground transport.

## Conclusion
This project found no statistically significant evidence that flight travel distance had a meaningful impact on match outcomes or group stage progression. While travel may still affect teams in real-world conditions, this analysis suggests that distance alone is not a strong predictor of performance.
