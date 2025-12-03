<div align="center">

# 🐾 FurEverHome

Your console-based pet adoption-donation system.  

**IT 2110**  

Estiva, Lorenz Daniell C.  
Lontoc, Kieron Ann A.  
Mangubat, Annika Grace P.

</div>


---

## ₊˚ ┊ Overview
FurEverHome is a console-based Java application for managing **pet adoptions** and **donations**. It allows users to add, view, modify, delete, and insert records for pets, adoptions, and donations directly through the terminal.

The application demonstrates practical use of **Object-Oriented Programming (OOP) concepts** such as encapsulation, inheritance, polymorphism, and abstraction, alongside proper file handling and modular design.

Users can:
- 🐾 Add a new pet for adoption
- 🎉 Record an adoption
- 💖 Record a donation
- 📘 View all records
- ✍🏻 Modify or delete specific records
- ✨ Insert a record at any position

All records are stored in a plain text file: `furever_diary.txt`.

---

## ₊˚ ┊ Project Structure

📂 src/

└── 📂 fureverhome/

├── ☕ Main.java 

├── ☕ Diary.java 

├── ☕ RecordEntry.java 

├── ☕ PetEntry.java 

├── ☕ AdoptionEntry.java 

├── ☕ DonationEntry.java 

└── ☕ FileHandler.java 

- `Main.java` – Entry point, handles user interactions and menu.
- `Diary.java` – CRUD operations for all records.
- `RecordEntry.java` – Abstract superclass demonstrating inheritance and polymorphism.
- `PetEntry.java`, `AdoptionEntry.java`, `DonationEntry.java` – Subclasses of `RecordEntry` showing inheritance and polymorphism.
- `FileHandler.java` – Handles file creation, reading, writing, and appending (abstraction).

---

## ₊˚ ┊ Features
- **Add Pet** – Create a new pet adoption record with timestamp.
- **Record Adoption** – Log an adoption event.
- **Record Donation** – Log a donation with optional message.
- **View Records** – Display all records with numbering.
- **Modify Record** – Edit any existing record.
- **Delete Record** – Remove a record permanently.
- **Insert Record** – Add a record at a specific position.

---

## ₊˚ ┊ Object-Oriented Principles

### 💊 Encapsulation
- Private and protected fields in classes like `Diary` and `RecordEntry`.
- Data accessed only through class methods (`addEntry()`, `viewRecords()`, etc.).
- Ensures data integrity and controlled access.

### 💡 Abstraction
- `FileHandler` abstracts file operations (read/write/append).
- `RecordEntry` abstracts the record format.
- `Diary` interacts with records without needing to know internal details.

### 🧬 Inheritance
- `RecordEntry` is an abstract superclass.
- `PetEntry`, `AdoptionEntry`, and `DonationEntry` inherit from it.
- Allows code reuse and flexibility for future extensions.

### 🎭 Polymorphism
- `format()` method is overridden in each subclass for dynamic behavior.
- `Diary.addEntry()` can accept any subclass of `RecordEntry`.
- Switch statement in `Main.java` demonstrates method-level polymorphism.

---

## ₊˚ ┊ Example Output

🐾 Welcome to FurEverHome 🐾

1. Add Pet for Adoption

2. Record Adoption

3. Record Donation

4. View Records

5. Modify Record

6. Delete Record

7. Insert Record

8. Exit

   
Choose an option: 1

Pet Name: Bella

Species: Dog

Age: 2

✅ Entry added successfully!


---

## ₊˚ ┊ How to Run the Program

1. Open a terminal in the `src/` folder.
2. Compile the Java files:
javac fureverhome/*.java

## ₊˚ ┊ **Contributors**

Lorenz Daniell Estiva  
Kieron Ann Lontoc  
Annika Grace Mangubat
