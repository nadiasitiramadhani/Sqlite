🐾 Projek with SQLite & Python






📌 Overview

Project ini merupakan implementasi data wrangling menggunakan SQLite dan Python, mulai dari pembuatan database, manipulasi data menggunakan SQL, hingga transformasi data menjadi DataFrame untuk analisis.

Fokus utama:

Database management (SQLite)
SQL Query (DDL & DML)
Relasi antar tabel
Integrasi Python dengan database
Data transformation ke Pandas
🎯 Objectives
Memahami cara kerja database SQLite
Mengimplementasikan operasi CRUD
Menggunakan query lanjutan (JOIN, GROUP BY)
Mengolah data menjadi format analisis (DataFrame)
🧰 Tech Stack
Python
SQLite (sqlite3)
Pandas
DB Browser for SQLite
⚙️ Workflow
1. Database Initialization
Membuat database pets.db
Menghubungkan Python ke SQLite
2. Table Creation
CREATE TABLE Pet (
    PetID INTEGER,
    PetName VARCHAR(25),
    OwnerName VARCHAR(100)
);

3. Data Insertion
INSERT INTO Pet VALUES (1, 'Felix', 'Alex');
INSERT INTO Pet VALUES (2, 'Auburn', 'Britt');

4. Data Manipulation
SELECT (menampilkan data)
ORDER BY (sorting ascending & descending)
ALTER TABLE (menambah kolom)
UPDATE (mengubah data)
DELETE (menghapus data)
5. Advanced Query

GROUP BY

SELECT COUNT(*), Gender FROM Pet GROUP BY Gender;


JOIN

SELECT PetName, OwnerName, TreatResult
FROM Pet
JOIN PetTreatment USING (PetID);

🧩 Database Schema
Table: Pet
Column	Type
PetID	Integer
PetName	Varchar
OwnerName	Varchar
Age	Integer
Gender	Varchar(1)
Table: PetTreatment
Column	Type
PetID	Integer
TreatDate	Date
TreatResult	Varchar
📊 Sample Output
Data Setelah Update
(1, 'Felix', 'Alex', 3, 'M')
(2, 'Auburn', 'Britt', 2, 'F')

GROUP BY Result
(2, 'M')
(2, 'F')

🔄 Data Transformation (SQLite → Pandas)
import pandas as pd

df = pd.DataFrame(data, columns=[
    "PetID", "PetName", "OwnerName",
    "Age", "Gender", "TreatDate", "TreatResult"
])


📌 Output:

Data siap untuk analisis lanjutan
Bisa digunakan untuk visualisasi / machine learning
🚀 How to Run
Install dependency:
pip install pandas

Jalankan script Python / Jupyter Notebook
Pastikan file database tersedia:
pets.db

📁 Project Structure
├── pets.db
├── source code.ipynb
├── penjelasan tiap langkah.pdf
└── README.md

💡 Key Insights
SQLite cocok untuk project skala kecil–menengah
SQL + Python = powerful untuk data wrangling
Relasi database meningkatkan integritas data
DataFrame mempermudah analisis lanjutan
👤 Author

Nadia Siti Ramadhani
S1 Sains Data – UPN “Veteran” Jawa Timur

⭐ Notes

Project ini dibuat untuk pembelajaran dan penguatan konsep:

Database
SQL Query
Data Wrangling
Data Analysis Preparation
