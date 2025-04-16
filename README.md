# U.S. Hospital Quality Dashboard

This project analyzes publicly available data from the Centers for Medicare & Medicaid Services (CMS) to explore how hospital ownership, type, and location affect overall hospital ratings across the United States.

## Dashboard Overview

The final Tableau dashboard includes:
- Average hospital rating by ownership type
- Rating comparison by hospital type
- State-level map of average hospital scores
- Interactive filters by state and ownership

(DASHBOARD)

## Tools Used

- Python (pandas) for data cleaning and preparation
- Jupyter Notebook for exploring and organizing the data
- Tableau Public for creating the final visual dashboard

## Files

- `notebooks/cms_hospital_analysis.ipynb` – Notebook used to clean and analyze the dataset
- `Data/hospital_quality_dashboard.csv` – Cleaned dataset used in Tableau
- `.gitignore` – Added to prevent large files from being pushed to GitHub

## What I Learned

This was my first time cleaning real-world healthcare data and creating a dashboard with Tableau. I learned how to:
- Use pandas to explore and clean a large dataset
- Narrow down the data to only the most useful columns
- Handle missing values and convert text-based columns into numeric ones
- Export a cleaned CSV that could be used in a visualization tool like Tableau
- Build a multi-sheet dashboard with filters, maps, and comparison charts

## Challenges

- I accidentally tried to push a file that was too large for GitHub, which caused multiple errors and blocked my push.
- I wasn’t sure how to organize a Tableau dashboard layout at first, so it looked messy and confusing.
- I didn’t know how to show filters like "State" or "Hospital Ownership" across all my Tableau sheets.

## Fixes and Workarounds

- I added a `.gitignore` file to stop Git from tracking the large CSV file
- I used `git rm --cached` and a Git history cleanup to permanently remove the file from the project history
- I rearranged my Tableau sheets using vertical containers and resized the charts to create a cleaner layout
- I used “Apply to all using this data source” in Tableau to make my filters apply across every sheet

## Key Questions Explored

- Which hospital ownership types receive the highest average ratings?
- How do hospital types (e.g., acute care vs. critical access) compare in quality?
- Are there noticeable geographic patterns in hospital performance across states?

## How to Use This Project

### To View the Dashboard:
1. Go to the Tableau Public link listed above.
2. Use the filters at the top (like state or ownership) to explore the data.
3. Hover over bars, states, or table rows to see more details.

### To Run the Notebook:
1. Download or clone this repository.
2. Open `cms_hospital_analysis.ipynb` using Jupyter Notebook or VS Code with the Jupyter extension.
3. Make sure `pandas` is installed in your Python environment.
4. Run the notebook from top to bottom to see how the dataset was cleaned and exported for Tableau.

### Dataset Used:
- File: `Data/Hospital General Information.csv` (from CMS website)
- Cleaned version saved as `hospital_quality_dashboard.csv`

### Note:
The file `cms_hospital_patient_satisfaction_2020.csv` was too large for GitHub, so it was excluded. It is not required to run this version of the project.
