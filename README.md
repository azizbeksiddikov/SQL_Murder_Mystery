# SQL Murder Mystery Project

## Objective
The goal of this project was to solve a murder mystery using SQL queries to analyze the database, identify suspects, gather evidence, and uncover the true culprit behind the crime.

## Database Structure
Dataset source: https://www.kaggle.com/datasets/johnp47/sql-murder-mystery-database/data

Report on Findings: https://docs.google.com/document/d/1mNiXk7ZAr9jttkQ0xp64hBmyTke7L-0r_QSWMIv-RjY/edit?usp=sharing

The database contains the following tables:
1. `crime_scene_report`
2. `drivers_license`
3. `facebook_event_checkin`
4. `interview`
5. `get_fit_now_member`
6. `get_fit_now_check_in`
7. `solution`
8. `income`
9. `person`

## Key Steps and SQL Skills Demonstrated

### Initial Investigation
- Queried the `crime_scene_report` table to gather initial information about the crime, such as the date of the murder, location, and witness descriptions.

### Witness Statements
- Retrieved witness statements by querying the `interview` table based on the addresses and names provided in the initial report.
- First witness described a suspect with a gym bag and specific membership details.
- Second witness provided additional physical characteristics and vehicle details.

### Identifying Suspects
- Used the `get_fit_now_member` and `get_fit_now_check_in` tables to filter suspects based on gym membership and check-in details.
- Queried the `drivers_license` table to match physical descriptions and vehicle information.

### Narrowing Down Suspects
- Combined multiple criteria including gym membership, vehicle registration, and physical descriptions using `JOIN` and `WHERE` clauses to narrow down the list of suspects.
- Identified Jeremy Bowers as a prime suspect based on the evidence.

### Gathering Comprehensive Information
- Retrieved all related data for the suspect, including Facebook event check-ins and interview transcripts.
- Queried the `facebook_event_checkin` table to find event participation details.
- Queried the `income` table to assess financial status.

### Final Culprit Identification
- Interrogated the suspect's interview transcript to identify the mastermind behind the murder.
- Uncovered Miranda Priestly as the true villain behind the crime.
