# DATA STRUCTURES AND ALGORITHMS- CO2003

# ASSIGNMENT 1 - PROCESSING MNIST DATASET AND IMPLEMENTING kNN ALGORITHM USING LIST

## ASSIGNMENT'S SPECIFICATION

## Version 1.1

### 1. Assignment's Outcome

Upon completing this assignment, students will review and apply:

- Object Oriented Programming (OOP)
- List data structures
- Sorting algorithms

### 2. Introduction

Classification stands as one of the fundamental tasks in machine learning, involving the categorization of data into distinct groups or classes based on their attributes. Examples include sorting emails as spam or non-spam, identifying images as cat or dog, etc. In this assignment, students will delve into the k-nearest neighbors (kNN) algorithm, a simple yet effective classification approach. They will apply this algorithm to process and classify the MNIST dataset.

Students are tasked with implementing a class enabling the processing of the MNIST dataset. Additionally, they must develop a class efficiently executing the kNN classification algorithm utilizing list data structures.

## Implementation Details

### Class: List

- **Purpose:** Represents a generic list data structure.
- **Functionality:**
  - Provides operations for managing a list of elements.
  - Supports dynamic resizing and efficient element access.

#### Member Functions:

1. `push_back(T value)`: Adds an element to the end of the list.
2. `push_front(T value)`: Inserts an element at the beginning of the list.
3. `insert(int index, T value)`: Inserts an element at the specified index in the list.
4. `remove(int index)`: Removes the element at the specified index from the list.
5. `get(int index) const`: Retrieves the element at the specified index.
6. `length() const`: Returns the number of elements in the list.
7. `clear()`: Removes all elements from the list.
8. `print() const`: Prints the elements of the list.
9. `reverse()`: Reverses the order of elements in the list.

#### Additional Helper Functions:

1. `getIndex(T value)`: Returns the index of the first occurrence of a value in the list.
2. `subList(int start, int end)`: Returns a sub-list containing elements from the specified start index to the end index.
3. `printHeadHelper(int start, int end) const`: Prints the elements of the list from the head to the specified end index.
4. `printTailHelper(int start, int end) const`: Prints the elements of the list from the specified start index to the tail.

#### Type Parameters:

- `T`: The type of elements stored in the list.

#### Usage:

- Implement concrete subclasses of `List` (e.g., LinkedList, ArrayList) to define specific list implementations.
- Override virtual member functions in concrete subclasses to customize list behavior.
- Use list operations to manage collections of elements efficiently.

#### Notes:

- The `List` class provides a flexible and reusable abstraction for managing collections of elements.
- Concrete implementations of `List` can vary in underlying data structures and performance characteristics.

### Class: Image

- **Purpose:** Handles the processing of the MNIST dataset.
- **Functionality:**
  - Load MNIST dataset.
  - Preprocess data (e.g., normalization, flattening).
  - Provide methods to access training and testing data.

### Class: kNN

- **Purpose:** Implements the k-nearest neighbors (kNN) classification algorithm.
- **Functionality:**
  - Accepts a training dataset.
  - Implements kNN algorithm for classification.
  - Utilizes list data structures for efficient storage and retrieval.
  - Provides methods to classify new data points.
  - Allows customization of k value and distance metric.
