# Library-Management-System
This project is an **Object-Oriented Library Management System** implemented in Python. It serves as an excellent demonstration of **Object-Oriented Programming (OOP)** principles, specifically how different classes interact to model real-world relationships between entities (Books, Users, and a Library).

---

## 🚀 Key Features

* **Object-Oriented Design:** Utilizes specialized classes for `Book`, `User`, and `Library` to encapsulate data and behavior.
* **Transaction Management:** A logical system for issuing and returning books that updates both the library inventory and the user's personal borrowing list.
* **Availability Tracking:** Prevents double-booking by tracking the `is_issued` status of every book in the collection.
* **Error Handling:** Built-in validation to check for non-existent User IDs, invalid ISBNs, or books that are already checked out.
* **Inventory Visualization:** A formatted dashboard to view all books, their authors, and current availability at a glance.

---

## 🛠️ Project Architecture

The system is built on the interaction between three primary components, showcasing the power of **Class Composition**.

* **Book Class:** Stores metadata (ISBN, Title, Author) and its current circulation status.
* **User Class:** Manages user identity and maintains a list of currently borrowed `Book` objects.
* **Library Class:** The "Controller" that manages the collections of users and books, handling the logic for transactions.

---

## 💻 Technical Highlights

* **Composition & Relationships:** The `Library` class "has-a" collection of `Book` and `User` objects, demonstrating how complex systems are built from simpler parts.
* **Dictionary-Based Lookups:** Uses Python dictionaries (`{}`) for ISBN and User ID storage, ensuring $O(1)$ time complexity for searching records.
* **Status Logic:** Employs boolean flags to toggle book states, ensuring data integrity during high-frequency transactions.
* **Modular Interface:** Separation of the "Backend" logic (the classes) from the "Frontend" (the `main()` loop), making the code easy to test and extend.

---

## 📖 How to Run

1. **Clone the Repo:**
```bash
git clone https://github.com/your-username/oop-library-system.git

```


2. **Run the Script:**
```bash
python library_system.py

```


3. **Demo Data:** The system comes pre-loaded with a user (`kalpu__0907`) and two books to get you started immediately.

---

* Saving data to a JSON/SQL file?
* Adding due dates and late fines?
* Searching by Author or Title?
* Adding an admin login?

What feature are you planning to code next?
