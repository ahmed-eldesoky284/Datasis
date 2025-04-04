# Datasis - A Python Library for Data Analysis

## Introduction
`Datasis` is a data analysis library built using `pandas`, `numpy`, `matplotlib`, and `seaborn`. It provides tools for loading, cleaning, analyzing data, handling outliers and duplicates, as well as filtering, grouping, and sorting data.

## Requirements
Make sure you have the following libraries installed before using `Datasis`:
```bash
pip install Datasis
```

## How to Use
### 1. Import the Class and Create an Object
```python
from data_analysis import Datasis

da = Datasis()
```

### 2. Load Data
```python
da.load_data("data.csv")  # Or any Excel or JSON file
```

### 3. Display Data
```python
print(da.show_data())  # Display the first 5 rows
print(da.tail())       # Display the last 5 rows
```

### 4. Get Data Info and Statistics
```python
print(da.get_info())
print(da.get_statistics())
```

### 5. Handle Missing Values
```python
print(da.missing_values())  # Show count of missing values per column
print(da.fill_missing(strategy='mean'))  # Replace missing values with the mean
```

### 6. Detect and Handle Outliers
```python
print(da.outlier_detection("column_name"))  # Detect outliers
print(da.drop_outliers("column_name"))  # Remove outliers
```

### 7. Remove Duplicates
```python
print(da.drop_duplicates())
```

### 8. Filter, Group, and Sort Data
```python
print(da.filter_data("column_name > 50"))  # Filter data based on a condition
print(da.group_by("category"))  # Group data by a specific column
print(da.sort_data("column_name", ascending=False))  # Sort data in descending order
```

### 9. Save Data After Modifications
```python
da.save_data("cleaned_data.csv")
```

## Contribution
If you'd like to improve the code or add new features, feel free to submit a pull request on GitHub.

## License
This library is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
## Contributing
Contributions are welcome! Feel free to submit issues or pull requests to improve the library.
## Author
Created by Ibrahem abo kila. For any inquiries, please contact me at ibrahemabokila@gmail.com.
