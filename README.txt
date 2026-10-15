NUTRITION DEFICIENCY ANALYSIS USING LOCAL HEALTH SURVEY DATA
TYDS Mini Project | Python Flask + SQLite + Chart.js

FEATURES
- Home page with project overview and sample statistics
- Survey page with nutrition habit questions
- Basic rule-based Low / Medium / High risk screening
- Dashboard with bar chart, pie chart, age chart and key indicators
- User access and Admin access
- Admin can view/delete recent survey records, upload CSV and export all data
- Automatically creates 500 synthetic sample survey records on first run

IMPORTANT
- The 500 rows are fictional sample/demo data, not real people or medical findings.
- Risk score is only a simple educational screening demonstration. It cannot diagnose a nutrient deficiency.
- Do not upload identifiable personal health data unless you have permission and appropriate safeguards.
- Change the default passwords and SECRET_KEY before using beyond a local class demo.

REQUIREMENTS
Python 3.10+ recommended
VS Code
Internet connection for Chart.js charts (loaded from CDN)

RUN IN VS CODE (Windows)
1. Extract the ZIP to a folder.
2. Open VS Code -> File -> Open Folder -> select nutrition_deficiency_analysis.
3. Open Terminal -> New Terminal.
4. Create a virtual environment:
   py -m venv .venv
5. Activate it:
   .venv\Scripts\activate
6. Install packages:
   pip install -r requirements.txt
7. Run:
   python app.py
8. Open the URL shown in terminal, usually http://127.0.0.1:5000

DEMO LOGINS
Admin: username admin | password admin123
User:  username user  | password user123

PAGES
/          Home
/survey    Submit survey
/risk      Understand the risk score
/login     User/admin login
/dashboard Dashboard (login required)
/admin     Admin panel (admin only)
/logout    Logout

CSV IMPORT
Log in as admin -> Admin panel -> choose a CSV file -> Import CSV.
Column matching supports common labels, but CSV headers/options should be checked after importing.
Export uses Admin panel -> Export CSV.

DATABASE
nutrition.db is created automatically in the project folder. Delete it only when the app is stopped
and you want a fresh database with 500 new demo rows.
