# Hotel Reservation System ERD

## Overview

This repository contains the Entity-Relationship Diagram (ERD) for an extended hotel reservation system. The ERD defines the structure of the database, including entities, attributes, and relationships, to support the functionalities of the hotel reservation system.

## Entity Descriptions

1. **Guest:**
   - GuestID (PK)
   - FirstName
   - LastName
   - Email
   - Phone
   - Address

2. **Reservation:**
   - ReservationID (PK)
   - CheckInDate
   - CheckOutDate
   - NumOfAdults
   - NumOfChildren
   - SpecialRequests
   - EmployeeID (FK)

3. **Room:**
   - RoomID (PK)
   - RoomNumber
   - RoomType
   - RatePerNight
   - Capacity
   - Amenities
   - HotelID (FK)
   - RoomTypeID (FK)

4. **ReservationRoom:**
   - ReservationRoomID (PK)
   - ReservationID (FK)
   - RoomID (FK)
   - NumOfAdults
   - NumOfChildren

5. **Payment:**
   - PaymentID (PK)
   - ReservationID (FK)
   - Amount
   - PaymentDate
   - PaymentMethod
   - TransactionID

6. **Employee:**
   - EmployeeID (PK)
   - FirstName
   - LastName
   - Position
   - Email
   - Phone
   - HireDate

7. **Availability:**
   - AvailabilityID (PK)
   - RoomID (FK)
   - Date
   - IsAvailable
   - PriceModifier

8. **RoomType:**
   - RoomTypeID (PK)
   - TypeName
   - Description
   - MaxOccupancy
   - BaseRate

9. **CustomerProfile:**
   - CustomerProfileID (PK)
   - GuestID (FK)
   - MembershipLevel
   - LoyaltyPoints

...

## Relationships

1. **Guest-Reservation (1 to M):**
   - Guest.GuestID → Reservation.GuestID

2. ...

## Usage

- Clone the repository to your local machine.
- Open the ERD diagram using your preferred database modeling tool or viewer.

## Suggestions for Improvement

1. Consider breaking down the ReservationRoom entity into Reservation and ReservedRoom for clarity.
2. Clarify the relationships between Reservation, Room, and Hotel.
3. Review the Employee-Reservation relationship for alignment with business requirements.
4. Customize the ERD based on specific business rules and real-world scenarios.

## Contributors

- [Your Name]
- [Contributor 2 Name]
- [Contributor 3 Name]

## License

This project is licensed under the [License Name] - see the [LICENSE.md](LICENSE.md) file for details.
