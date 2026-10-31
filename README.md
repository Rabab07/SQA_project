# Unit Testing: Parking System Management

JUnit 5 unit tests for a Java Parking System Management application, written for the Software Quality Assurance course at United International University (UIU). The tests were written from the class documentation, and every test case is explained in the report.

## Team

| Student ID | Name |
| --- | --- |
| 011221227 | Rabab Bin Karim |
| 011221021 | Mahi Ahsan |
| 011221173 | Sadman Sakib Omi |
| 011221002 | Jakaria Alam Saimon |

## Project structure

```
.
├── test/
│   ├── BookingTest.java
│   ├── ParkingSlotTest.java
│   ├── ParkingSystemTest.java
│   ├── VehicleTest.java
│   └── WalletTest.java
└── 011221227_011221021_011221002_011221173_unit_test_report.md
```

## What is tested

| Test class | Class under test | Test cases |
| --- | --- | --- |
| `BookingTest` | `Booking` | 14 |
| `ParkingSlotTest` | `ParkingSlot` | 29 |
| `ParkingSystemTest` | `ParkingSystem` | 21 |
| `VehicleTest` | `Vehicle` | 13 |
| `WalletTest` | `Wallet` | 21 |

The report lists 98 test cases (TC-01 to TC-98). For each one it gives the method under test, why the test was written, the verdict and our observations.

## Results

- **89 passed, 9 failed**
- Failed cases: TC-13, TC-14, TC-26, TC-31, TC-34, TC-36, TC-42, TC-61, TC-62
- TC-13 shows a real defect: `completeBooking()` still works after `cancelBooking()`, which goes against the documented lifecycle (ACTIVE to COMPLETED, or ACTIVE to CANCELLED).
- The other failures and their causes are described in the report.

## How to run

The tests need the Parking System source classes (`Booking`, `ParkingSlot`, `ParkingSystem`, `Vehicle`, `Wallet` and the related enums), which come from the course and are not included in this repo.

1. Create a Java project (IntelliJ IDEA or any IDE) and add the source classes.
2. Copy the files from `test/` into the project's test folder.
3. Add JUnit 5 (`org.junit.jupiter`) as a dependency.
4. Run all tests in the test folder.

## Tools

Java, JUnit 5
