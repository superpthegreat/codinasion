## Write a program to swap two numbers without using third variable.

```
Input:  a=10 b=20
Output: a=20 b=10
```

---

<CodeBlock slots="heading, code" repeat="3" languages="Python, C, C++" />

#### Python

```python
# define variables
a = 10
b = 20

# swap numbers
a, b = b, a

# print result
print(a, b)
```

#### C

```c
#include <stdio.h>

int main()
{
  // initialize two numbers
  int number1, number2;
  printf("enter two numbers ");

  // taking input from user
  scanf("%d %d", &number1, &number2);

  // swapping the numbers
  number1 = number1 + number2;
  number2 = number1 - number2;
  number1 = number1 - number2;

  // after swapping output
  printf("after swap two numbers are %d and %d", number1, number2);

  return 0;
}
```

#### C++

```cpp
#include <iostream>

void swap(int &x, int &y)
{
  x = x + y;
  y = x - y;
  x = x - y;
}

int main()
{
  int a, b;
  std::cout << "a : ";
  std::cin >> a;
  std::cout << "b : ";
  std::cin >> b;

  swap(a, b);

  std::cout << "\na = " << a << "\nb = " << b << "\n";

  return 0;
}
```
