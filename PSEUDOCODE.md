# CAMPUS SMART PARKING SYSTEM

## PSEUDOCODE

### 1. Main Parking System

```text
START

Create ParkingFacility object

Create ParkingFeeCalculator object

Display the parking capacity of each floor

WHILE the system is running

    Display the menu:

        1. Park a Vehicle
        2. Exit a Vehicle
        3. View Available Parking Slots
        4. Calculate Parking Fee
        5. Exit System

    Read user choice

    IF choice = 1 THEN

        Read vehicle registration number
        Read vehicle type
        Read floor number
        Read slot number

        Validate vehicle and parking slot details

        Allocate the selected parking slot

        Generate and display parking ticket

    ELSE IF choice = 2 THEN

        Read vehicle registration number

        Search for the active parking ticket

        Calculate parking duration

        Calculate parking fee

        Release the occupied parking slot

        Close the parking ticket

    ELSE IF choice = 3 THEN

        Display available and occupied parking slots

    ELSE IF choice = 4 THEN

        Calculate and display the parking fee

    ELSE IF choice = 5 THEN

        Stop the parking system

    ELSE

        Display "Invalid choice"

    END IF

END WHILE

STOP
```

### 2. Vehicle Management

```text
START

Create an abstract class named Vehicle

Store the vehicle registration number

Define method getRegNo()

Define method getType()

Create the following subclasses:

    Car
    ElectricCar
    TwoWheeler
    EBike
    DeliveryVan

Override getType() in each subclass

Return the corresponding vehicle type

STOP
```

### 3. Parking Slot Allocation

```text
START

INPUT floorNumber

INPUT slotNumber

IF floorNumber is invalid THEN

    DISPLAY "Invalid floor number"

ELSE IF slotNumber is invalid THEN

    DISPLAY "Invalid slot number"

ELSE IF the selected slot is occupied THEN

    DISPLAY "Slot is already occupied"

ELSE

    Mark the selected slot as occupied

    DISPLAY "Vehicle parked successfully"

END IF

STOP
```

### 4. Parking Slot Release

```text
START

INPUT floorNumber

INPUT slotNumber

Validate the floor number and slot number

IF floor number and slot number are valid THEN

    Mark the selected parking slot as available

    DISPLAY "Parking slot released successfully"

ELSE

    DISPLAY "Invalid floor number or slot number"

END IF

STOP
```

### 5. Parking Fee Calculation

```text
START

INPUT vehicleType

INPUT parkingMinutes

INPUT entryTime

INPUT visitorPass

IF visitorPass = TRUE THEN

    fee = 100

ELSE IF vehicleType = EBike THEN

    fee = 20

ELSE

    hours = CEILING(parkingMinutes / 60)

    IF vehicleType = TwoWheeler THEN

        rate = 10

    ELSE IF vehicleType = Car THEN

        rate = 30

    ELSE IF vehicleType = ElectricCar THEN

        rate = 40

    ELSE IF vehicleType = DeliveryVan THEN

        IF entryTime is from 9 AM to before 5 PM THEN

            rate = 60

        ELSE

            rate = 30

        END IF

    END IF

    fee = hours * rate

END IF

DISPLAY "Total Parking Fee: ", fee

STOP
```

### 6. Five-Floor Parking Facility Design

```text
START

Create a parking facility with five floors

Assign parking capacities:

    Floor 1 = 2 slots
    Floor 2 = 3 slots
    Floor 3 = 1 slot
    Floor 4 = 4 slots
    Floor 5 = 2 slots

Display the parking capacity of each floor

Allow vehicles to be allocated to valid parking slots

Allow occupied parking slots to be released

STOP
```

## RESULT

The pseudocode successfully describes the major operations of the Campus Smart Parking System, including vehicle management, parking slot allocation, parking slot release, parking fee calculation, and five-floor parking facility management.

**Implementation note:** The original fee-calculation logic does not specify a rate for an unrecognized vehicle type. Add vehicle-type validation when implementing the pseudocode in Java.
