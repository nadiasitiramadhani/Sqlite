# 🐾 Data Wrangling with SQLite & Python

![Python](https://img.shields.io/badge/Python-3.x-blue)
![SQLite](https://img.shields.io/badge/Database-SQLite-lightgrey)
![Pandas](https://img.shields.io/badge/Data-Pandas-yellow)


## 📌 Overview
Project ini merupakan implementasi **data wrangling menggunakan SQLite dan Python**, mulai dari pembuatan database, manipulasi data menggunakan SQL, hingga transformasi data menjadi **DataFrame** untuk analisis.

Project ini mencakup:
- Pembuatan database SQLite
- Operasi CRUD (Create, Read, Update, Delete)
- Query lanjutan (JOIN, GROUP BY)
- Relasi antar tabel
- Integrasi Python dengan database
- Transformasi data ke Pandas DataFrame


## 🎯 Objectives
- Memahami penggunaan SQLite dalam Python
- Mengimplementasikan query SQL dasar dan lanjutan
- Membangun relasi antar tabel
- Mengolah data menjadi format siap analisis


## 🧰 Tech Stack
- Python
- SQLite (`sqlite3`)
- Pandas
- DB Browser for SQLite


## ⚙️ Workflow

1. Database Initialization
Membuat dan menghubungkan database SQLite menggunakan Python:

```python
import sqlite3

conn = sqlite3.connect("pets.db")
cursor = conn.cursor()
conn.close()

2. Data Manipulation

Operasi yang dilakukan:
- SELECT → menampilkan data
- ORDER BY → sorting data
- ALTER TABLE → menambah kolom
- UPDATE → mengubah data
- DELETE → menghapus data

💡 Key Insights
- SQLite cocok untuk project skala kecil hingga menengah
- SQL + Python sangat efektif untuk data wrangling
- Relasi database meningkatkan integritas data
- DataFrame mempermudah analisis lanjutan

👤 Author
Nadia Siti Ramadhani
S1 Sains Data – UPN “Veteran” Jawa Timur

⭐ Notes
Project ini dibuat untuk pembelajaran dan penguatan konsep:
- Database
- SQL Query
- Data Wrangling
- Data Analysis Preparation
