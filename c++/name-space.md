# Namespace

  - 같은 namespace를 써서 생기는 문제를 해결

  ```c++
  namespace OwnSpace
  {
      int add(int a, int b)
      {
          return a + b;
      }   
  }
  
  int add(int a, int b)
  {
      return a + b;
  }   
  ```

  - namespace 안에 namespace 도 가능
  - OwnSpace의 add 를 호출하고 싶다면 OwnSpace::add(3, 4) 와 같이 한다.
  - 이중으로 namespace 안에 함수가 있다면 `using namespace OwnSpace1::OwnSpace2;` 과 같이 써서 add(3, 4) 만 호출 가능

