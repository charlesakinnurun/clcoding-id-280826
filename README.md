# Python Set Comprehension & Modulo

A simple Python project demonstrating **set comprehension**, the **modulo operator (`%`)**, and how Python automatically removes duplicate values from a set.

## 📌 Code

```python
x = {i*i % 5 for i in range(10)}

print(len(x))
```

## 🔍 How It Works

### 1. `range(10)`

```python
range(10)
```

Generates the numbers:

```text
0, 1, 2, 3, 4, 5, 6, 7, 8, 9
```

### 2. Squaring Each Number

The expression:

```python
i * i
```

calculates the square of each number.

For example:

```text
0² = 0
1² = 1
2² = 4
3² = 9
4² = 16
5² = 25
...
```

### 3. Applying Modulo `% 5`

The `%` operator returns the remainder after division by 5.

```python
i*i % 5
```

The resulting values are:

```text
0, 1, 4, 4, 1, 0, 1, 4, 4, 1
```

### 4. Set Comprehension

The curly braces:

```python
{i*i % 5 for i in range(10)}
```

create a **set**.

Sets automatically remove duplicate values, so:

```text
0, 1, 4
```

are the only unique results.

Therefore:

```python
x = {0, 1, 4}
```

### 5. `len(x)`

Finally:

```python
len(x)
```

counts the number of unique elements in the set.

The output is:

```text
3
```

## 💡 Key Concepts

* **Set comprehension**
* **`range()`**
* **Modulo operator `%`**
* **Squaring numbers**
* **Removing duplicates with sets**
* **`len()`**

## ▶️ How to Run

Make sure Python is installed, then run:

```bash
python main.py
```

### Expected Output

```text
3
```

## 🎯 Purpose

This project is a small exercise for understanding how **set comprehensions and modular arithmetic** work together in Python.

It also demonstrates an important property of sets: **only unique values are stored**.

## 🛠️ Technologies

* Python 3
