# DAX Measures — Starter Templates

Adjust table names to match your Power BI model.

## Passenger count
The supplied solution labels `DISTINCTCOUNT(FlightID)` as total passengers, but this counts distinct flights. For a passenger-ID count, consider:

```DAX
Total Passengers =
DISTINCTCOUNT ( Passenger_Information[PassengerID] )
```

## Tickets booked
```DAX
Total_Ticket_Booked =
COUNT ( Ticket_Information[TicketID] )
```

## Condition column
```DAX
Customer_Condition =
IF (
    CONTAINSSTRING ( Flight_Information[Status], "On Time" ),
    "Best",
    "To Be Improved"
)
```

## Best flights
```DAX
Best Flights =
CALCULATE (
    DISTINCTCOUNT ( Flight_Information[FlightID] ),
    Flight_Information[Customer_Condition] = "Best"
)
```

Validate table and column names in Power BI before use.
