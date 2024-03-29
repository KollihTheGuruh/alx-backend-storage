# MongoDB Tasks

## Tasks

### 0. List all databases

**File:** `0-list_databases`

Write a script that lists all databases in MongoDB.

### 1. Create a database

**File:** `1-use_or_create_database`

Write a script that creates or uses the database `my_db`.

### 2. Insert document

**File:** `2-insert`

Write a script that inserts a document in the collection `school` with the attribute `name` set to "Holberton school".

### 3. All documents

**File:** `3-all`

Write a script that lists all documents in the collection `school`.

### 4. All matches

**File:** `4-match`

Write a script that lists all documents with `name="Holberton school"` in the collection `school`.

### 5. Count

**File:** `5-count`

Write a script that displays the number of documents in the collection `school`.

### 6. Update

**File:** `6-update`

Write a script that adds a new attribute `address` with the value “972 Mission street” to documents with `name="Holberton school"` in the collection `school`.

### 7. Delete by match

**File:** `7-delete`

Write a script that deletes all documents with `name="Holberton school"` in the collection `school`.

### 8. List all documents in Python

**File:** `8-all.py`

Write a Python function that lists all documents in a collection.

### 9. Insert a document in Python

**File:** `9-insert_school.py`

Write a Python function that inserts a new document in a collection based on `kwargs`.

### 10. Change school topics

**File:** `10-update_topics.py`

Write a Python function that changes all topics of a school document based on the name.

### 11. Where can I learn Python?

**File:** `11-schools_by_topic.py`

Write a Python function that returns the list of school having a specific topic.

### 12. Log stats

**File:** `12-log_stats.py`

Write a Python script that provides stats about Nginx logs stored in MongoDB.

### 13. Regex filter

**File:** `100-find`

Write a script that lists all documents with name starting by "Holberton" in the collection `school`.

### 14. Top students

**File:** `101-students.py`

Write a Python function that returns all students sorted by average score.

### 15. Log stats - new version

**File:** `102-log_stats.py`

Improve `12-log_stats.py` by adding the top 10 of the most present IPs in the collection `nginx` of the database `logs`.
