# 🚀 RideVault – Java + PostgreSQL Console App

RideVault is a modular Java console application simulating a dynamic ride booking system backed by PostgreSQL. Built with layered design principles separating business logic, data handling, and user interaction.

---

## 📁 Project Structure

```text
RideVault-CLI/
├── Database/
│   └── schema.sql                    # PostgreSQL database setup script
├── src/main/java/com/RideVault/
│   ├── model/                        # Data classes (Rider, Driver, Location, Wallet)
│   ├── dao/                          # Database operations and queries
│   ├── service/                      # Business logic (pricing, booking, users)
│   └── Main.java                     # Main entry point and CLI menus
├── pom.xml                           # Maven configuration file
└── README.md

```

---

## 🚀 Features

* User Login/Signup and Authentication for Riders and Drivers
* JDBC-based PostgreSQL database integration
* Ride-sharing backend logic (dynamic pricing, booking, state management)
* Console-based interactive portals
* Clean modular Java design using OOP principles
* Extensible service and data access layers

---

## 🎮 How to Run

### ✅ Compile the Project

**Windows (PowerShell with Maven):**

```bash
mvn clean compile

```

**Linux/macOS:**

```bash
mvn clean compile

```

### ▶ Run the App

**Windows:**

```bash
mvn exec:java -Dexec.mainClass="com.RideVault.Main"

```

**Linux/macOS:**

```bash
mvn exec:java -Dexec.mainClass="com.RideVault.Main"

```

---

## 🛠️ Requirements

* Java 8 or above
* PostgreSQL Database (v12+)
* Maven (Build tool to automatically handle the JDBC driver)
* Terminal or IDE (IntelliJ, Eclipse, VS Code etc.)

---

## 📚 Class Overview

### `Main.java`

* Main class that starts the application
* Connects UI menus and delegates tasks to service layers

### `model/`

* Contains data classes like `Rider.java`, `Driver.java`, `Location.java`

### `service/`

* Logic for booking rides, calculating fares, and user operations

### `dao/`

* JDBC interactions with the database (inserting users, updating wallets)

---

## 📌 Notes

* Ensure your PostgreSQL DB is set up using the `schema.sql` file provided
* Edit database credentials (username/password) inside `DatabaseConnection.java`
* Ensure PostgreSQL is running locally on port `5432` before starting

  
