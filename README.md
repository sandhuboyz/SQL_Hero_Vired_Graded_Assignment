Here’s a comprehensive `README.md` guide for our **Hero Vired Graded SQL Assignment**. You can copy this into your repository or submission folder:

---

# Hero Vired Graded SQL Assignment

## 📝 Introduction

This project is a graded SQL assignment for Hero Vired's Data Science program. The task involves working with airline-related datasets stored across eight SQL schemas. The goal is to write and execute SQL queries to extract, analyse, and derive insights from the data, solving a total of 17 analytical problems.

## 📁 Table of Contents

* [Introduction](#-introduction)
* [Schemas](#-schemas)
* [Installation](#-installation)
* [Usage](#-usage)
* [Features](#-features)
* [SQL Questions Solved](#-sql-questions-solved)
* [Dependencies](#-dependencies)
* [Examples](#-examples)
* [Troubleshooting](#-troubleshooting)
* [Contributors](#-contributors)
* [License](#-license)

---

## 🗃 Schemas

The database is built using the following eight schema files, which should be executed in the listed order to maintain referential integrity:

1. `a. airlines_data_tickets.sql`
2. `b. airlines_data_aircrafts.sql`
3. `c. airlines_data_airports.sql`
4. `d. airlines_data_boarding_passes.sql`
5. `e. airlines_data_bookings.sql`
6. `f. airlines_data_flights.sql`
7. `g. airlines_data_seats.sql`
8. `h. airlines_data_ticket_flights.sql`

Each script sets up a part of the data infrastructure needed for running analysis queries.

---

## 🛠 Installation

1. Install MySQL or any compatible RDBMS.
2. Create a new database (e.g., `airlines_data`).
3. Execute the schema files in the order listed above.
4. Ensure all tables and relationships are properly created and populated.

---

## 🚀 Usage

Once the schemas are set up, the SQL queries can be executed using any SQL interface, like:

* **MySQL**

Each query answers a specific analytical question using data from the airline domain.

---

## ✨ Features

* Schema-driven relational database design.
* Complex SQL querying using aggregation, joins, and grouping.
* Revenue, passenger behaviour, aircraft usage, and airport traffic analysis.
* Time-series and trend analytics.

---

## 🧠 SQL Questions Solved

Below are the SQL queries written and executed as part of the assignment:

1. **Average Delay in Departures for Delayed Flights**
2. **Flights Grouped by Aircraft Usage Frequency**
3. **Total Revenue per Flight**
4. **Boarding Number Patterns per Flight**
5. **Occupancy Rate per Aircraft**
6. **Top 3 Revenue-Generating Flights**
7. **Average Flight Duration by Aircraft Model**
8. **Departure Flight Count per Airport**
9. **Arrival Flight Count per Airport**
10. **Daily Booking Trends**
11. **Frequent Route Analysis**
12. **Passenger Boarding Summary per Flight**
13. **Average Boarding Number per Flight**
14. **Total Spend per Passenger**
15. **Fare Condition Distribution**
16. **Revenue by Route**
17. **Peak Booking Hours**

---

## 📦 Dependencies

* MySQL (or compatible RDBMS)
* SQL client for executing queries
* The eight `.sql` files for schema creation and data population

---

## 🧪 Examples

Examples of queries used:

```sql
-- Average Delay in Departures for Delayed Flights
SELECT AVG(actual_departure - scheduled_departure) AS avg_delay
FROM flights
WHERE actual_departure > scheduled_departure;
```

```sql
-- Total Revenue per Flight
SELECT flight_id, SUM(amount) AS total_revenue
FROM ticket_flights
GROUP BY flight_id;
```

---

## 🛠 Troubleshooting

* **Foreign Key Errors**: Ensure SQL scripts are run in the correct order.
* **Missing Data**: Validate that all data insertions in `.sql` scripts execute successfully.
* **Time Format Issues**: Verify that the time and date columns are parsed correctly in your SQL engine.

---

## 👥 Contributors

* **\[Inderbir Singh]** – Author & Analyst

---

## 📄 License

This project is undertaken for academic purposes as part of the Hero Vired coursework. Redistribution or use for commercial purposes is not allowed without prior permission.

---

Let me know if you'd like me to also generate the SQL queries as a `.sql` file or include explanations for each question!
