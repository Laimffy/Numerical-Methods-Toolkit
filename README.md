# Numerical-Methods-Toolkit
A collection of root-finding algorithms (Bisection, Newton-Raphson, Secant) implemented in pure Python, focusing on accuracy and convergence.

## 🚀 Features
* Implemented using pure Python (no external libraries)
* Multiple root-finding methods:
  * Bisection Method
  * Fixed Point Iteration
  * Newton-Raphson Method
  * Secant Method
  * Secant Modified Method
  * Newton-Raphson Modified Method
* Handles convergence checks and iteration limits
* Easy-to-run scripts for testing different equations

## 📂 Project Structure
```text
iterative-root-finding/
│
├── methods/
│   ├── bisection.py
│   ├── newton.py
│   ├── secant.py
│
├── examples/
│   ├── example1.py
│   ├── example2.py
│
├── utils/
│   ├── functions.py
│
├── main.py
└── README.md
```

## ⚙️ Requirements
Python 3.x

(No additional libraries required)

Check your Python version: 
```Bash
  python --version
```

## ▶️ How to Run
1.Clone the repository
```Bash
git clone [https://github.com/your-username/iterative-root-finding.git](https://github.com/your-username/iterative-root-finding.git)
cd iterative-root-finding
```
2. Run the main program
```Bash
python main.py
```
3. Example usage (inside code)
You can define your function like this:
Python
```Bash
def f(x):
    return x**3 - x - 2
```
Then call a method:
```text
Python
```
```Bash
from methods.bisection import bisection

root = bisection(f, a=1, b=2, tol=1e-6, max_iter=100)
print("Root:", root)
```
## 🧠 Implemented Methods

### 🔹 Bisection Method
* Requires interval `[a, b]` where `f(a)` and `f(b)` have opposite signs
* Guaranteed convergence, but slower

### 🔹 Newton-Raphson Method
* Requires derivative `f'(x)`
* Fast convergence but sensitive to the initial guess

### 🔹 Secant Method
* Does not require a derivative
* Faster than Bisection, less stable than Newton

## 📊 Convergence Criteria
The iteration stops when:
* `|f(x)| < tolerance`, or
* Maximum iterations reached

## ⚠️ Notes
* These methods compute approximate roots, not exact values
* Poor initial guesses may lead to divergence (especially in the Newton method)
* Always choose appropriate intervals or starting points

## 🛠 Future Improvements
* Add a graphical visualization of convergence
* Add more numerical methods (False Position, Fixed Point, etc.)
* Build a CLI interface for easier usage
* Performance comparison between methods

## 📌 Author
**Laimffy**

Aspiring Software Engineer | Full-Stack Developer
