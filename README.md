# Array Reversal Implementation - Two-Pointer Technique

C++ implementation to reverse an array in-place. The algorithm uses the two-pointer approach, which is memory-efficient and fast.

---

## 🚀 How the Algorithm Works

The algorithm uses two markers (pointers): **Start** and **End**.

1. **Initialize:** `start` at the first index (0) and `end` at the last index (`size - 1`).
2. **Swap:** Swap the elements at `arr[start]` and `arr[end]`.
3. **Move Pointers:** Increment `start` and decrement `end`.
4. **Repeat:** Continue the process until the `start` pointer meets or crosses the `end` pointer.

## 📊 Complexity Analysis

| Metric | Complexity | Description |
| :--- | :--- | :--- |
| **Time Complexity** | $O(n)$ | We iterate through half the array ($n/2$ swaps), which simplifies to linear time. |
| **Space Complexity** | $O(1)$ | The reversal is done "in-place," meaning no extra memory is used regardless of array size. |

---

## 💻 Code Overview

The core logic is contained in the `reverseArray` function:

```cpp
void reverseArray(int arr[], int sz) {
    int start = 0; 
    int end = sz - 1;
    
    while (start <= end) {
        swap(arr[start], arr[end]); 
        start++;
        end--; 
    }
}
```

.

🛠️ Clone the repo:
```
git clone [https://github.com/your-username/array-reverse-cpp.git](https://github.com/your-username/array-reverse-cpp.git)
```
