# CAMPUS SMART PARKING SYSTEM

# CONSOLIDATED TEST CASES

## 1. Basic Data Management and Parking Operations Tests

| Test ID | Test Description | Expected Result |
|---|---|---|
| TC01 | Store vehicle information | Vehicle details are stored successfully |
| TC02 | Create a parking slot | Parking slot is created successfully |
| TC03 | Allocate an available parking slot | Vehicle is parked successfully |
| TC04 | Release an occupied parking slot | Parking slot becomes available |
| TC05 | Attempt to allocate an occupied parking slot | System displays an appropriate slot-occupied message |
| TC06 | Enter an invalid parking slot number | System displays an invalid-slot error message |

## 2. Object-Oriented Programming (OOP) Tests

| Test ID | OOP Concept | Expected Result |
|---|---|---|
| TC07 | Constructor Overloading | Appropriate constructor is executed based on the supplied arguments |
| TC08 | Static Members | Shared static variables maintain common values across objects |
| TC09 | Inheritance | Subclass successfully accesses inherited members from its parent class |
| TC10 | Method Overriding | Subclass-specific method implementation is executed |
| TC11 | Encapsulation | Private data members are accessed through appropriate getter and setter methods |
| TC12 | Abstraction | Concrete subclasses provide implementations for required abstract methods |
| TC13 | Interface Implementation | Implementing classes provide definitions for all required interface methods |

## 3. Complete System Validation – Task 11

| Test ID | Test Description | Expected Result |
|---|---|---|
| TC14 | Park a valid car | Car is parked successfully |
| TC15 | Park a valid two-wheeler | Two-wheeler is parked successfully |
| TC16 | Exit a previously parked vehicle | Parking ticket is closed and the occupied slot is released |
| TC17 | Allocate the last available parking slot | Vehicle is accepted and allocated the remaining slot |
| TC18 | Calculate parking fee for zero minutes | Zero billable hours are calculated |
| TC19 | Calculate parking fee for exactly 60 minutes | One billable hour is calculated |
| TC20 | Calculate parking fee for 61 minutes | Two billable hours are calculated |
| TC21 | Enter an unsupported vehicle type | System rejects the vehicle type with an appropriate error message |
| TC22 | Enter a duplicate vehicle registration number | System rejects the duplicate registration number |
| TC23 | Enter an invalid parking slot number | System rejects the invalid slot selection |

## 4. Design Challenge Validation – Task 12

| Test ID | Test Description | Expected Result |
|---|---|---|
| TC24 | Calculate the parking fee for an E-Bike | Flat parking fee of Rs. 20 is applied |
| TC25 | Calculate the delivery van fee during 9 AM–5 PM for 2 hours | Total parking fee is Rs. 120 |
| TC26 | Calculate the delivery van fee after 5 PM for 2 hours | Total parking fee is Rs. 60 |
| TC27 | Calculate the visitor one-day pass fee | Fixed visitor pass fee of Rs. 100 is applied |
| TC28 | Display the five-floor parking facility | All five parking floors and their capacities are displayed |
| TC29 | Calculate the total parking capacity | Total capacity is displayed as 12 parking slots |
| TC30 | Allocate a parking slot on Floor 5 | Vehicle is successfully allocated to a valid slot |
| TC31 | Enter an invalid floor number | System rejects the invalid floor number with an appropriate error message |

## 5. Test Result Summary

The consolidated test cases provide comprehensive coverage of the following system functionalities:

1. **Basic Parking Operations:** Vehicle registration, parking slot creation, allocation, and release.
2. **Object-Oriented Programming:** Constructor overloading, static members, inheritance, method overriding, encapsulation, abstraction, and interface implementation.
3. **System Validation:** Vehicle parking, vehicle exit, registration number validation, and parking slot verification.
4. **Boundary Testing:** Zero-minute parking, exactly 60 minutes, and 61-minute parking duration calculations.
5. **Vehicle Categories and Pricing:** E-Bike flat fees, delivery van time-based charges, and visitor pass calculations.
6. **Five-Floor Parking Management:** Floor validation, individual floor capacity, and total parking capacity verification.

**Testing Instructions:**

- Execute each test case using the implemented Java program.
- Compare the actual program output with the corresponding expected result.
- Record the test status as PASS or FAIL based on the observed output.
- Capture relevant screenshots as evidence of successful test execution.
- Do not mark a test case as PASS without verifying its actual execution result.

## RESULT

The consolidated test plan establishes a structured approach for evaluating the Campus Smart Parking System. It covers basic parking operations, object-oriented programming principles, system validation, boundary conditions, vehicle-specific pricing rules, and the five-floor parking facility design. These test cases help verify the system's functionality, reliability, and compliance with the assignment requirements.
