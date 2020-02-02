# 전처리기

  - Case 1

    ```c++
    #include <iostream>
    #define COUNT 4    // 메크로는 보통 대문자로 표현. 코드에서 만나면 이 값으로 대치됨. 잘 쓰진 않는다
    using namespace std;
    int main()
    {
        cout << COUNT << endl;
    }
    ```

  - Case 2

    ```c++
    #include <iostream>
    #define MAC
    using namespace std;
    int main()
    {
        #ifdef MAC
        cout << "MAC이다" <<endl;
        #endif
        #ifndef MAC
        cout << "MAC이 아니다" << endl;
        #endif
    }
    
    // 주로 운영제체 확인하거나 멀티플랫폼 소프트웨어 개발시 쓰임 
    ```