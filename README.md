## 🔍 find_missing_number Function
Description
The find_missing_number function identifies the single missing number in a sequence of distinct numbers ranging from 0 to n. The input list contains n numbers from the range [0, n], with one number missing.

## 🔧 Function Definition
python
Copy
Edit
def find_missing_number(nums):
    n = len(nums)
    expected_sum = n * (n + 1) // 2
    actual_sum = sum(nums)
    return expected_sum - actual_sum
## 🧪 Example Usage
python
Copy
Edit
print(find_missing_number([3, 0, 1]))  # Output: 2
In the list [3, 0, 1], the numbers range from 0 to 3 (i.e., [0, 1, 2, 3]), but 2 is missing. The function correctly returns 2.

## 🧠 How It Works
The sum of numbers from 0 to n can be calculated using the formula:

expected_sum
=
𝑛
⋅
(
𝑛
+
1
)
2
expected_sum= 
2
n⋅(n+1)
​
 
The function subtracts the actual sum of the given list from this expected sum to find the missing number.

## ✅ Requirements
Python 3.x

No external libraries required

