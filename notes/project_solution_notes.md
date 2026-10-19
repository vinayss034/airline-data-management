# Project Solution Notes

Summary of the uploaded `docs/project_solution.pdf`.

## Task 1 — Data cleaning
Remove blank records, duplicates, and errors.

## Task 2 — Data modeling
Create relationships between the three tables using `FlightID`.

## Task 3 — Condition column
Create `Customer_Condition`: if `Status` contains `On Time`, show `Best`; otherwise show `To Be Improved`.

## Task 4 — Calculations
The solution lists:

```DAX
Total Passenger = DISTINCTCOUNT(ticket_information[FlightID])
```

```DAX
Total_Ticket_Booked = COUNT(ticket_information[TicketID])
```

It also requests filtering `Best` flights only.

**Metric check:** `DISTINCTCOUNT(FlightID)` counts distinct flights, not passenger IDs. Confirm the intended metric before reporting it as a passenger count.

## Task 5 — Visualizations
- Clustered bar chart: passenger count by airline.
- Pie chart: booking status and count by status.
- Stacked column chart: flights by destination.
- Slicers: Destination and Airline.

## Task 6 — Dashboard and Power BI Service
Create a dashboard, configure Row-Level Security for Airline A, and schedule refresh daily at 5 PM.

This summarizes the uploaded solution and does not confirm that these steps have been implemented in Power BI.
