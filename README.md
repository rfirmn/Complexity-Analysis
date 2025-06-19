# complexity analysis with Box Sorting in C

This program is a simple simulation of generating random numbers, organizing them into boxes, and sorting them using two classic algorithms — Bubble Sort and Quick Sort. It also includes performance timing for sorting operations.

## 📦 Box Analogy Explanation

In this program, each **Box** is analogous to a physical display or container that can hold items with weight. Here's how the analogy works:

- Each **number** (between 5 and 20) represents the **weight (in kilograms)** of an individual item.
- A **Box** represents a **physical container/display**, such as a shelf or storage bin, that can hold multiple items.
- Each Box has a **maximum capacity of 100 items**, meaning the total number of items (not weight) it can contain is limited to 100.
- This simulates a real-world scenario where boxes (displays) are filled with objects of various weights, and you're interested in managing and organizing them efficiently.

This analogy can help users better understand how data structures in programming (like arrays and structs) can be used to model real-life organizational problems, such as load distribution and sorting based on weight.

## 🧠 Program Overview

The program performs the following:

- Generates 1000 random integers between 5 and 20
- Allows the user to insert these numbers into up to 10 boxes (100 numbers per box)
- Provides options to sort the array using bubble sort and quick sort, and measure execution time
- Displays box contents and remaining unboxed numbers

## 🗂️ Data Structure

### `struct Box`

Holds a fixed-size array of integers:

- `numbers[MAX_NUMBERS]`: Holds the actual numbers
- `count`: Number of elements in the box

## 🔧 Key Functionalities

### `bubbleSort(int arr[], int n)`

Implements the Bubble Sort algorithm to sort an array of `n` integers.

### `quickSort(int arr[], int low, int high)`

Implements the Quick Sort algorithm recursively for better performance.

### `displayBox(Box boxes[], int boxIndex, int totalBoxes)`

Displays the contents of a specific box and the count of elements in it.

### `displayAllNumbers(int angka[], int totalNumbers)`

Prints all numbers from the given array.

## 🖥️ Menu Interface

The `main()` function provides the following menu:

1. Insert numbers into boxes (max 10 boxes, 100 numbers each)
2. Sort numbers using Bubble Sort and Quick Sort (with execution time in milliseconds)
3. View a specific box's contents
4. Display all numbers
5. Show numbers not yet placed in any box
6. Exit

## ⏱️ Sorting Performance Example

When option 2 is selected, the program displays:

```
Waktu Bubble Sort: 82.00 ms
Waktu Quick Sort: 1.30 ms
```

This gives users a practical demonstration of performance difference.

## 📌 Sample Usage

```c
Menu:
1. Masukkan angka ke dalam box
2. Urutkan angka
3. Tampilkan isi Box
4. Tampilkan semua angka
5. Angka yang belum masuk
6. Keluar
Masukkan pilihan: 1
Angka berhasil dimasukkan ke dalam Box 1.
```

## 🚀 Final Notes

This project provides hands-on practice for:

- Random number generation
- Array manipulation
- Basic sorting algorithms
- Struct usage in C
- Performance measurement using `clock()`

It is a great starting point for learners who want to understand the efficiency of sorting methods and organize data in structured containers like "boxes".

Feel free to extend it by:

- Adding other sorting algorithms
- Supporting dynamic memory allocation
- Visualizing data with graphs
- Exporting box data to files

