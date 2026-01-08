# 🌲 C++ Decision Tree Classifier

<div align="center">



![GitHub language top](https://img.shields.io/github/languages/top/ShivJee-Yadav/Decision-Tree-Classifier?style=for-the-badge&logo=c%2B%2B&logoColor=white&color=blue)

**A optimized C++ implementation of the Decision Tree ID3 classification algorithm.**

</div>

## 📖 Overview

This repository presents a pure C++ implementation of a Decision Tree Classifier, a powerful and widely used machine learning algorithm for both classification and regression tasks. 

This project focuses on providing a clear and efficient implementation, suitable for understanding the core mechanics of decision tree algorithms, including entropy calculation, information gain, tree construction, and prediction. It processes tabular data from CSV files, making it a self-contained tool for classification experiments.

## ✨ Features

-   **Decision Tree Algorithm:** Full implementation of a classification decision tree.
-   **Entropy Calculation:** Core logic for calculating information entropy.
-   **Information Gain:** Measures the effectiveness of splitting data on a given attribute.
-   **CSV Data Handling:** Reads and processes tabular datasets from CSV files for training and prediction.
-   **Prediction:** Uses the trained tree to classify new, unseen data points.
-   **Standalone Executable:** Compiles into a single executable for ease of use.
-   **Print Decision Tree**: Visualize the decision tree with split conditions ( Level-wise or top-Down).
-   **Verify Predictions**: Evaluate the model using test data.
-   **Show Training Data Table**: Display the complete training dataset.
-   **Show Specific Row**: Retrieve any row from the training data.
-   **Count Unique Attributes**: Count unique values for each feature.
-   **Calculate Information Gain**: Compute Information Gain for each feature.
-   **Calculate Entropy**: Measure the impurity of data using Entropy.

## 🛠️ Tech Stack

**Libraries:**
-   **C++ Standard Library:** For core functionalities like input/output, data structures (vectors, maps), and mathematical operations.

## 🚀 Quick Start

To get started with the Decision Tree Classifier, you'll need a C++ compiler.

### Prerequisites
-   A C++ compiler (e.g., GCC, Clang, MSVC).
    -   On Linux/macOS: Install `g++` (usually comes with `build-essential` or Xcode Command Line Tools).
    -   On Windows: Install MinGW-w64 or Visual Studio with C++ development tools.

### Installation & Compilation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/ShivJee-Yadav/Decision-Tree-Classifier.git
    cd Decision-Tree-Classifier
    ```

2.  **Compile the source code**
    Use a C++ compiler like `g++` to compile all `.cpp` files and link them.
    ```bash
    g++ EntropyCal.cpp Information_entropy.cpp Input_DTC.cpp Tree.cpp -o Tree -std=c++11 -O2
    ```
    *   `-o Tree`: Specifies the output executable name as `Tree` (or `Tree.exe` on Windows).
    *   `-std=c++11`: Ensures C++11 standard features are available (e.g., for `std::to_string` or other modern C++ constructs).
    *   `-O2`: Optimization flag for better performance.

### Usage

After successful compilation, an executable named `Tree` (or `Tree.exe`) will be created in the repository root.

1.  **Prepare your dataset**
    Ensure your dataset is in a CSV format. Example datasets like `car_evaluation.csv` are provided. The last column of your CSV is expected to be the target/class variable.

2.  **Run the classifier**
    Execute the compiled program, typically providing the dataset as an input.
    ```bash
    ./Tree
    ```
    The program will likely prompt you to enter the CSV file name and other necessary parameters (e.g., columns to use) directly in the console.

    **Example with provided data:**
    ```bash
    ./Tree
    # The program will then guide you through inputs (e.g., enter car_evaluation.csv)
    ```

## 📁 Project Structure

```
Decision-Tree-Classifier/
├── EntropyCal.cpp          # Implements entropy calculation logic
├── Information_entropy.cpp # Contains functions for information gain and related entropy measures
├── Input_DTC.cpp           # Handles reading and parsing input data from CSV files
├── prediction.h            # Header file likely containing declarations for prediction-related functions or data structures
├── Tree.cpp                # Main implementation of the Decision Tree algorithm (tree building, traversal, classification)
├── Tree.exe                # Compiled executable (Windows)
├── car2.csv                # Sample dataset
├── car3.csv                # Sample dataset
├── car_evaluation.csv      # Primary sample dataset for car evaluation
├── README.md               # This README file
└── README                  # Original README file
```
*Note: `Index.html` is an empty file and is not part of the core C++ project functionality.*

## 🔧 Development

### Compiling for Development

During development, you might want to compile without optimizations or with debugging symbols:

```bash
g++ EntropyCal.cpp Information_entropy.cpp Input_DTC.cpp Tree.cpp -o Tree -std=c++11 -g
```
*   `-g`: Includes debugging information, useful when using a debugger.

### Code Organization
-   The project is organized into modular `.cpp` files, each responsible for a specific aspect of the decision tree algorithm.
-   `prediction.h` likely defines the interfaces or data structures used for building and predicting with the tree.

## 🧪 Testing

Given this is a standalone C++ implementation without an explicit testing framework, testing typically involves:

1.  **Running with Sample Data:** Execute the `Tree` program with the provided `car_evaluation.csv` and other `.csv` files.
2.  **Verifying Output:** Manually inspect the console output for classification results, tree structure, or metrics, comparing them against expected outcomes or known ground truth for the datasets.
3.  **Custom Datasets:** Create small, custom CSV datasets with known outcomes to validate specific scenarios and edge cases of the decision tree.

## 🙏 Acknowledgments

-   Inspired by the foundational concepts of Decision Trees and Information Theory in Machine Learning.
-   The C++ programming community for robust tools and resources.

<div align="center">
Made with ❤️ by [ShivJee-Yadav](https://github.com/ShivJee-Yadav)

</div>
