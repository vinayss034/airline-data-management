# Airline Data Management and Analysis Using Power BI

GitHub project folder for an airline analytics project using flight, passenger, and ticket data. Includes the uploaded project brief and solution PDF, source CSV files, solution-page images, dataset inventory, and starter DAX documentation.

## Objective
Analyze flight schedules, passenger details, and ticket bookings to support operational insights and passenger management.

## Repository structure
```text
airline-powerbi-github/
├── data/raw/                  # Original CSV datasets
├── data/processed/            # Cleaned/exported data
├── docs/                      # Project brief, solution, inventory
├── images/solution-pages/     # PNG images of the solution PDF
├── notes/                     # Solution summary
├── powerbi/                   # DAX templates and future .pbix report
├── screenshots/               # Add actual Power BI screenshots
├── report/                    # Add final PDF report
```

## Included datasets
- `flight_information.csv`
- `passenger_information.csv`
- `ticket_information.csv`

See [`docs/dataset_inventory.md`](docs/dataset_inventory.md) for columns, row counts, and missing-value counts.

## Tasks from the project brief and solution
1. Clean blank records, duplicates, errors, missing values, and column formats in Power Query.
2. Create relationships between the three tables using `FlightID`.
3. Create `Customer_Condition`: `Best` when `Status` contains `On Time`, otherwise `To Be Improved`; extract the flight number from `FlightNumber`.
4. Create DAX calculations for passenger counts, tickets booked, and filtering `Best` flights.
5. Create visuals for passenger count by airline, ticket booking status, and flights by airline/destination, with Destination and Airline slicers.
6. Create the final dashboard, configure Row-Level Security for Airline A, and schedule refresh daily at 5 PM where supported.
