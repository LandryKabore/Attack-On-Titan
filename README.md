# Attack on Titan Fandom Database Web App  
**CMSC 4323 - Database Systems — Final Project**  
**Author:** Landry Muntasir Kabore

---

Overview
This project is a full-stack web application built using **Flask**, **MySQL**, and **SQLAlchemy**.  
It simulates an Attack on Titan (AOT) fandom database with:

- Character information  
- Titan forms  
- Organizations  
- Episodes  
- Character episode appearances  

The system supports complete **CRUD operations, includes **LLM natural language SQL querying**, and contains a **large dataset (2000+ rows)** automatically generated.



Features

1. Graphical User Interface (GUI)
The Flask GUI allows users to:

- **Create** new characters  
- **View** all characters  
- **Edit** status  
- **Delete** characters (with cascade cleanup)  

All forms and views are designed for beginners and simplicity.

---

 2. Natural Language to SQL (LLM Integration)
The `/ask` page allows users to type questions in English, such as:
> “Which characters are alive?”  
> “List all dead characters.”  
> “Which episodes feature Eren Yeager?”  

The app uses **GPT-4.1-mini** to convert these questions into a **safe SELECT SQL query**, then executes it and displays the results.

**Safety enforced:**
- Only SELECT statements allowed  
- Inserts/Updates/Deletes are blocked  
- Reserved word `character` is automatically escaped  

---

 

Final database size:
- **46 characters**
- **48 episodes**
- **2000+ episode appearance rows**  



---

Project Structure


