# header

- 헤더파일 만들기

  ```c++
  // add.h
  // prototype 으로도 가능(e.g. int add(int a, int b))
  int add(int a, int b)
  {
      return a + b;
  }
  
  ```

  ```c++
  #include <iostream>
  #include "add.h"    // 상대경로도 가능
  using namespace std;
  
  int main()
  {
      cout << add(2, 3) << endl;
  }
  ```

- 헤더 가드

  - visual studio 에서 헤더에 h 확장자 파일을 생성하면 `#pragma once` 가 자동 생성된다.

  - 동일 함수를 include 해서 생기는 문제를 방지하기 위해 쓰인다.

    ```c++
    // 전처리기 표준 방식
    #ifndef SOME_FUCTION
    #define SOME_FUNCTION
    .
    .
    .
    #endif
    ```