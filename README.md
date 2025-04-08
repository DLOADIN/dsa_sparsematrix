# BX Operator

A high-performance library for advanced sparse matrix operations.

## Overview

BX Operator provides a powerful command-line interface for working with sparse matrices. It efficiently handles large matrix operations through optimized algorithms and memory management techniques.

## Features

- **Matrix Management**
  - Import matrices from standard file formats
  - Export results to various formats
  - Memory-efficient sparse representation

- **Core Operations**
  - Matrix addition and subtraction
  - Matrix multiplication with optimized algorithms
  - Transpose operation
  - Conversion to/from Compressed Sparse Row (CSR) format

- **Interactive CLI**
  - User-friendly command interface
  - Progress indicators for long-running operations
  - Comprehensive error reporting

## Installation

```bash
# Clone the repository
git clone https://github.com/DLOADIN/dsa_sparsematrix.git

# Navigate to project directory
cd dsa_sparsematrix

# Install dependencies
pip install -r requirements.txt
```

## Usage

### Starting the Application

```bash
python drain.py
```

### Basic Commands

| Command | Description |
|---------|-------------|
| `load <file1> <file2>` | Load two matrices from specified files |
| `opp + <output_file>` | Add matrices and save to output file |
| `opp - <output_file>` | Subtract matrices and save to output file |
| `opp * <output_file>` | Multiply matrices and save to output file |
| `help` | Display available commands |
| `exit` | Exit the application |

### Example Session

```
$ python drain.py
BX Operator v1.0.0
> load matrix1.txt matrix2.txt
Matrices loaded successfully.
> opp * result.txt
Operation completed successfully.
> exit
```

## Input File Format

BX Operator accepts matrices in the following format:

```
rows=3
cols=3
(1 0 0)
(0 1 0)
(0 0 1)
```

- The first line specifies the number of rows
- The second line specifies the number of columns
- Subsequent lines contain the matrix values in parentheses
- Values must be space-separated

## Error Handling

The application provides detailed error messages for common issues:
- File not found or permission errors
- Matrix dimension mismatches
- Invalid file formats
- Memory limitations

## Performance Considerations

- Optimized for sparse matrices with many zero elements
- Memory usage scales with the number of non-zero elements rather than matrix dimensions
- Large matrices may require significant processing time for multiplication operations

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b new-feature`
3. Commit your changes: `git commit -am 'Add new feature'`
4. Push to the branch: `git push origin new-feature`
5. Submit a pull request

