# Flight Reservation System

## Overview
This is a C++ console-based Flight Reservation System that allows both administrators and passengers to manage flights and bookings. The system provides functionalities for flight management, passenger registration, seat booking, and reservation management.

## Features

### Admin Features
- Add new flights with details (flight ID, departure, arrival, time, seats, price)
- View all flight details
- View all passenger registrations
- View all booking reservations

### Passenger Features
- Create a new account with personal details
- Login to existing account
- View available flights
- Book seats on flights
- View personal details
- Cancel bookings (full or partial)

### Data Persistence
- All data (flights, passengers, bookings) is saved to text files
- Data is automatically loaded when the program starts

## How to Use

### Compilation
Compile the program using a C++ compiler (g++ recommended):
```
g++ flight.cpp -o flight
```

### Running the Program
Execute the compiled program:
```
./flight
```

### Admin Access
- Username: `mirza`
- Password: `mirza123`

### File Structure
- `flights.txt` - Stores flight data
- `passengers.txt` - Stores passenger data
- `bookings.txt` - Stores booking data

## Data Validation
The system includes robust input validation for:
- Flight IDs (alphanumeric, max 10 chars)
- Names (alphabetic only)
- Emails (standard email format)
- Phone numbers (exactly 11 digits)
- Passport numbers (6-9 alphanumeric chars)
- Passwords (exactly 8 digits)
- Dates (YYYY-MM-DD HH:MM format)

## Code Structure
The program uses linked lists to manage:
- Flights (`FlightNode` struct)
- Passengers (`passengerNode` struct)
- Bookings (`bookingNode` struct)

Key functions include:
- `addFlight()` - Add new flights
- `addPassenger()` - Register new passengers
- `bookSeat()` - Make new bookings
- `cancelBooking()` - Cancel reservations
- File I/O functions for data persistence

## Limitations
- Console-based interface (no GUI)
- Basic error handling
- Single admin account (hardcoded credentials)

## Future Enhancements
- Graphical user interface
- Enhanced search functionality
- Multiple admin accounts
- Payment gateway integration
- More detailed reporting

## Author
Mirza Abdullah

## License
This project is open-source and free to use.
