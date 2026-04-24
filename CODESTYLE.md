# CODESTYLE
---
codestyle of `C` language ( using CLion )

`tab-indent: 4`

`*.c`
```c
#include <stdio.h>

#define MAYBE_IMPORTANT_MACRO 1

struct PascalCase {
  int a;
  int b;
};

int
maybe_very_important_fn(int a)
{
  if (a < 5) { return a; }
  else if (a-5==7) { return 2222; }
  else { return 5-a; }
  return 0;
}

int
main()
{
  maybe_very_important_fn(5);
  maybe_very_important_fn(MAYBE_IMPORTANT_MACRO);

  return 0;
}
```

`*.h`
```c
#ifndef __Header_Guard_H__
#define __Header_Guard_H__

// very very complex code

#endif
```
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
