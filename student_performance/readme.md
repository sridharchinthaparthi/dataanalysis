# Student Marks Management System

A simple Jupyter Notebook application for managing and analyzing student marks using NumPy.

## Features

- Input marks for multiple students and subjects
- View individual student performance
- Analyze subject-wise performance
- Update marks (re-evaluation)
- Pass/Fail evaluation (35+ marks)
- Calculate totals and averages
- Generate class statistics

## Usage

1. Run all cells in the notebook
2. Enter number of students and subjects when prompted
3. Input marks for each student
4. Use the interactive menu for various operations:
   - View student marks
   - View subject performance
   - Update marks
   - Check pass/fail status
   - Calculate statistics

## Example

```
Enter number of students: 3
Enter number of subjects: 4

Enter marks for Student 1:
 Subject 1: 85
 Subject 2: 78
 Subject 3: 92
 Subject 4: 88

--- Marks Data (Students x Subjects) ---
[[85 78 92 88]
 [76 82 69 91]
 [94 87 85 79]]

Choose an option:
1. View marks of a student
2. View marks of a subject
3. Update marks (Re-evaluation)
4. Pass/Fail Check
5. Student-wise Total and Average
6. Subject-wise Highest and Lowest
7. Overall Class Performance
8. Exit
```

## Sample Output

**Student Performance:**
```
Student 1 -> Total: 343, Average: 85.75
Student 2 -> Total: 318, Average: 79.50
Student 3 -> Total: 345, Average: 86.25
```

**Pass/Fail Check:**
```
Pass/Fail Matrix (True=Pass, False=Fail):
[[ True  True  True  True]
 [ True  True  True  True]
 [ True  True  False True]]
```

**Subject Statistics:**
```
Subject 1 -> Highest: 94, Lowest: 76
Subject 2 -> Highest: 87, Lowest: 78
Subject 3 -> Highest: 92, Lowest: 69
Subject 4 -> Highest: 91, Lowest: 79
```

**Class Performance:**
```
Class Total Marks: 1006
Class Average Marks: 83.83
Highest Marks in Class: 94
Lowest Marks in Class: 69
```

## Key Operations

- **View Student**: `marks_array[student_index]`
- **View Subject**: `marks_array[:, subject_index]`
- **Update Mark**: `marks_array[student, subject] = new_value`
- **Pass/Fail**: `marks_array >= 35`
- **Statistics**: `sum()`, `mean()`, `max()`, `min()`

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## Author

**Your Name**
- GitHub: [@sridharchinthaparthi](https://github.com/sridharchinthaparthi)

## License

MIT License
