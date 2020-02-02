# Base

## 변수 초기화하는 두가지 방법

```c++
int x = 123;
int x(123);    
```

## std:: 생략하기

```c++
#include <iostream>

using namespace std;    // 컴파일러가 cout 만나면 std namespace에서 찾아준다.
int main()
{
    cout << "Hello, world!" << endl;
}
```

## C++ 특징

- c++ 은 함수 안에서 함수 정의가 되지 않는다.

## Forward Declaration

```c++
#include <iostream>

using namespace std;
int subtract(int a, int b);    // 컴파일러가 순서대로 읽으므로 문제될 상황을 forward declaration 으로 해결

int main()
{
    cout << subtract(1, 2) << endl;
}

int subtract(int a, int b)
{
    return a - b
}
```