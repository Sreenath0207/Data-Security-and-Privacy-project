# SecureDB_Project

## Overview

This project is designed for a class on Data Security and Privacy. It aims to create a secure database-as-a-service system focusing on healthcare information. The project demonstrates various security features such as user authentication, access control, data confidentiality, and query integrity.

## Features

### Authentication

- Uses SHA-256 hashing for passwords.
- Verifies user credentials before allowing access.

### Access Control

- Differentiates between two groups of users: 'H' (can access all fields) and 'R' (restricted access).
  
### Data Confidentiality

- Encrypts sensitive fields like 'age' and 'gender' using Fernet symmetric encryption.

### Query Integrity

- Creates and verifies hashes for data items to ensure data integrity.
- Verifies the completeness of query results.

## Directory Structure
SecureDB_Project/
├── README.md
├── Report.docx
├── secure_db.sqlite
├── src
│   ├── access_control.py
│   ├── authentication.py
│   ├── data_confidentiality.py
│   ├── db_setup.py
│   ├── main.py
│   ├── query_integrity.py
└── tests
    ├── test_access_control.py
    ├── test_authentication.py
    ├── test_data_confidentiality.py
    └── test_query_integrity.py

## How to Run

1. Clone the repository.
2. Navigate to the `src` directory.
3. Run `db_setup.py` to set up the initial SQLite database.

```python
python db_setup.py
```

4. Run `main.py` to execute the program.

```python
python main.py
```

## Author

Ian Peter

## License

[MIT](https://choosealicense.com/licenses/mit/)