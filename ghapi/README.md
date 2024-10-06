### GitHub API

See [GitHub Docs](https://docs.github.com/en/rest/using-the-rest-api/getting-started-with-the-rest-api?apiVersion=2022-11-28&tool=curl) to learn the use of GitHub API, and accomplish two following sub-tasks.

#### Sub-task 1

Search GitHub repositories that use Python language, sorting them in descending order by the number of stars. Use [pagination](https://docs.github.com/en/rest/using-the-rest-api/using-pagination-in-the-rest-api) to show more results.

#### Sub-task 2

Write a Python program, it automatically checks whether a GitHub repository involves interoperation of Python and C/C++.

Input: Full name of a GitHub repository, e.g., `python-pillow/Pillow`, `giampaolo/psutil`, `scipy/scipy` or `encode/httpcore`.

Output: `Y` if the repository contains C or C++ (`.cpp` or `.cc`) code that includes `Python.h`. `N` if it does not. 

`#include <Python.h>` has to be declared when extending Python with C or C++ ([docs.python](https://docs.python.org/3/extending/extending.html)), it is a simple way to identify interoperation of Python and C/C++.

Think about the effect of the following practice: Search top-N Python repositories, and check existence of C/C++ code in each of them.