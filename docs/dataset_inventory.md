# Dataset Inventory

## Flight Information

- **Rows:** 200
- **Columns:** 5

| Column | Non-null | Missing | Data type |
|---|---:|---:|---|
| `FlightID` | 200 | 0 | `int64` |
| `FlightNumber` | 200 | 0 | `object` |
| `Airline` | 200 | 0 | `object` |
| `Destination` | 200 | 0 | `object` |
| `Status` | 200 | 0 | `object` |

## Passenger Information

- **Rows:** 100
- **Columns:** 3

| Column | Non-null | Missing | Data type |
|---|---:|---:|---|
| `PassengerID` | 100 | 0 | `int64` |
| `FlightID` | 100 | 0 | `int64` |
| `SeatNumber` | 100 | 0 | `object` |

## Ticket Information

- **Rows:** 50
- **Columns:** 3

| Column | Non-null | Missing | Data type |
|---|---:|---:|---|
| `TicketID` | 50 | 0 | `int64` |
| `FlightID` | 50 | 0 | `int64` |
| `BookingStatus` | 50 | 0 | `object` |

