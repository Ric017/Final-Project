# Final-Project
# Parking Lot System - README

## Purpose:

This system simulates the management of a parking lot, including vehicle assignments, ticketing, payment processing, and administrative summaries.

## How to Run:

### 1. **Compile Java Files**:

Ensure all Java files in the project are compiled before running the system.

* **Using an IDE (NetBeans or other Java IDE):**

  * Open the project in the IDE, and it will automatically compile the files for you.

* **Using Command Line:**
  Navigate to the project's root directory and compile the Java files by running the following command:

  ```bash
  javac -d bin src/com/mycompany/parkinglotsystem/*.java
  ```

### 2. **Run the Main Class**:

To execute the system, run the `ParkingLotSystem.java` class.

* **Using NetBeans:**

  * Right-click on `ParkingLotSystem.java` and select **Run File**.

* **Using Command Line:**
  Navigate to the root directory of the project and run the following command:

  ```bash
  java -cp bin com.mycompany.parkinglotsystem.ParkingLotSystem
  ```

### 3. **Running Unit Tests**:

To run unit tests, ensure that JUnit (or another testing framework) is configured in your IDE. You can write tests for methods like vehicle assignments, payment processing, etc.

---

## Features:

1. **Assign Parking Spots**: Vehicles are assigned parking spots with vehicle ID and type.
2. **Track Entry and Exit Times**: The system records entry and exit times for each vehicle.
3. **Handle Payments**: Parking fees are calculated based on parking duration, and payment is processed when a vehicle exits.
4. **Admin Summary**: Provides an overview of the total revenue and average parking duration.
5. **Search for Vehicles**: Find a vehicle’s parking spot by its ID.

---

## Requirements:

* **Java JDK 8 or higher** is required.
* A **Java IDE** like NetBeans (or Eclipse) is recommended for easy development and testing.
* **JUnit** is required for running unit tests.

---

## Data Collection Script Instructions - README4.txt

This section provides instructions on how to run the data collection script for the Parking Lot Management System. The script simulates vehicle entries, exits, and logs parking lot data.

### Prerequisites:

Make sure the following are set up:

* **Java Development Kit (JDK)** is installed on your system.
* **NetBeans IDE** (or any Java IDE) is recommended for easy execution of the project.

### Steps to Run the Data Collection Script:

#### 1. **Download the Project Files**:

Make sure the following classes are included in your project:

* `ParkingLot.java`
* `TicketingSystem.java`
* `PaymentSystem.java`
* `DataCollectionScript.java` (Script to collect data)

#### 2. **Compile the Code**:

* **Using NetBeans**: NetBeans automatically compiles the project files when opened.
* **Using Command Line**:

  * Navigate to your project directory.
  * Run the following command to compile all Java files:

    ```bash
    javac -d bin src/com/mycompany/parkinglotsystem/*.java
    ```

#### 3. **Run the Data Collection Script**:

The data collection script simulates parking lot entries and exits, logs the parking availability, and records the data in a log file.

* **Using NetBeans**:

  * Right-click on `DataCollectionScript.java` and select **Run File**.
* **Using Command Line**:

  * Navigate to the root project directory.
  * Run the following command:

    ```bash
    java -cp bin com.mycompany.parkinglotsystem.DataCollectionScript
    ```

#### 4. **View the Results**:

After running the data collection script, the parking lot data will be logged into a text file named `parking_data_log.txt` in the root directory of your project.

* Open the `parking_data_log.txt` file to view the following details:

  * Parking lot availability
  * Vehicle assignments (including vehicle type and spot number)
  * Entry and exit times for each vehicle
  * Payment amounts and any change given to the user

---

## Example Data Log (parking\_data\_log.txt)

```txt
--- Parking Lot Data Log ---
Date: 2025-05-07

Spot 1: Occupied by vehicle ABC123 (Car) [Entry: 2025-05-07 10:00]
Spot 2: Occupied by vehicle XYZ456 (Truck) [Entry: 2025-05-07 10:05]
Spot 3: Available
Spot 4: Occupied by vehicle LMN789 (Car) [Entry: 2025-05-07 10:15]
Spot 5: Occupied by vehicle PQR321 (Motorcycle) [Entry: 2025-05-07 10:30]

--- Vehicle Exits ---
Spot 1: Vehicle ABC123 [Exit: 2025-05-07 12:00] - Fee: $15.00 - Payment: $15.00 - Change: $0.00
Spot 2: Vehicle XYZ456 [Exit: 2025-05-07 12:30] - Fee: $20.00 - Payment: $20.00 - Change: $0.00

--- Admin Summary ---
Total Revenue: $35.00
Average Parking Duration: 105.00 minutes
```

This log file captures the parking lot status, vehicle assignments, entry and exit times, payment processing, and an administrative summary of the day's revenue and average parking duration.


