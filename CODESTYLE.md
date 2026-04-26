# CODESTYLE
---
codestyle of `C` language ( using CLion )

Formatting

Indentation

4 spaces per indent level.


Braces and Layout

static int doSomething(int value) {
    if (value < 0) return -1;
    if (value == 0) return 0;
    return value * 2;
}

Rules:

Keep function signatures on one line.

Opening brace on the same line.

Single-line if allowed for simple statements.



---

Early Return Pattern

int process(int x) {
    if (x < 0) return -1;
    if (x == 0) return 0;
    return x + 1;
}

Avoid:

if (x < 0) {
    return -1;
} else {
    return 0;
}


---

Condition Formatting

if (a == b)
if (x > 10)

Rules:

Spaces around operators.

Split complex conditions into multiple steps.



---

Naming Convention

Functions and Variables

int getValue();
int maxCount;

Use camelCase.


Constants

#define MAX_SIZE 1024

Use UPPER_CASE.


Structs

typedef struct {
    int x;
    int y;
} Point;


---

Data Handling

Boolean

#include <stdbool.h>

bool isValid(int x) {
    return x > 0;
}

const Usage

const int maxValue = 10;


---

Function Design

One function, one responsibility.

Aim for 20–30 lines.

Minimize side effects.



---

Example

#include <stdio.h>
#include <stdbool.h>

#define SPECIAL_VALUE 2222

static int maybeVeryImportantFn(int a) {
    if (a < 5) return a;
    if (a - 5 == 7) return SPECIAL_VALUE;
    return 5 - a;
}

int main(void) {
    printf("%d\n", maybeVeryImportantFn(5));
    return 0;
}


---

Anti-Patterns

Unnecessary else

if (x) return 1;
else return 2;

Macro misuse

#define add(a,b) a+b

Overly complex expressions

return (a+b)*(c-d)/x+y;

Prefer:

int temp = (a + b) * (c - d);
return temp / x + y;


---

Trade-offs

Aspect	JS-like C Style

Readability	High
Safety	Preserved
Traditional	Low
Team Fit	Depends



---

Final Rule

Write code that reads like JavaScript, but behaves like C.
---
codestyle of `JS` language ( using visual-studio-code-bin(arch) )

`tab-indent: 2`

```quotes-default-use: ` ```

`*.js`

[NAVER-JS-CODESTYLE](https://github.com/naver/eslint-config-naver/blob/master/STYLE_GUIDE.md)
---
codestyle of `PYTHON` language ( using pycharm or visual-studio-code-bin(arch) )

`tab-indent: 4`

`*.py`

[PEP-8](https://github.com/naver/eslint-config-naver/blob/master/STYLE_GUIDE.md)
```python
import this
```
---
