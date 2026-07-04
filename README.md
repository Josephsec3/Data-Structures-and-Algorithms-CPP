# Efficient Pair Counting using Hash Maps in C++

## 🚀 Project Overview
This project contains an optimized C++ solution designed for competitive programming and algorithmic problem-solving. The core objective is to count specific pairs in an array efficiently by transforming the mathematical condition to reduce time complexity.

## 🧠 Algorithmic Logic & Optimization
A naive brute-force approach to find pairs satisfying a specific condition would take **$O(N^2)$** time complexity, which is too slow for large inputs. 

This solution optimizes the process to **$O(N)$** time complexity by using the following mathematical transformation:
* The target condition involving array elements and their indices is rewritten so that all terms related to a single element are on one side (e.g., transforming $A[i] - i$).
* By mapping the frequency of these transformed values using `unordered_map` (Hash Map), we can count valid pairs in a single pass while traversing the array.

## 💻 Code Architecture
* **Fast I/O:** Utilizes `ios_base::sync_with_stdio(false); cin.tie(nullptr);` to untie C++ streams from C streams, significantly speeding up execution for large datasets.
* **Data Structure:** `unordered_map<int, int>` provides average $O(1)$ time complexity for insertions and lookups.
* **Data Types:** Uses `long long` for the counter (`done`) to prevent integer overflow when dealing with a high number of valid pairs.

## 🛠️ Requirements & Compilation
To compile and run the solution locally, use any standard C++ compiler supporting C++11 or higher:
```bash
g++ -O3 main.cpp -o solution
./solution
