# Technical Paper on Python, SQL & HTML Concepts

---

## 1. How to Handle Exceptions in Python?

- Exception handling is a mechanism to handle runtime errors gracefully without breaking program execution.

- Key Mechanisms:

    - try : contains code that may raise an exception.

    - except : catches and handles the exception.

    - else : runs if no exception occurs.

    - finally : always executes, used for cleanup tasks.

- Simple Example:

``` python

    try:
        num = 10 / 0
    except ZeroDivisionError:
        print("Cannot divide by zero")
    finally:
        print("Execution complete")

```

- Real-Life Example

    - Like wearing a seatbelt in a car: you cannot prevent accidents (errors), but you can reduce the impact safely (handling).

---

## 2. What Is Encapsulation in Python?

- Encapsulation is the concept of hiding internal data and restricting access to certain class components.

- How It Works:

    - Private variables using __var

    - Getter and Setter methods to access data safely

- Simple Example:

``` python

    class Bank:
        def __init__(self):
            self.__balance = 5000

        def get_balance(self):
            return self.__balance

```

- Real-Life Example:

    - ATM allows withdrawing money but does not show internal machine logic.

---

## 3. Is Python Compiled or Interpreted?

- Python is both compiled and interpreted.

- First, Python compiles source code into bytecode (.pyc).

- Then the Python Virtual Machine (PVM) interprets the bytecode line by line.

- Real-Life Example

    - Like writing a letter (compile) and then someone reads it aloud (interpretation).

---

## 4. What Are the Advantages of OOPs?

- Key Benefits:

    - Improves code reusability

    - Enhances data security using encapsulation

    - Simplifies debugging and modularity

    - Supports inheritance which reduces code duplication

    - Promotes clear structure using classes and objects

---

## 5. What Is the Difference Between WHERE and HAVING in SQL?
    | Feature                    | WHERE                    | HAVING                            |
    |----------------------------|--------------------------|--------------------------------   |
    | Purpose                    | Filters rows             | Filters results after aggregation |
    | Works With                 | Non-aggregated data      | Aggregated data                   |
    | Use of Aggregate Functions | Not allowed              | Allowed                           |


- Example

``` sql
SELECT department, COUNT(*)
FROM employees
GROUP BY department
HAVING COUNT(*) > 5;

```

---


## 6. What Are the Four Pillars of OOP?

- Encapsulation

- Inheritance

- Polymorphism

- Abstraction

---

## 7. What Is the Single Responsibility Principle (SRP)?

- A class should have only one reason to change.

- Each class should do only one job.

- Example

    - Class InvoiceCalculator should only compute invoice, not print or save it.

## 8. What Are the Three Ways to Apply CSS?
    | Type         |	Usage                                  |
    |--------------|-------------------------------------------|
    | Inline CSS   |	Inside HTML tags using style attribute |
    | Internal CSS |	Inside <style> tag within <head>       |
    | External CSS |	Linking .css file using <link>         |

---

## 9. What Is the Difference Between DELETE and TRUNCATE?

    | Type         | Usage                                       |
    |--------------|---------------------------------------------|
    | Inline CSS   | Inside HTML tags using `style` attribute    |
    | Internal CSS | Inside `<style>` tag within `<head>`        |
    | External CSS | Linking `.css` file using `<link>`          |

---

## 10. What Is the Difference Between Padding and Margin?

    | Padding                                      | Margin                                         |
    |----------------------------------------------|------------------------------------------------|
    | Space inside an element (around content)     | Space outside an element (around border)       |
    | Affects element size                         | Affects element spacing outside                |

---

## 11. What Is the Open/Closed Principle?

- Software entities should be open for extension but closed for modification

- Meaning

    - New functionality should be added without changing existing code.

---

## 12. What Is Encapsulation?

- Encapsulation is the bundling of data and methods inside a class and restricting direct access to internal variables.

- Helps protect data integrity.