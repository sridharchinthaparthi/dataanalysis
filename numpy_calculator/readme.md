# NumPy Mathematical Calculator

A comprehensive command-line calculator built with NumPy that provides powerful array operations, statistical analysis, and array manipulation capabilities.

## 🚀 Features

### 1. Basic Arithmetic Operations
- **Element-wise operations** between two arrays
- Addition, Subtraction, Multiplication, Division
- Power operations using `np.power()`
- Automatic error handling for incompatible array shapes

### 2. Statistical Operations
- **Descriptive Statistics**: Mean, Median, Standard Deviation, Variance
- **Array Properties**: Shape, Size, Data Type
- **Extremes**: Minimum, Maximum values
- **Aggregations**: Sum, Product of all elements

### 3. Array Manipulation
- **Dynamic Reshaping**: Automatically finds all possible 2D and 3D reshape combinations
- **Sorting**: Ascending and descending order
- **Filtering**: Elements greater than mean value
- **Array Information**: First/last elements, unique values


## 💻 Usage

### Quick Start

Run the program and choose from the interactive menu:

```
==================================================
        NUMPY MATHEMATICAL CALCULATOR
==================================================
1. Basic Arithmetic Operations
2. Statistical Operations
3. Array Manipulation
4. Exit
==================================================
```

### Input Format

Enter numbers separated by spaces when prompted:
```
Enter Array 1:
Enter numbers separated by spaces: 1 2 3 4 5
```

### Example Outputs

**Basic Arithmetic:**
```
Array 1: [1. 2. 3. 4. 5.]
Array 2: [2. 4. 6. 8. 10.]

Addition: [3. 6. 9. 12. 15.]
Subtraction: [-1. -2. -3. -4. -5.]
Multiplication: [2. 8. 18. 32. 50.]
Division: [0.5 0.5 0.5 0.5 0.5]
Power: [1. 16. 729. 65536. 9765625.]
```

**Statistical Analysis:**
```
Array: [1. 2. 3. 4. 5.]
Shape: (5,)
Size: 5
Data type: float64

Mean: 3.0000
Median: 3.0000
Standard Deviation: 1.4142
Variance: 2.0000
Minimum: 1.0
Maximum: 5.0
Sum: 15.0
Product: 120.0
```

**Array Manipulation:**
```
Original Array: [1. 2. 3. 4. 5. 6.]

All possible 2D reshapes:
(1, 6):
[[1. 2. 3. 4. 5. 6.]]

(2, 3):
[[1. 2. 3.]
 [4. 5. 6.]]

(3, 2):
[[1. 2.]
 [3. 4.]
 [5. 6.]]

All possible 3D reshapes:
(1, 1, 6):
[[[1. 2. 3. 4. 5. 6.]]]

(1, 2, 3):
[[[1. 2. 3.]
  [4. 5. 6.]]]
```

## 🔧 Code Structure

```
numpy_calculator.py
├── input_array()           # Handles user input and array creation
├── basic_arithmetic()      # Performs element-wise operations
├── statistical_operations() # Calculates statistical measures
├── array_manipulation()    # Handles reshaping and sorting
└── main()                 # Main program loop and menu
```

## ✨ Key Features Explained

### Smart Reshaping Algorithm
The program automatically calculates all mathematically valid reshapes for your array:
- **2D Reshapes**: Finds all factor pairs of array length
- **3D Reshapes**: Finds all valid combinations of three factors
- **Error Handling**: Gracefully handles impossible reshape operations

### Robust Input Handling
- Accepts any sequence of numbers separated by spaces
- Automatic conversion to NumPy float arrays
- Error handling for invalid operations (e.g., mismatched array sizes)

### Comprehensive Statistics
Beyond basic operations, provides complete statistical analysis including:
- Central tendency measures (mean, median)
- Variability measures (standard deviation, variance)
- Array metadata (shape, size, data type)

## 🚨 Error Handling

The calculator includes comprehensive error handling for:
- **Shape Mismatch**: When arrays have incompatible shapes for arithmetic operations
- **Division by Zero**: Automatic handling of zero division cases
- **Invalid Reshapes**: When requested shapes are mathematically impossible
- **Input Validation**: Graceful handling of invalid user inputs

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 Future Enhancements

- [ ] Matrix operations (dot product, cross product, determinant)
- [ ] Linear algebra functions (eigenvalues, eigenvectors)
- [ ] Advanced statistical functions (correlation, regression)
- [ ] File I/O for saving/loading arrays
- [ ] Plotting capabilities with matplotlib integration
- [ ] Support for complex numbers
- [ ] Broadcasting explanation for mismatched arrays

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@sridharchinthaparthi](https://github.com/sridharchinthaparthi)
- Email: your.email@example.com

## 🙏 Acknowledgments

- NumPy community for the excellent documentation
- Python community for continuous inspiration
- Contributors and users who provide feedback

---

⭐ **Star this repository** if you found it helpful!

## 📊 Example Use Cases

**Data Analysis**: Quick statistical analysis of datasets
```python
# Example: Analyzing test scores
scores = [85, 92, 78, 96, 88, 91, 87, 93]
# Use Statistical Operations to get mean, median, std dev
```

**Mathematical Computations**: Element-wise operations on vectors
```python
# Example: Physics calculations
velocity = [10, 15, 20, 25]
time = [2, 3, 4, 5]
# Use Basic Arithmetic to calculate distance = velocity * time
```

**Array Processing**: Reshaping data for different applications
```python
# Example: Image processing
pixel_data = [255, 128, 64, 32, 16, 8, 4, 2, 1]
# Use Array Manipulation to reshape into different matrix forms
```
