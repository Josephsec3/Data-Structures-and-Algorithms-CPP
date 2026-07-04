# Competitive Programming: Efficient Index-Value Matching in C++

## 🧠 Problem Logic & Optimization
The project solves an algorithmic problem where we need to find pairs $(i, j)$ such that:
$$a_j - a_i = j - i$$

A naive brute-force solution would take $O(N^2)$ time by comparing every pair, which causes a **Time Limit Exceeded (TLE)** error on large datasets. 

By mathematically rearranging the equation:
$$a_j - j = a_i - i$$

We can transform the problem into finding elements that yield the same value when subtracted by their index. 

## 🚀 Technical Implementation
* **Time Complexity:** $O(N)$ - The array is traversed only once.
* **Space Complexity:** $O(N)$ - Utilizes a Hash Map (`std::unordered_map`) for fast lookups.
* **I/O Optimization:** Uses `ios_base::sync_with_stdio(false); cin.tie(nullptr);` for lightning-fast competitive programming input/output operations.

## 💻 How to Run
Ensure you have a C++17 compatible compiler installed.
```bash
g++ -O3 main.cpp -o solution
./solution
