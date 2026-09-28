# WildlifeRescueSystem-
# Wildlife Rescue Operations System

## Student Information
- **Name:** Gcebile Dhlamini
- **Student Number:**st10519830
- **Module:** prog1B
- **Institution:** The Independent Institute of Education (IIE)

## Project Description
WildLife SA is a non-profit conservation organisation responsible for rescuing and rehabilitating injured, orphaned and endangered wildlife across Southern Africa. 

This Java application is a Wildlife Rescue Operations System developed to assist conservation staff in managing wildlife rescue cases. It replaces the manual paper-based system with a digital, easy-to-use solution.

## Features
The system allows staff to:
- **Create** new rescue cases with validation (unique ID, non-blank fields).
- **Search** for existing rescue cases using the Rescue Case ID.
- **Update** the rescue status of an existing case.
- **Display** all stored rescue cases.
- **Generate** a comprehensive rescue report showing all cases with priorities and total costs.

## Rescue Case Types Supported
1. **Injured Animal Rescue**
   - Stores: Injury Description, Veterinary Treatment Cost, Surgery Required
   - Cost calculation: Base cost + Vet cost + R5000 (if surgery is required)
   - Priority: Critical (if surgery required) / High

2. **Orphaned Animal Rescue**
   - Stores: Estimated Age (Months), Feeding Cost, Foster Care Required
   - Cost calculation: Base cost + Feeding cost + R2500 (if foster care is required)
   - Priority: High (if under 6 months) / Medium

## Technical Requirements Implemented
- **Language:** Java
- **Interface:** Graphical User Interface using `JOptionPane`
- **Storage:** `ArrayList` (in-memory)
- **OOP Principles:**
  - **Inheritance:** `InjuredAnimalRescue` and `OrphanedAnimalRescue` extend `RescueCase`
  - **Abstraction:** `RescueCase` is an abstract class; `RescueOperations` is an interface
  - **Encapsulation:** All fields are `private` with `public` getters/setters
  - **Polymorphism:** `calculateTotalCost()` and `getRescuePriority()` are overridden
- **Validation:** Unique Rescue Case ID, no blank fields, numeric input validation
- **Unit Testing:** JUnit tests verify cost calculations, priority logic, and ID uniqueness

## How to Run the Application
1. Open the project in NetBeans.
2. Locate `RescueSystem.java` in the `Source Packages` folder.
3. Right-click the file and select **Run File** (or press **Shift + F6**).
4. Use the on-screen menu (1-6) to interact with the system.

## File Structure
- `RescueSystem.java` - Main application (includes GUI, menu logic, and all supporting classes)
- `RescueSystemTest.java` - JUnit 5 unit tests
- `README.md` - Project documentation

## Assumptions
- The application is used by a single wildlife conservation organisation.
- All rescue cases are stored in memory (ArrayList) and reset when the application closes.
- Rescue Case IDs must be unique across the system
- link https://github.com/gcebiledhlamini13-max/WildlifeRescueSystem-/edit/main/README.md
