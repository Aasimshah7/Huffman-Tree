# Huffman Tree – Lossless Data Compression in Java

## Overview

This project implements a **Huffman Tree Abstract Data Type (ADT)** in Java to demonstrate **lossless data compression** using tree-based data structures. Huffman coding assigns variable-length, prefix-free binary codes to characters based on their frequencies, minimizing overall encoded size.

The project combines theoretical foundations with practical implementation and performance analysis across diverse datasets.

---

## Problem Domain

Efficient storage and transmission of data are critical in modern computing. Huffman coding is a widely used lossless compression technique that:

* Assigns **shorter codes to frequent characters**
* Assigns **longer codes to rare characters**
* Guarantees **optimal average code length**

This project focuses on building, encoding, and decoding data using a Huffman Tree while analysing compression efficiency.

---

## Key Features

* Builds a **frequency map** from input text
* Constructs a **Huffman Tree** using a **priority queue**
* Generates **prefix-free Huffman codes** via tree traversal
* Encodes text into compressed binary form
* Decodes compressed data back to its original form
* Handles edge cases (empty files, corrupted data)
* Includes **performance benchmarking** and analysis

---

## Data Structures Used

* **Binary Trees** – Core structure of the Huffman Tree
* **Priority Queue (Min-Heap)** – For optimal node selection during tree construction
* **Maps (HashMaps)** – To store character frequencies and Huffman codes

---

## Implementation Approach

1. **Frequency Analysis** – Count character occurrences in the input
2. **Tree Construction** – Iteratively merge least-frequent nodes using a priority queue
3. **Code Generation** – Traverse the tree to assign binary codes
4. **Encoding** – Replace characters with their Huffman codes
5. **Decoding** – Reconstruct original text from encoded data

---

## Experiments & Results

The algorithm was tested on multiple datasets including:

* Large literary texts
* Highly repetitive patterns
* Sparse data
* Unicode and emoji-based text

### Highlights:

* Compression savings up to **97.5%** on highly redundant data
* Average compression savings of **~61%** across datasets
* Correct restoration of **11/12 test files** (corrupted file detected correctly)
* Scales efficiently with large input sizes

---

## Key Takeaways

* Huffman coding is highly effective for redundant and sparse data
* Compression efficiency depends heavily on character frequency distribution
* Tree-based data structures are powerful tools for real-world optimization problems

---

## Technologies

* **Java**
* **Priority Queues & Trees**
* **JUnit (Testing & Validation)**
