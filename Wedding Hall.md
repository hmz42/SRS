# Wedding Hall Reservation System Documentation

## Overview

This repository contains the documentation for the Wedding Hall Reservation System, detailing the entities, attributes, and relationships in the Entity-Relationship Diagram (ERD).

## Entity-Relationship Diagram (ERD) Mapping

### Entities and Attributes:

1. **Customer:**
   - Primary Key: CustomerID
   - Attributes: FirstName, LastName, Email, Phone, Address

2. **Reservation:**
   - Primary Key: ReservationID
   - Attributes: EventDate, StartTime, EndTime, NumOfGuests, SpecialRequests

3. **Hall:**
   - Primary Key: HallID
   - Attributes: HallName, Capacity, Amenities, BaseRate

4. **ReservationHall:**
   - Primary Key: ReservationHallID
   - Foreign Keys: ReservationID, HallID

5. **Payment:**
   - Primary Key: PaymentID
   - Foreign Keys: ReservationID
   - Attributes: Amount, PaymentDate, PaymentMethod, TransactionID

6. **Employee:**
   - Primary Key: EmployeeID
   - Attributes: FirstName, LastName, Position, Email, Phone

7. **Availability:**
   - Primary Key: AvailabilityID
   - Foreign Key: HallID
   - Attributes: Date, IsAvailable, PriceModifier

8. **CustomerProfile:**
   - Primary Key: CustomerProfileID
   - Foreign
