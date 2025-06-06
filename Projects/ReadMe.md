# Campus Entry/Exit Management System

This Python program processes and manages the entry and exit records of IIIT-D students living off-campus. The data includes entries with the student's name, crossing type (ENTER or EXIT), gate number, and time (in 24-hour format). The program performs the following tasks:

---

## Features

1. **Data Processing and Storage**:
   - Reads a sorted data file containing student entry and exit records.
   - Stores the data in a nested dictionary where each student's records are maintained with details of crossing type, gate number, and time.

2. **Query Functions**:
   - **Query 1**: Displays a student's movements throughout the day and determines if the student is currently on campus.
   - **Query 2**: Identifies students who entered or exited the campus within a specified time range and saves the results to an output file.
   - **Query 3**: Calculates the number of entries and exits through a specific gate.

---

## Installation and Usage

### Prerequisites
- Python 3.x

### Setup
1. Place the sorted data file (`sorted_data.txt`) in the same directory as the Python script.
2. Run the Python script.

### Running the Program
- Execute the script in a Python environment.
- Follow the on-screen instructions to select and perform queries.

---

## Code Overview

### Data Reading and Storage
The program reads a sorted data file (`sorted_data.txt`) line by line and extracts:
- Student name
- Crossing type (ENTER/EXIT)
- Gate number
- Time (in 24-hour format)

This data is stored in a nested dictionary with the student's name as the key.

### Query Functions
1. **Query 1**:  
   - Input: Student name and current time.  
   - Output: Displays the student's movements for the day and whether they are currently on campus. Results are written to `query1_output.txt`.  

2. **Query 2**:  
   - Input: Start time and end time.  
   - Output: Lists all students who entered or exited the campus during the specified time period. Results are written to `query2_output.txt`.  

3. **Query 3**:  
   - Input: Gate number.  
   - Output: Displays the count of entries and exits through the specified gate.

### Main Loop
The program operates in a loop, allowing users to select a query (1 to 3) or exit by pressing Enter. It processes user input and executes the corresponding query function.

---

## Example Usage

### Query 1: Student Movements and Campus Presence
```plaintext
Select option (1 to 3), or press Enter to exit:
Enter option: 1
Enter student name: John_Doe
Enter current time: 15:30
```
Output: Displays John Doe's movements for the day and their campus presence status.

---

### Query 2: Students Entering/Exiting During a Time Range
```plaintext
Select option (1 to 3), or press Enter to exit:
Enter option: 2
Enter start time: 09:00
Enter end time: 17:00
```
Output: Lists all students who entered or exited the campus between 09:00 and 17:00.

---

### Query 3: Gate Usage Statistics
```plaintext
Select option (1 to 3), or press Enter to exit:
Enter option: 3
Enter gate number: 1
```
Output: Displays the number of entries and exits through gate number 1.

---

## Output Files

- **`query1_output.txt`**: Contains the queried student's movements and current campus presence status.
- **`query2_output.txt`**: Lists all students who entered or exited the campus within a specified time range.

---

## Conclusion

The Campus Entry/Exit Management System efficiently processes and queries entry/exit records, making it a valuable tool for campus management.
