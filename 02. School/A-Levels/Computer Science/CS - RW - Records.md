---
title: <% tp.file.title %>
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-03-25
tags:
  - A-Level
  - Data-Structures
  - CS
  - Computer-Science
type: Lesson Note
---
> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}

# What is a Record?
- More commonly referred to as a *row in a file* and is made up of *fields*
- Groups related fields together under one unit
- Are a composite data structure -> Holds multiple fields with different data types
- Each field holds a specific piece of data with its own data type
- Records are typically used in databases ![[Pasted image 20250325155758.png]]![[Pasted image 20250325160042.png]]
- Are used to save data so it can be accessed for subsequent usage
## Python Example

```python
# Dictionary representation of a record
student = {
    "name": "John Doe",
    "age": 18,
    "grade": "A",
    "ID": 12345
}
# Accessing record fields
print(student["name"])  # Output: John Doe
```
# Related Notes
[[Computer Science MOC]]
[[CS - RW - Data Structures]]