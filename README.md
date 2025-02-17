# EventMasterCpp

EventMasterCpp is a C++-based event management system that allows users to manage event bookings, guest details, and payments using Object-Oriented Programming (OOP) principles. This project provides functionalities such as event creation, booking, searching, checkout, and payment handling.

## Features
- **User Management**: Add, search, and manage users who book events.
- **Event Management**: Create, search, display, and delete event records.
- **Booking System**: Allows users to check in, book events, and manage reservations.
- **Payment Handling**: Handles event booking payments, including deposit transactions.
- **Guest Summary**: Displays event details, guest information, and booking statuses.

## Technologies Used
- **C++** (Object-Oriented Programming)
- **Standard Library Headers** (iostream, string, etc.)
- **Console-based User Interface**

## Class Structure

### 1. `User`
- Stores user details like name, address, phone number, and booking ID.

### 2. `Event`
- Stores event details including event number, venue, guest size, duration, and booking status.
- Key methods:
  - `addEvent(int ev)`: Adds a new event.
  - `searchEvent(int ev)`: Searches for an event by event number.
  - `displayEvent(Event)`: Displays event details.

### 3. `EventMen` (Derived from `Event`)
- Handles event bookings and guest management.
- Key methods:
  - `checkIn()`: Books an event for a user.
  - `getAvailEvent()`: Shows available events.
  - `searchUser(char *name)`: Searches for a user by name.
  - `checkOut(int EventNum)`: Handles event checkout, cost calculation, and payment.

### 4. `Account`
- Handles financial transactions.
- Key method:
  - `deposit(int num)`: Processes payments.

## How to Run
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/EventMasterCpp.git
   ```
2. Compile the code:
   ```sh
   g++ EventMasterCpp.cpp -o EventMasterCpp
   ```
3. Run the executable:
   ```sh
   ./EventMasterCpp
   ```

## Future Enhancements
- Implement a graphical user interface (GUI) for better user experience.
- Store event and user data persistently using a database.
- Add an admin panel for better event monitoring and control.


## Contributing
Contributions are welcome! Feel free to fork this repository and submit a pull request.

## Contact
For any issues or suggestions, reach out at [kaushikborah4080@gmail.com](mailto:kaushikborah4080@gmail.com).
